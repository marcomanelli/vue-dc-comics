<template>
  <div id="app">
    <!-- Header -->
    <header>
      <Header/>
    </header>

    <!-- Main -->
    <main>
      <div class="wrapper">
        content
      </div>
    </main>

    <footer>
      <Footer />
    </footer>
  </div>
</template>

<script>
import Header from './components/Header'

import Footer from './components/Footer'

export default {
  name: 'App',
  components: {
    Header,
    Footer,
  }
}
</script>

<style lang="scss">
  @import './style/general.scss';

  .wrapper {
    width: 80%;
    margin: auto;
  }

  header{
    .header-container {
      height: 130px;
      display: flex;
      justify-content: space-between;
      align-items: center;
    }
  }

  main {
    height: 100px;
    background-color: rgb(24, 24, 24);
    color: white;
    display: flex;
    align-items: center;
  }

  footer {
    .links {
      background-color: #0282F9;
      height: 200px;
      .link-box {
        float: left;
        height: 200px;
        width: calc(100%/5);
        display: flex;
        justify-content: center;
        align-items: center;
        color: white;
        text-transform: uppercase;
        img {
          max-height: 80px;
          max-width: 100px;
          margin-right: 10px;
        }
      }
    }

    .footer-list {
      background-image: url(./assets/img/footer-bg.jpg);
      height: 480px;
      padding: 30px 0;
      .footer-list-box {
        float: left;
        margin-right: 50px;
        h3 {
          color: white;
          text-transform: uppercase;
          margin: 30px 0;
        }
        li {
          color: gray;
          margin: 10px 0;
          cursor: pointer;
          transition: 0.1s;
          &:hover {
            color: white;
          }
        }
      }
      .footer-list-right {
        float: right;
        background-image: url(./assets/img/dc-logo-bg.png);
        height: 600px;
        width: 600px;
        background-size: cover;
      }
    }
  }
  
</style>
