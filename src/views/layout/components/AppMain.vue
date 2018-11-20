<template>
  <section class="app-main" id="app-main" @click.stop="appMain">
    <transition name="fade" mode="out-in">
      <!-- <router-view :key="key"></router-view> -->
      <router-view></router-view>
    </transition>
  </section>
</template>

<script>
export default {
  name: 'AppMain',
  computed: {
    // key() {
    //   return this.$route.name !== undefined ? this.$route.name + +new Date() : this.$route + +new Date()
    // }
  },
  methods:{
    appMain(){
      console.log(this.$route)
    }
  }

}
</script>
