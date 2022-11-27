/* eslint-enable */
<template>
  <header>
    <div class="big-container">
      <div class="container">
        <div class="logo">
          <img class="header-logo"
          src="@/assets/img/dc-logo.png" alt="">
        </div>
        <div class="nav">
          <ul>
            <li
            :class="(link.isActive)? 'active-link' : ''"
            v-for="(link,i) in menuLinks" :key="i"
            >
            <a
            @click="activateLink(i)"
            href="#">{{link.label.toUpperCase()}}</a>
            </li>
          </ul>
        </div>
      </div>

    </div>
    <div class="jumbotron"></div>
  </header>

</template>

<script>
export default {
  name: 'HeaderPage',
  methods: {
    /* eslint-disable */
    activateLink(index) {
      //SETTO TUTTO FALSE
      this.menuLinks.forEach((link) => {
        link.isActive = false;
      });
      //ATTIVO QUELLO CLICKATO
      this.menuLinks[index].isActive = true;
    },



  },
  data() {
    return {

      menuLinks: [
        {
          label: 'characters',
          isActive: false,
          index: 0,
        },
        {
          label: 'comics',
          isActive: true,
        },
        {
          label: 'movies',
          isActive: false,
        },
        {
          label: 'tv',
          isActive: false,
        },
        {
          label: 'games',
          isActive: false,
        },
        {
          label: 'collectibles',
          isActive: false,
        },
        {
          label: 'videos',
          isActive: false,
        },
        {
          label: 'fans',
          isActive: false,
        },
        {
          label: 'news',
          isActive: false,
        },
        {
          label: 'shop',
          isActive: false,
        },
      ],
    };
  },
};
</script>

<style lang="scss">


  .big-container {
    width: 1300px;
    height: 500px;
    margin: 0 auto;


    .container {
      display: flex;
    justify-content: space-between;
    justify-items: center;
    height: 100px;
    }

    .logo {
      width: 100px;

      .header-logo {
        height: 100%;
      }
    }

    .jumbotron {
      height: 250px;
      background-image: url('@/assets/img/jumbotron.jpg');
      width: 100%;
      background-size: cover;
      background-repeat: no-repeat;
    }

    .nav {
      width: 60%;
      height: 100%;

      ul {
        display: flex;
        justify-content: space-between;
        align-items:center;
        height: 100%;

        li {
          height: 100%;
          line-height: 100px;
          list-style: none;
          font-size: 12px;
          font-weight: bolder;

          a {
            text-decoration: none;
          }
          a:visited {
            color: black;
          }

          &.active-link {
            color: rgb(0, 89, 255);
            border-bottom: 5px solid rgb(0, 89, 255);
          }
        }
      }
    }

  }
</style>
