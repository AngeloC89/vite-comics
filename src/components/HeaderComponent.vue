<template>
  <header>
    <div id="header" class="container ">
      <!-- Logo -->
      <div class="p-3">
        <img class="img-fluid" src="/public/img/dc-logo.png" alt="">
      </div>
      <!-- navbar -->
      <div id="nav" class="p-3">
        <ul>
          <li v-for="(item, index) in menu" :key="index">
            <a href="#">{{ item }}</a>
          </li>
        </ul>      
      </div>

    </div>
  </header>
</template>

<script>
  export default {
    name: 'HeaderComponent',
    data() {
      return {
        menu: [
          'characters',
          'comics',
          'movies',
          'tv',
          'games',
          'collectibles',
          'videos',
          'fans',
          'news',
          'shop'
        ]

      }
    }
  }

</script>

<style lang="scss" scoped>

  @use '../assets/styles/partials/variables' as *;

  header {

    background-color: $backgroundHeader;
    width: 100%;
    display: flex;
    align-items: center;

    #header {
      display: flex;
      justify-content: space-between;
      align-items: center;

      ul {
        display: flex;
        align-items: center;
        margin: auto;

        li {
          list-style: none;
          margin: 10px;

          a {
            text-decoration: none;
            text-transform: uppercase;
            color: black;
            font-weight: bold;

            &:hover {
              color: #0282f9;
            }

            &:after {
              content: '';
              display: block;
              height: 5px;
              width: 100%;
              margin: 0 auto;             
              background-color: transparent;
              position: relative ;
              top: 53px;
            }
            &.active:after,
            &:hover:after {
              background-color: #0282f9;
            }
          }
        }
      }
    }
  }
</style>
