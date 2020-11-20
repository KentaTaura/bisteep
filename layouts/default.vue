<template>
  <div>
    <transition name="fade" mode="out-in" appear>
      <Nuxt />
    </transition>
  </div>
</template>

<script>
export default {
  transition: 'fade'
}
</script>

<style>

</style>
