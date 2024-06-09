<template>
  <div class="categories-card">
    <ul class="categories-card--list">
      <li class="active-categori">
        <nuxt-link to="/">Bugün</nuxt-link>
      </li>
      <li>
        <nuxt-link to="/">Ortadoğu</nuxt-link>
      </li>
      <li><nuxt-link to="/">Avrupa</nuxt-link></li>

      <li class="responsive-hidden-tablet">
        <nuxt-link to="/">Amerika</nuxt-link>
      </li>
      <li class="responsive-hidden-tablet">
        <nuxt-link to="/">Asya</nuxt-link>
      </li>

      <li class="responsive-hidden-mobil">
        <nuxt-link to="/">Afrika</nuxt-link>
      </li>
      <li class="responsive-hidden-mobil">
        <nuxt-link to="/">Antartika</nuxt-link>
      </li>
      <li class="responsive-hidden-mobil">
        <nuxt-link to="/">Okyanusya</nuxt-link>
      </li>

      <li>
        <button>
          <Icon name="heroicons:ellipsis-horizontal" color="black" size="30" />
        </button>
      </li>
    </ul>
    <div class="categories-card--rss">
      <span>Rss </span>
      <Icon name="arcticons:rssreader" size="23" />
    </div>
  </div>
</template>

<style lang="scss" src="./categories-card.scss" />
