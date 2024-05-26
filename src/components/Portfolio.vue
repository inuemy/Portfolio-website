<script setup>
const slides = [
  'Yui',
  'ながのケーキ',
  'Bookers2',
  'Bookers1',
]
</script>

<template>
  <h2>Portfolio</h2>
  <v-carousel
    height="400"
    width="400"
    show-arrows="hover"
    cycle
    hide-delimiter-background
  >
    <v-carousel-item
      v-for="(slide, i) in slides"
      :key="i"
    >
      <v-sheet
        class="background-sheet"
        height="100%"
      >
        <div class="d-flex fill-height justify-center align-center">
          <div class="text-h2">
            {{ slide }}
          </div>
        </div>
      </v-sheet>
    </v-carousel-item>
  </v-carousel>
</template>

<style scoped>
.background-sheet {
  background-image: url("src/assets/no-image.png");
  background-size: auto; /* 画像を要素に合わせて拡大・縮小 */
  background-position: center; /* 画像の位置を中央に設定 */
}
</style>
