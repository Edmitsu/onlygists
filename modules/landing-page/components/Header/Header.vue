<script setup lang="ts"></script>

<template>
  <header class="w-full shadow">
    <nav class="bg-white px-4 lg:px-6 py-2.5">
      <div class="flex justify-center md:justify-between items-center mx-auto max-w-screen-xl">
        <div class="flex item-center">
          <NuxtLink to="/"> <Logo /> </NuxtLink>
        </div>
        <div class="hidden md:flex items-center">
          <Button label="Continuar como creator" iconPos="right" icon="pi pi-arrow-right" />
        </div>
      </div>
    </nav>
  </header>
</template>
