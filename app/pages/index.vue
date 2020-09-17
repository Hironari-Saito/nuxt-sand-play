<template>
  <div>
    <div class="container-hero">
      <nuxt-link to="/design">See Design</nuxt-link>
    </div>
    <div class="container-hero bg-gray-100">
      <button class="animate-spin">Spin</button>
      <button class="animate-ping">Ping</button>
      <button class="animate-pulse">Pulse</button>
      <button class="animate-bounce">Bounce</button>
    </div>
  </div>
</template>

<style lang="stylus" scoped>
.container-hero {
  @apply h-screen;
  @apply flex items-center justify-center;
}
a {
  @apply p-3;
  @apply border;
  @apply transition duration-300;
  @apply border-current;

  color: $base-color;
  &:hover {
    @apply bg-green-400;
    @apply text-white;
  }
}
</style>
