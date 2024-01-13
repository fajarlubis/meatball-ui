<template>
  <aside class="h-screen">
    <nav class="h-full flex flex-col bg-white border-r shadow-sm">
      <div class="p-4 pb-2 flex justify-between items-center">
        <img src="https://img.logoipsum.com/243.svg" class="w-32" alt="" />
        <UButton icon="i-heroicons-chevron-double-left-20-solid" size="md" color="primary" square variant="solid" />
      </div>

      <ul class="flex-1 px-3">
        <li class="relative flex items-center py-2 px-3 my-1 font-medium rounded-md cursor-pointer">Test</li>
      </ul>

      <div class="border-t flex p-3">
        <img src="https://ui-avatars.com/api/?background=c7d2fe&color=3730a3&bold=true" alt=""
          class="w-10 h-10 rounded-md" />
        <div class="flex justify-between items-center w-52 ml-3">
          <div class="leading-4">
            <h4 class="font-semibold">John Doe</h4>
            <span class="text-xs text-gray-600">johndoe@mail.com</span>
          </div>
          <UIcon name="ellipsis-vertical-20-solid" />
        </div>
      </div>
    </nav>
  </aside>
</template>

<script lang="ts" setup>

</script>

<style></style>