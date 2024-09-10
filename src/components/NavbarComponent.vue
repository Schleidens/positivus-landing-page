<script setup lang="ts">
  import { ref } from 'vue';
  import Logo from '../assets/logo.svg';

  const isOpen = ref(false);

  const triggerMenu = () => {
    isOpen.value = !isOpen.value;
  };
</script>

<template>
  <navbar class="navbar">
    <div class="main">
      <div class="logo">
        <img
          :src="Logo"
          alt=""
        />
      </div>
      <nav
        class="nav-list"
        :class="isOpen && 'sm-open'"
      >
        <ul>
          <li>About Us</li>
          <li>Services</li>
          <li>Use Cases</li>
          <li>Pricing</li>
          <li>Blog</li>
        </ul>
        <a href="">Request a quote</a>
      </nav>
      <div
        class="hamburger"
        @click="triggerMenu"
      >
        <svg
          xmlns="http://www.w3.org/2000/svg"
          fill="none"
          viewBox="0 0 24 24"
          stroke-width="1.5"
          stroke="currentColor"
          class="size-6"
        >
          <path
            stroke-linecap="round"
            stroke-linejoin="round"
            d="M3.75 6.75h16.5M3.75 12h16.5m-16.5 5.25h16.5"
          />
        </svg>
      </div>
    </div>
  </navbar>
</template>

<style lang="scss" scoped>
  navbar {
    display: flex;
    justify-content: center;
    align-items: center;

    margin: 40px 0;
    padding: 0 20px;

    position: sticky;
    top: 0;

    background-color: #fff;

    .main {
      display: flex;
      justify-content: space-between;
      align-items: center;

      font-size: 20px;

      max-width: 1281px;
      width: 100%;
      height: 68px;

      .logo {
        img {
          height: 36px;
        }
      }

      nav {
        display: flex;
        gap: 40px;

        position: relative;

        z-index: 1;

        @media (max-width: 800px) {
          display: none;

          &.sm-open {
            display: flex !important;
            justify-content: center;
            align-items: center;

            position: fixed;

            height: 100%;
            width: 100%;

            top: 0;
            left: 0;

            background-color: #fff;

            ul {
              display: flex;
              flex-direction: column;
              align-items: flex-start;

              font-size: 11vw;
              font-weight: bolder;

              li {
                text-shadow: -15px 5px #baff668c;
              }
            }
          }
        }

        ul {
          display: flex;
          align-items: center;
          justify-content: center;

          gap: 40px;
          list-style: none;

          margin: 0;
          padding: 0;
        }

        a {
          border: 1px solid black;

          padding: 20px 35px;

          border-radius: 14px;

          color: black;
          text-decoration: none;

          @media (max-width: 900px) {
            display: none;
          }
        }
      }

      .hamburger {
        z-index: 9;
        @media (min-width: 800px) {
          display: none;
        }
        svg {
          height: 45px;
          width: 45px;
        }
      }
    }
  }
</style>
