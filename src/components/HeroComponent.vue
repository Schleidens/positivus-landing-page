<script setup lang="ts">
  import Illustration from '../assets/Illustration_hero.svg';
</script>

<template>
  <header>
    <div class="hero">
      <div class="right">
        <h2>Navigating the digital landscape for success</h2>
        <div class="text">
          Our digital marketing agency helps businesses grow and succeed online
          through a range of services including SEO, PPC, social media
          marketing, and content creation.
        </div>
        <a href="">Book a consultation</a>
      </div>
      <div class="left">
        <img
          :src="Illustration"
          alt=""
        />
      </div>
    </div>
  </header>
</template>

<style scoped lang="scss">
  header {
    display: flex;
    justify-content: center;
    align-items: center;

    height: calc(100vh - 134px);

    .hero {
      max-width: 1281px;
      width: 100%;

      display: flex;
      justify-content: space-between;

      padding: 0 1em;

      .right {
        display: flex;
        flex-direction: column;
        gap: 20px;

        h2 {
          font-size: 52px;

          margin: 0;
          padding: 0;
        }

        .text {
          font-size: 20px;
        }

        a {
          font-size: 20;

          width: 264px;

          padding: 20px 35px;

          background-color: #000;
          color: #fff;

          text-align: center;
          text-decoration: none;

          border-radius: 14px;
        }
      }
    }
  }
</style>
