<template>
  <div class="navbar-setting">
    <div class="navbar-setting__right">
      <button class="navbar-setting__right--menu-button">
        <Icon name="ic:baseline-menu" size="19" />
      </button>
      <nuxt-link class="navbar-setting__right--site-name" to="/"
        >YeniŞafak</nuxt-link
      >
      <div class="navbar-setting__right--lang lang__list">
        <span class="lang__list__edisyon">EDİSYON :</span>
        <ul class="lang__list__flag-list">
          <li
            class="lang__list__flag-list--content"
            v-for="(item, index) in flag"
            :class="{ active: index === 0 }"
          >
            <img
              class="lang__list__flag-list--content--flag-image"
              :src="item.flagImage"
              alt=""
            />
            <span class="lang__list__flag-list--content--flag-name">{{
              item.name
            }}</span>
          </li>
        </ul>
      </div>
    </div>
    <div class="navbar-setting__left">
      <div class="lang__list__flag-list__content-responsive">
        <img
          class="lang__list__flag-list__content-responsive--flag-image"
          src="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAARMAAAC3CAMAAAAGjUrGAAAAjVBMVEXjChf////iAAD0u7zjABHjAA7jBRTjAAviAAXoVVn40NHwnZ/97/DvkJL74+TxpKbmNjzuiYzkJCz40tP+9vbyqqz63+D0trjtf4L86urmPkTkGSPsdnn52NnnTFHqZmrzsbPpXGD2xcbseX3rcXTlLzbmO0HwlpnnRkzujI7pYGT3yMrkFiDpWV3kISlKFajKAAAEG0lEQVR4nO3d23qiMBQFYNhGwCNKtdZDrVp7sq3v/3gTxNZ2skGxUUJY/50z83XiKoQdEoLjAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADAtXjCj9W9ohtiBEGxoDdfbpaNyXT3qV50owrkye+/nQ2bY/dgcD/qv8o/F0U3rhDyi69rbZfV7EREVTuR5Cmzfufz2Ot2BPlFN/OKBDlhZiCJ1ZyCopt6JR5NRyckErv/rEaHS7Q4MZFdKhP7+xVBdzkSiY2Iim70ZdH2Pmck0oPVhwrNTgphMPj9uWZvryKodiSMZvg4dygxWbdWX+XLOLL0/PH9blYe3VZcv5K/P0+8evwp6t8kf/tpZSgUDTISGfbYcY6s7eqd3dHyaGEo1MvoP/oZAz85Ktrcyn/0Zl0oWZG8HbvaBrSR48SOZaH4UWoiJ9UfAXVc986qUESQ1pcMGicWH7S9dTc2hUK3KZHcnF6kCgrdnj0jZUob84W5KlRau9ZUtPK78PJ2ENRoWnL2iI+USGa5vyDNLelnKWXYd04VFkym+ht4ffTIR/Jy1m/cinvXHvGR1Ow4Cc5CQzaSsZZIRCkPG+Hwh0mk444ILZwyXptTbr7qGdDR6qaEZ6Dns5F09XwVqrn98oVCLTaTVz01enzfrnzlPrFjv3dNv9w4k3bZyv3ggT1MeppuOe/u75btok4rLhJtg5bknve6XKHw9dqnri5gPw8w/b9KEQZPk/GnTltbg/eZ/L6K1Ymi1sLYUPjipKU7Ezf8/okykF6r67qesR0vjblMdPWwh0zcxi4Un2gS7v5Lc2eDPHHZU+eQyYA8Gch8uJ83HBobSUp3MrpAJvJS1lh8l0KaquSL4ItYjRN6P+aff9aGW4Nn3Pnq5Enf+J6fk89/S/OK+BkMfS322PkAs+tadrCj62SPF9fOmIUKho9/2CpWy/gvDuSuyf1499nocbJX59r898tOXLl/LUtRGL76QDxxjQ7/1mgZyLSTvibO9Ptu9Weu1X+q7D2KXtKmnmMDszsTmcmEa/Z50zoJb5q9Ht381Rg4TlToT1S47jBQn6hQx6ow3lFhXKwq7P6JwasNcJ9NhfuxDNy3V2F+R4V5QAY/X7ys8nwx1hUwsP6EgXVKKqxnU2HdIwPrY1Vp66ifKryO2iF+p5Mqr7fHcxkcPL/DwHNeKjwPyMBzoww8X8zAc+gqwY8F3SrvV+D425RM4kKlmvtaaNn/xPTp8fywTw7j+H5KTAdq935Ksk8JsO+WItf+bEEl9mdzsI8fi6bY71GBfUE5OfePfbb8IElgn2FOvB91VrGyt5pXapduD/uWc7C/PSd5D0L46z0I7Uq/ByGRvC+DevPlctmYfFT+fRkHeK8KAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIBd/gGdWzmvdW3tugAAAABJRU5ErkJggg=="
          alt=""
        />
        <span class="lang__list__flag-list__content-responsive--flag-name">
          <span class="lang__list__flag-list__content-responsive--edisyon"
            >Edisyon</span
          >
          <span class="lang__list__flag-list__content-responsive--contry"
            >TR <Icon name="ep:caret-bottom" size="10" />
          </span>
        </span>
      </div>

      <div class="navbar-setting__left__content">
        <button>
          <Icon name="ic:baseline-search" size="24" color="white" />
        </button>
        <Icon
          class="mx-2"
          name="material-symbols-light:radio-button-unchecked"
          size="9"
          color="#ffffff23"
        />
        <button>
          <Icon
            name="ic:baseline-notifications-active"
            size="24"
            color="white"
          />
        </button>
        <Icon
          class="mx-2"
          name="material-symbols-light:radio-button-unchecked"
          size="9"
          color="#ffffff23"
        />
        <button>
          <Icon name="mingcute:settings-6-line" size="24" color="white" />
        </button>
        <Icon
          class="mx-2"
          name="material-symbols-light:radio-button-unchecked"
          size="9"
          color="#ffffff23"
        />
        <button>
          <Icon name="solar:user-circle-line-duotone" size="24" color="white" />
          Giriş yapın
        </button>
      </div>

      <button class="navbar-setting__left--responsive-user">
        <Icon name="solar:user-circle-line-duotone" size="24" color="white" />
      </button>
    </div>
  </div>
