<template>
  <div class="other-categories-banner-next-news">
    <ul class="other-categories-banner-next-news__list">
      <li
        class="other-categories-banner-next-news__list--item"
        :class="{
          'other-categories-banner-next-news__list--active': item === 1,
        }"
        v-for="item in 7"
      >
        CHP’ye yakınlığıyla bilinen Şaban Sevinç’ten Kılıçdaroğlu’na eleştiri:
        Değişim çağrılarını bastırmak için
      </li>
    </ul>
  </div>
</template>
<style lang="scss" src="./other-categories-banner-next-news.scss"></style>
