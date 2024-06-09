<template>
  <div class="navbar-chanel">
    <div class="navbar-chanel__content">
      <div class="navbar-chanel__time">
        <span> 20.04.2024, PERŞEMBE </span>
        <Icon
          class="mx-2"
          name="material-symbols-light:radio-button-unchecked"
          size="9"
          color="#ffffff23"
        />
        <span>15:32</span>
      </div>
      <div class="flex">
        <ul class="navbar-chanel__list">
          <li v-for="(item, index) in chanel">
            <Icon
              v-if="index != 0"
              class="navbar-chanel__list--icon"
              name="material-symbols-light:radio-button-unchecked"
              size="9"
              color="#ffffff23"
            />
            <span>{{ item }}</span>
          </li>
        </ul>
        <div class="navbar-chanel__icon">
          <Icon
            name="material-symbols:arrow-right-alt"
            color="#ffffff3a"
            size="24"
          />
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
const chanel = ref([
  'TVNET',
  'GZT',
  'LOKMA',
  'DERİN TARİH',
  'SKYROAD',
  'Z RAPORU',
  'MECRA',
  'CİNS',
  'NİHAYET',
  'Z RAPORU',
  'MECRA',
  'CİNS',
  'MECRA',
]);
</script>
<style lang="scss" src="./navbar-chanel.scss"></style>
