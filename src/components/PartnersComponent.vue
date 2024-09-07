<template>
  <section class="partners">
    <div class="partners__logos">
      <img
        src="../assets//partners/Company logo.svg"
        alt=""
      />
      <img
        src="../assets//partners/Company logo-1.svg"
        alt=""
      />
      <img
        src="../assets//partners/Company logo-2.svg"
        alt=""
      />
      <img
        src="../assets//partners/Company logo-3.svg"
        alt=""
      />
      <img
        src="../assets//partners/Company logo-4.svg"
        alt=""
      />
      <img
        src="../assets//partners/Company logo-5.svg"
        alt=""
      />
    </div>
  </section>
</template>

<script setup lang="ts"></script>

<style scoped>
  section.partners {
    display: flex;
    justify-content: center;
    align-items: center;

    width: 100%;

    .partners__logos {
      max-width: 1281px;
      width: 100%;

      display: flex;
      flex-wrap: nowrap;
      justify-content: space-between;

      @media (max-width: 800px) {
        flex-wrap: wrap;
      }
    }
  }
</style>
