<template>
  <div class="navbar-categories">
    <div class="navbar-categories__list">
      <nuxt-link to="/">Bugün</nuxt-link>
      <nuxt-link class="navbar-categories__list--acitive" to="/"
        >Spor <Icon name="tabler:star-filled" size="14" color="white"
      /></nuxt-link>
      <nuxt-link class="navbar-categories__list--acitive" to="/"
        >Ekonomi
        <Icon name="tabler:star-filled" size="14" color="white" />
      </nuxt-link>
      <nuxt-link class="navbar-categories__list--responsive-hidden" to="/"
        >Yazarlar</nuxt-link
      >
      <nuxt-link class="navbar-categories__list--responsive-hidden" to="/"
        >Dünya</nuxt-link
      >
      <nuxt-link class="navbar-categories__list--responsive-hidden" to="/"
        >Hayat</nuxt-link
      >
      <nuxt-link class="navbar-categories__list--responsive-hidden" to="/"
        >Gündem</nuxt-link
      >
      <button class="hover:bg-[#0000002e] rounded">
        <Icon name="heroicons:ellipsis-horizontal" color="white" size="30" />
      </button>
    </div>
    <div class="navbar-categories__live">
      <nuxt-link class="navbar-categories__live__button" to="/">
        <span class="navbar-categories__live__button--destop">
          tvnet
          <Icon
            name="fluent:live-24-filled"
            size="21"
            color="white"
            class="mx-3 my-auto"
          />
          canlı
        </span>
        <span class="navbar-categories__live__button--mobil">C</span>
      </nuxt-link>
    </div>
  </div>
</template>
<style lang="scss" src="./navbar-categories.scss"></style>
