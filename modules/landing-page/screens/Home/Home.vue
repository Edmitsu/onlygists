<script setup lang="ts">
import Header from '../../components/Header/Header.vue'
import Hero from '../../components/Hero/Hero.vue'

const router = useRouter()
const handleLogin = () => {
  router.push('/auth/login')
}
</script>

<template>
  <MainContent>
    <template #header>
      <Header @wants-be-creator="handleLogin" />
    </template>

    <template #content>
      <Hero @wants-be-creator="handleLogin" />
    </template>
  </MainContent>
</template>
