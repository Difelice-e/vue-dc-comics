<template>
  <header class="header">
    <div class="container">
      <picture class="logo">
        <img src="../assets/img/dc-logo.png" alt="logo" />
      </picture>

      <nav class="main-nav">
        <ul>
          <li v-for="(item, i) in navLink" :key="i"  class="nav__item">
            <a :href="item.href">{{ item.id }}</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "PageHeader",
  data() {
    return {
      navLink: [
        {
          id: 'Characters',
          href: '#'
        },
        {
          id: 'Comics',
          href: '#'
        },
        {
          id: 'Movies',
          href: '#'
        },
        {
          id: 'Tv',
          href: '#'
        },
        {
          id: 'Games',
          href: '#'
        },
        {
          id: 'Collectibles',
          href: '#'
        },
        {
          id: 'Videos',
          href: '#'
        },
        {
          id: 'Fans',
          href: '#'
        },
        {
          id: 'News',
          href: '#'
        },
        {
          id: 'Shop',
          href: '#'
        },
      ]
    }
  }
};
</script>

<style lang="scss" scoped>
.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  gap: 10px;
  padding: 30px 10px;

  .logo {
      width: 100px;

      img {
          width: 100%;
      }
  }

  .main-nav {
    display: flex;
    gap: 20px;

    ul {
      display: contents;
      list-style: none;

      .nav__item {
        text-transform: uppercase;
        white-space: nowrap;

        &.active {
            color: blue;
        }

        a {
            text-decoration: none;
            color: currentColor;
            font-weight: 600;
            font-size: 0.7rem;
        }
      }
    }
  }
}
</style>