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
  
  @import './style/footer.scss';
</style>
