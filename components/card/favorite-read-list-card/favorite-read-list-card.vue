<template>
  <div class="favorite-read-list-card">
    <div class="favorite-read-list-card__head">
      <span>Çok Okunan / Çok İzlenen</span>
    </div>
    <ul class="favorite-read-list-card__list">
      <li class="favorite-read-list-card__list__item" v-for="item in 7">
        <p class="favorite-read-list-card__list__item--text">
          Taş sokakları ve tarihi yapılarıyla Heppenheim
        </p>
        <span class="favorite-read-list-card__list__item--num">{{ item }}</span>
      </li>
    </ul>
  </div>
</template>
<style lang="scss" src="./favorite-read-list-card.scss"></style>
