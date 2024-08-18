<script setup lang="ts">
  import Logo from '../assets/logo.svg';
</script>

<template>
  <navbar class="navbar">
    <div class="logo">
      <img
        :src="Logo"
        alt=""
      />
    </div>
    <nav>
      <ul>
        <li>About Us</li>
        <li>Services</li>
        <li>Use Cases</li>
        <li>Pricing</li>
        <li>Blog</li>
      </ul>
      <a href="">Request a quote</a>
    </nav>
  </navbar>
</template>

<script setup></script>

<style lang="scss" scoped>
  navbar {
    height: 68px;

    display: flex;
    justify-content: space-between;
    align-items: center;

    padding: 33px 50px;

    font-size: 20px;

    .logo {
      img {
        width: 219.54px;
        height: 36px;
      }
    }

    nav {
      display: flex;
      gap: 40px;
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
      }
    }
  }
</style>
