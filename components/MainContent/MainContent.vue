<template>
  <div class="w-full h-full flex flex-col">
    <slot class="flex-1" name="header"></slot>

    <div class="bg-gray-50 w-full h-max flex-1">
      <div class="2-full h-full p-5 mx-auto max-w-screen-xl">
        <slot name="content"></slot>
      </div>
    </div>
  </div>
</template>
