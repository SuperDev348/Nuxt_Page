<template>
  <nav class="fixed w-full z-30 top-0 h-20 bg-white px-20 rela">
    <div
      class="w-full mx-auto flex flex-wrap items-center justify-between items-center mt-0 py-4"
    >
      <div class="pl-4 flex items-center">
        <div class="text-3xl cursor-pointer">HSD</div>
      </div>
      <div class="flex items-center">
        <div class="text-xl text-gray cursor-pointer" style="color: gray;">
          <fa :icon="['fas', 'bell']" />
        </div>
        <div class="px-8 cursor-pointer">
          <img class="w-8 h-8 rounded-full" src="~assets/img/default-avatar.jpg" alt />
        </div>
        <div class="">
          <button class="text-sm items-center text-white py-2 px-5 bg-black rounded-lg">WRITE</button>
        </div>
      </div>
    </div>
  </nav>
</template>

<script>

export default {
  name: 'TheHeader',
  components: {
  },
  data() {
    return {
    }
  },
  computed: {
  },
  methods: {
  },
  mounted() {
  },
  beforeDestroy() {
  }
}
</script>
