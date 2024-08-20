<script setup lang="ts">
  import Logo from '../assets/logo.svg';
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
    </div>
  </navbar>
</template>

<style lang="scss" scoped>
  navbar {
    display: flex;
    justify-content: center;
    align-items: center;

    margin: 40px 0;

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
  }
</style>
