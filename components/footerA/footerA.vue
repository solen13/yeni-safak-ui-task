<template>
  <div class="footer">
    <div class="footer__title">
      <h3>YeniŞafak</h3>
    </div>
    <div class="footer__social-icon">
      <nuxt-link to="/">
        <Icon name="ri:twitter-x-fill" size="20"></Icon>
      </nuxt-link>
      <Icon
        class="mx-1"
        name="material-symbols-light:radio-button-unchecked"
        size="6"
        color="#989898"
      />
      <nuxt-link to="/">
        <Icon name="ri:youtube-fill" size="20"></Icon>
      </nuxt-link>
      <Icon
        class="mx-1"
        name="material-symbols-light:radio-button-unchecked"
        size="6"
        color="#989898"
      />
      <nuxt-link to="/">
        <Icon name="mdi:telegram" size="20"></Icon>
      </nuxt-link>
      <Icon
        class="mx-1"
        name="material-symbols-light:radio-button-unchecked"
        size="6"
        color="#989898"
      />
      <nuxt-link to="/">
        <Icon name="ph:instagram-logo" size="20"></Icon>
      </nuxt-link>
      <Icon
        class="mx-1"
        name="material-symbols-light:radio-button-unchecked"
        size="6"
        color="#989898"
      />
      <nuxt-link to="/">
        <Icon name="akar-icons:linkedin-box-fill" size="20"></Icon>
      </nuxt-link>
    </div>
    <div class="footer__categories">
      <div class="footer__categories__content">
        <span v-for="(item, index) in list" :class="{ hiddenlink: index > 18 }">
          <nuxt-link>{{ item }}</nuxt-link>
        </span>
      </div>
      <button>
        <Icon
          name="ic:outline-arrow-drop-down"
          color="#8D8D8D"
          size="22"
        ></Icon>
      </button>
    </div>
    <div class="footer__partner-companies">
      <div class="footer__partner-companies__content">
        <nuxt-link>
          <img src="../../public/gzt.png" alt="" />
        </nuxt-link>
        <nuxt-link>
          <img src="../../public/zraporu.png" alt="" />
        </nuxt-link>
        <nuxt-link>
          <img src="../../public/ketebe.png" alt="" />
        </nuxt-link>
        <nuxt-link>
          <img src="../../public/derintarih.png" alt="" />
        </nuxt-link>
        <nuxt-link>
          <img src="../../public/skyroad.png" alt="" />
        </nuxt-link>
        <nuxt-link>
          <img src="../../public/arkitekt.png" alt="" />
        </nuxt-link>
        <nuxt-link>
          <img src="../../public/postoyku.png" alt="" />
        </nuxt-link>
      </div>
    </div>
    <div class="footer__info">
      <div class="footer__info__left">
        <div class="footer__info__left--top">
          <span>Kurumsal</span>
          <Icon
            class="mx-1"
            name="material-symbols-light:radio-button-unchecked"
            size="6"
            color="#989898"
          />
          <span>İletişim</span>
          <Icon
            class="mx-1"
            name="material-symbols-light:radio-button-unchecked"
            size="6"
            color="#989898"
          />
          <span>RRS</span>
        </div>
        <div class="footer__info__left--text">
          <h3>Yasal uyarı</h3>
          <p>
            BIST isim ve logosu "Koruma Marka Belgesi" altında korunmakta olup
            izinsiz kullanılamaz, iktibas edilemez, değiştirilemez. BIST ismi
            altında açıklanan tüm bilgilerin telif hakları tamamen BIST'e ait
            olup, tekrar yayınlanamaz. Piyasa verileri iDealdata Finansal
            Teknolojiler A.Ş. tarafından sağlanmaktadır. BİST hisse verileri 15
            dakika gecikmelidir.
          </p>
        </div>
      </div>
      <div class="footer__info__right">
        <button>
          <Icon class="mr-2" name="ic:baseline-apple" size="27" /> App Store’dan
          indirin
        </button>
        <button>
          <Icon
            class="mr-2"
            name="teenyicons:google-play-store-solid"
            size="27"
          />Google Play’dan alın
        </button>
        <button>
          <Icon class="mr-2" name="cbi:huawei" size="27" />App Galeri ile
          keşfedin
        </button>
      </div>
    </div>
    <div class="footer__contack">
      <span>
        <Icon name="material-symbols:location-on-outline" size="24" />
        Maltepe Mah. Fetih Cad. No:6 34010 Zeytinburnu İstanbul, Türkiye
      </span>
      <div>
        <nuxt-link to="/">
          <Icon name="material-symbols:mail-outline" size="24" />
          iletisim@yenisafak.com.tr
        </nuxt-link>
        <nuxt-link to="/">
          <Icon name="arcticons:bip" size="24" /> +90 530 846 00 00
        </nuxt-link>
        <nuxt-link to="/">
          <Icon name="material-symbols:call" size="24" /> +90 212 467 65 15
        </nuxt-link>
      </div>
    </div>
  </div>
</template>
<style lang="scss" src="./footerA.scss"></style>

<script setup>
const list = ref([
  'Bugün',
  'Gündem',
  'Video',
  'Galari',
  'Son Dakika',
  'Haberler',
  'Dünya',
  'Ekonomi',
  'Spor',
  'Spor Haberleri',
  'Seçim',
  'Yazarlar',
  'Hayat',
  'Hava Durumu',
  'Özgün',
  'Dini Bilgiler',
  'Namaz vakitleri',
  'Ramazan',
]);
</script>
