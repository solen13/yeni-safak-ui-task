<template>
  <div class="slider-news-main">
    <div class="slider-news-main__header">
      <span class="slider-news-main__header--active"
        >Günün Manşetleri
        <hr width="50" />
      </span>
      <Icon
        class="mx-7"
        name="material-symbols-light:radio-button-unchecked"
        size="9"
        color="#747474"
      />
      <span>Basılı Gazete Haberleri</span>
    </div>

    <div class="slider-news-main__main">
      <div class="slider-news-main__main__container">
        <button class="slider-news-main__main__container--left-button">
          <Icon name="material-symbols:arrow-left" size="22" color="black" />
        </button>

        <slider-main-card />

        <button class="slider-news-main__main__container--right-button">
          <Icon name="material-symbols:arrow-right" size="22" color="black" />
        </button>
      </div>
    </div>

    <div class="slider-news-main__slider-number">
      <ul class="slider-news-main__slider-number__list">
        <li
          class="slider-news-main__slider-number__list--item"
          v-for="item in 25"
          :class="{
            'slider-news-main__slider-number__list--active': item == 1,
          }"
        >
          {{ item }}
        </li>
      </ul>
      <div class="slider-news-main__slider-number__button-content">
        <button class="slider-news-main__slider-number__button-content--button">
          TM
        </button>
        <div class="slider-news-main__slider-number__button-content--button">
          <button>
            <Icon name="material-symbols:arrow-left" size="17" color="white" />
          </button>
          <Icon
            class="mx-1"
            name="material-symbols-light:radio-button-unchecked"
            size="9"
            color="white"
          />
          <button>
            <Icon name="material-symbols:arrow-right" size="17" color="white" />
          </button>
        </div>
      </div>
    </div>
    <div class="slider-news-main__slider-number-responsive">
      <ul class="slider-news-main__slider-number-responsive__list">
        <li
          class="slider-news-main__slider-number-responsive__list--item"
          v-for="item in 15"
        >
          <Icon
            class="mx-1"
            name="material-symbols-light:radio-button-unchecked"
            size="8"
            color="#C1C4C9"
          />
        </li>
      </ul>
      <button class="slider-news-main__slider-number-responsive__list--button">
        Tümü
      </button>
    </div>
  </div>
</template>

<style lang="scss" src="./slider-news-main.scss"></style>
