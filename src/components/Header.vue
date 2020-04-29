<template>
  <header class="header">
    <g-link to="/"><h1 style="margin-bottom: 10px">😼 {{ siteName }} 🇨🇮</h1></g-link>
    <ClientOnly>
      <ThemeToggle />
    </ClientOnly>
  </header>
</template>

<script>
export default {
  props: ['siteName'],
  
  components: { ThemeToggle: () => import('@/components/ThemeToggle') }
}
</script>

<style lang="scss">
  .header {
    display:flex;
    align-items: center;
    justify-content: space-between;
    border-bottom: 1px dotted #9a9a9a;
    a {
      color:inherit;
      border-bottom: none;
    }
  }
</style>
