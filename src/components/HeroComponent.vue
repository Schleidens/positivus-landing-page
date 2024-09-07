<script setup lang="ts">
  import Illustration from '../assets/Illustration_hero.svg';
  import PartnersComponent from './PartnersComponent.vue';
</script>

<template>
  <header>
    <div class="hero">
      <div class="right">
        <h2>Navigating the digital landscape for success</h2>
        <img
          :src="Illustration"
          alt=""
        />
        <div class="text">
          Our digital marketing agency helps businesses grow and succeed online
          through a range of services including SEO, PPC, social media
          marketing, and content creation.
        </div>
        <div class="btn">
          <a href="">Book a consultation</a>
        </div>
      </div>
      <div class="left">
        <img
          :src="Illustration"
          alt=""
        />
      </div>
    </div>
    <PartnersComponent />
  </header>
</template>

<style scoped lang="scss">
  header {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;

    min-height: calc(100vh - 134px);
    height: 100%;

    padding: 0 20px;

    .hero {
      max-width: 1281px;
      width: 100%;

      display: flex;
      justify-content: space-between;

      .right {
        display: flex;
        flex-direction: column;
        gap: 40px;

        width: calc(100% - 531px);

        @media (max-width: 800px) {
          width: 100%;
        }

        h2 {
          font-size: 60px;

          margin: 0;
          padding: 0;

          @media (max-width: 800px) {
            font-size: 40px;
          }
        }

        img {
          max-height: 300px;

          @media (min-width: 800px) {
            display: none;
          }
        }

        .text {
          font-size: 20px;

          text-align: left;

          width: 420px;

          @media (max-width: 800px) {
            width: 100%;
          }
        }

        .btn {
          max-width: 264px;
          width: 100%;
          height: 100%;

          @media (max-width: 800px) {
            max-width: 100%;
            width: 100%;
          }

          a {
            display: block;

            font-size: 20px;

            padding: 20px 35px;

            background-color: #000;
            color: #fff;

            text-align: center;
            text-decoration: none;

            border-radius: 14px;
          }
        }
      }

      .left {
        width: 100%;

        display: flex;
        justify-content: flex-end;

        @media (max-width: 800px) {
          display: none;
        }

        img {
          width: 600.46px;
          height: 515px;

          @media (max-width: 1000px) {
            width: 400.46px;
          }
        }
      }
    }
  }
</style>
