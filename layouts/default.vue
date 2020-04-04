<template>
  <div class="l-content">
    <l-header />
    <transition
      enter-active-class="animated fadeInUp"
      leave-active-class="fadeOutDown"
    >
      <nuxt />
    </transition>
  </div>
</template>

<script>
import LHeader from '@/components/layout/Header'
export default {
  components: {
    LHeader
  }
}
</script>
