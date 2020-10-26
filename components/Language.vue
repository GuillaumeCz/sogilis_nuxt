<template>
  <div class="lang_selector">
    <div v-if="isFrench">
      <img src="/img/flag_eng.png">
      <nuxt-link :to="switchLocalePath('en')">
        English
      </nuxt-link>
    </div>
    <div v-else>
      <img src="/img/flag_fr.png">
      <nuxt-link :to="switchLocalePath('fr')">
        Français
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
name: "Language",
  computed: {
    isFrench() {
      return this.$i18n.locale === 'fr';
    }
  }
}
</script>
