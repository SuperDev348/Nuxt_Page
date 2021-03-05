<template>
  <div class="bg-pink-100 grid grid-cols-6 gap-4 -top-32">
    <div class="bg-white col-start-2 col-span-4 p-32">
        <highlightable-menu
          @share="onShare"
          @highlight="onHighlight"
        >
          <h1 class="text-4xl text-center" style="font-family: tinos;">I was wrong about macOS Big Sur...</h1>
        </highlightable-menu>
        <highlightable-menu
          @share="onShare"
          @highlight="onHighlight"
        >
          <p class="pt-10">
            A month ago, I published my story about macOS Big Sur review. I wrote about how macOS Big Sur has a big design overhaul, however with a performance bummer. Last time when I reviewed it, my early-2020 Base Model MacBook Pro had a significant performance decrease in speed and battery life, which made me unhappy with the update. Take note that this was the first public release of macOS Big Sur. 
          </p>
        </highlightable-menu>
        <highlightable-menu
          @share="onShare"
          @highlight="onHighlight"
        >
          <p class="pt-10">
            Not long ago after I published that story, Apple released a new update for Big Sur, which is 11.1. I also received some feedback from the Medium community here saying that I used too much non-Apple application, which has a significant hit on performance and battery (in particular, Google Chrome).
          </p>
        </highlightable-menu>
        <highlightable-menu
          @share="onShare"
          @highlight="onHighlight"
        >
          <p class="pt-10">
            That’s why, I decided to have a little experiment, which is to go full-on Safari. I also decided to not charge my MacBook Pro not often and see how much it lasts for a single charge.
          </p>
        </highlightable-menu>
        <highlightable-menu
          @share="onShare"
          @highlight="onHighlight"
        >
          <p class="pt-10">
            The result was surprising to me and I have to admit that I ate up my own words on my previous story. It is crazy how heavy the impact is from a third-party application. Well, Chrome is definitely a fast browser, but also fast in draining my MacBook’s battery.
          </p>
        </highlightable-menu>
        <highlightable-menu
          @share="onShare"
          @highlight="onHighlight"
        >
          <p class="pt-10">
            My experience with Safari is very smooth, as I don’t need to worry about plugging my MacBook oftenly. Checking emails, social media, watching YouTube and writing stories in Medium did not affect my battery significantly. Plus, I also get better security with Safari with its latest tracking prevention update.
          </p>
        </highlightable-menu>
        <highlightable-menu
          @share="onShare"
          @highlight="onHighlight"
        >
          <p class="pt-10">
            Last time when I use Safari in Catalina, YouTube only capable of showing 1080p videos at its max resolution. Now, the new update allows Safari to view up to 4k HDR content, which makes me happier. It means that I can continue using Safari to watch high-quality videos.
          </p>
        </highlightable-menu>
        
    </div>
  </div>
</template>

<script>
import HighlightableMenu from '@/components/HighlightableMenu'
export default {
  name: 'Article',
  components: {
    "highlightable-menu": HighlightableMenu,
  },
  data() {
    return {
      isTooltipOpen: false,
      tooltipX: 100,
      tooltipY: 100,
      offsetX: 0,
      offsetY: 0
    }
  },
  mounted() {
    // console.log(this.tooltip)
  },
  computed: {
  },
  methods: {
    onShare (text) {
      console.log('share:', text)
    },

    onHighlight (text) {
      console.log('highlight:', text)
    }
  },
  mounted() {
  },
  beforeDestroy() {
  }
}
</script>
<style>
  ::selection {
    background: #ffb7b7; /* WebKit/Blink Browsers */
  }
  ::-moz-selection {
    background: #ffb7b7; /* Gecko Browsers */
  }
</style>
