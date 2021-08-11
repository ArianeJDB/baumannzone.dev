<template>
  <section class="bg-white pt-16 pb-20 px-4 sm:px-6 lg:pt-24 lg:pb-28 lg:px-8">
    <div
      class="relative max-w-lg mx-auto divide-y-2 divide-gray-200 lg:max-w-7xl"
    >
      <div>
        <h2
          class="
            text-3xl
            tracking-tight
            font-extrabold
            text-gray-900
            sm:text-4xl
          "
        >
          Skins
        </h2>
      </div>
      <!-- eslint-disable-next-line vue/no-v-html -->
      <div class="prose prose-purple" v-html="skins" />
    </div>
  </section>
</template>

<script>
import skins from '@/components/SkinsPage/skins.md'

export default {
  // streaming-outfits
  name: 'Skins',
  computed: {
    skins() {
      return skins
    },
  },
}
</script>