</template>
<style lang="scss" src="./navbar-setting.scss"></style>
<script setup>
const flag = ref([
  {
    flagImage:
      'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAARMAAAC3CAMAAAAGjUrGAAAAjVBMVEXjChf////iAAD0u7zjABHjAA7jBRTjAAviAAXoVVn40NHwnZ/97/DvkJL74+TxpKbmNjzuiYzkJCz40tP+9vbyqqz63+D0trjtf4L86urmPkTkGSPsdnn52NnnTFHqZmrzsbPpXGD2xcbseX3rcXTlLzbmO0HwlpnnRkzujI7pYGT3yMrkFiDpWV3kISlKFajKAAAEG0lEQVR4nO3d23qiMBQFYNhGwCNKtdZDrVp7sq3v/3gTxNZ2skGxUUJY/50z83XiKoQdEoLjAAAAAAAAAAAAAAAAAAAAAAAAAAAAAADAtXjCj9W9ohtiBEGxoDdfbpaNyXT3qV50owrkye+/nQ2bY/dgcD/qv8o/F0U3rhDyi69rbZfV7EREVTuR5Cmzfufz2Ot2BPlFN/OKBDlhZiCJ1ZyCopt6JR5NRyckErv/rEaHS7Q4MZFdKhP7+xVBdzkSiY2Iim70ZdH2Pmck0oPVhwrNTgphMPj9uWZvryKodiSMZvg4dygxWbdWX+XLOLL0/PH9blYe3VZcv5K/P0+8evwp6t8kf/tpZSgUDTISGfbYcY6s7eqd3dHyaGEo1MvoP/oZAz85Ktrcyn/0Zl0oWZG8HbvaBrSR48SOZaH4UWoiJ9UfAXVc986qUESQ1pcMGicWH7S9dTc2hUK3KZHcnF6kCgrdnj0jZUob84W5KlRau9ZUtPK78PJ2ENRoWnL2iI+USGa5vyDNLelnKWXYd04VFkym+ht4ffTIR/Jy1m/cinvXHvGR1Ow4Cc5CQzaSsZZIRCkPG+Hwh0mk444ILZwyXptTbr7qGdDR6qaEZ6Dns5F09XwVqrn98oVCLTaTVz01enzfrnzlPrFjv3dNv9w4k3bZyv3ggT1MeppuOe/u75btok4rLhJtg5bknve6XKHw9dqnri5gPw8w/b9KEQZPk/GnTltbg/eZ/L6K1Ymi1sLYUPjipKU7Ezf8/okykF6r67qesR0vjblMdPWwh0zcxi4Un2gS7v5Lc2eDPHHZU+eQyYA8Gch8uJ83HBobSUp3MrpAJvJS1lh8l0KaquSL4ItYjRN6P+aff9aGW4Nn3Pnq5Enf+J6fk89/S/OK+BkMfS322PkAs+tadrCj62SPF9fOmIUKho9/2CpWy/gvDuSuyf1499nocbJX59r898tOXLl/LUtRGL76QDxxjQ7/1mgZyLSTvibO9Ptu9Weu1X+q7D2KXtKmnmMDszsTmcmEa/Z50zoJb5q9Ht381Rg4TlToT1S47jBQn6hQx6ow3lFhXKwq7P6JwasNcJ9NhfuxDNy3V2F+R4V5QAY/X7ys8nwx1hUwsP6EgXVKKqxnU2HdIwPrY1Vp66ifKryO2iF+p5Mqr7fHcxkcPL/DwHNeKjwPyMBzoww8X8zAc+gqwY8F3SrvV+D425RM4kKlmvtaaNn/xPTp8fywTw7j+H5KTAdq935Ksk8JsO+WItf+bEEl9mdzsI8fi6bY71GBfUE5OfePfbb8IElgn2FOvB91VrGyt5pXapduD/uWc7C/PSd5D0L46z0I7Uq/ByGRvC+DevPlctmYfFT+fRkHeK8KAAAAAAAAAAAAAAAAAAAAAAAAAAAAAIBd/gGdWzmvdW3tugAAAABJRU5ErkJggg==',
    name: 'TR',
  },
  {
    flagImage:
      'data:image/png;base64,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',
    name: 'EN',
  },
  {
    flagImage:
      'data:image/png;base64,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',
    name: 'AR',
  },
  {
    flagImage:
      'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAARMAAAC3CAMAAAAGjUrGAAAAFVBMVEX///8AI5XtKTkAFZJ2frnzgYftHTARpUz/AAAA/klEQVR4nO3QSQ0AIAADsHH6l4yKPUhaCc2oWTs9586aOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHixIkTJ06cOHHy4ckD5KrN4eD2boIAAAAASUVORK5CYII=',
    name: 'FR',
  },
  {
    flagImage:
      'data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAARMAAAC3CAMAAAAGjUrGAAAAD1BMVEX///8AOabVKx4ALaTWKxfsyKzRAAAA9UlEQVR4nO3QsQGAMAzAsBT4/2b2eOwqnaAZAAAAAAAAAAAAAAAAAAAAAK69bHPYnJSTclJOykk5KSflpJyUk3JSTspJOSkn5aSclJNyUk7KSTkpJ+WknJSTclJOykk5KSflpJyUk3JSTspJOSkn5aSclJNyUk7KSTkpJ+WknJSTclJOykk5KSflpJyUk3JS87HNw+aknJSTclJOykk5KSflpJyUk3JSTspJOSkn5aSclJNyUk7KSTkpJ+WknJSTclJOykk5KSflpJyUk3JSTspJOSkn5aSclJNyUk7KSTkpJ+WknJSTclJOykk5KSflpJyUk/oBg6TI4mvpq6EAAAAASUVORK5CYII=',
    name: 'RU',
  },
  {
    flagImage:
      'data:image/png;base64,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',
    name: 'UR',
  },
]);
</script>
