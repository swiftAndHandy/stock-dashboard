<script setup lang="ts">
import BaseCard from '../components/cards/BaseCard.vue';
import CorpCard from '../components/cards/CorpCard.vue';
import DarkCard from '../components/cards/DarkCard.vue';
import PageTitle from '../components/PageTitle.vue';
</script>

<template>
  <PageTitle>The Magnificent Seven Companies</PageTitle>
  <main>
    <DarkCard></DarkCard>
    <BaseCard>
      <h1>Test</h1>
    </BaseCard>
    <CorpCard corpName="Apple"></CorpCard>
  </main>
</template>

<style scoped>
main {
  align-self: center;
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 1920px;
  width: 100%;
  padding: 100px;
}
</style>