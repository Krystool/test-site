<template>
  <section>
    <h1>PARTENAIRES</h1>
    <div class="icon-list">
      <a :href="partner.link" class="icon-list-el" v-for="partner in getPartners()" target="_blank">
        <NuxtImg width="70" height="70" :src="partner.icon" alt="" />
        <p>{{ partner.name }}</p>
      </a>
    </div>
  </section>
</template>

<style scoped lang="scss">
.icon-list .icon-list-el img {
  width: 70px;
  height: 70px;
}
</style>