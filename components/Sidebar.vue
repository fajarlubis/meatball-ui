<template>
  <aside class="h-screen">
    <nav class="h-full inline-flex flex-col bg-white border-r shadow-sm">
      <div class="p-4 pb-2 flex justify-between items-center">
        <img src="https://img.logoipsum.com/243.svg"
          :class="`overflow-hidden transition-all ${expanded ? 'w-32' : 'w-0'}`" alt="" />
        <UButton @click="expanded = !expanded"
          :icon="expanded ? 'i-heroicons-chevron-double-left-20-solid' : 'i-heroicons-chevron-double-right-20-solid'"
          size="md" color="primary" square variant="solid" />
      </div>

      <ul class="flex-1 px-3">
        <li
          :class="`relative flex items-center py-2 px-3 my-1 font-medium rounded-md cursor-pointer text-gray-600 transition-colors group`">
          Test
        </li>
      </ul>

      <div class="border-t flex p-3">
        <img src="https://ui-avatars.com/api/?background=c7d2fe&color=3730a3&bold=true" alt=""
          class="w-10 h-10 rounded-md" />

        <div
          :class="`flex justify-between items-center overflow-hidden transition-all ${expanded ? 'w-52 ml-3' : 'w-0'}`">
          <div class="leading-4">
            <h4 class="font-semibold text-gray-600">John Doe</h4>
            <span class="text-xs text-gray-600">johndoe@mail.com</span>
          </div>
          <UPopover :popper="{ placement: 'top-start' }">
            <UButton color="white" trailing-icon="i-heroicons-ellipsis-vertical-20-solid" />

            <template #panel>
              <div class="p-4">
                <!-- <UVerticalNavigation :links="links">
                  <template #default="{ link }">
                    <span class="group-hover:text-primary relative">{{ link.label }}</span>
                  </template>
                </UVerticalNavigation> -->
              </div>
            </template>
          </UPopover>
        </div>
      </div>
    </nav>
  </aside>
</template>

<script lang="ts" setup>
const expanded = useState('expanded', () => true)

// const links = [{
//   label: 'Vertical Navigation',
//   to: '/navigation/vertical-navigation'
// }, {
//   label: 'Command Palette',
//   to: '/navigation/command-palette'
// }, {
//   label: 'Table',
//   to: '/data/table'
// }]
</script>

<style></style>