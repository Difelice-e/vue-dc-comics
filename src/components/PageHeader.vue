<template>
  <header class="header">
    <div class="container">
      <picture class="logo">
        <img src="../assets/img/dc-logo.png" alt="logo" />
      </picture>

      <nav class="main-nav">
        <ul>
          <li v-for="(item, i) in navLink" :key="i"  class="nav__item" :class="item.active ? 'active' : '' ">
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
          href: '#',
          active: true
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
  padding: 10px 10px;

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
        position: relative;

        &::after {
          position: absolute;
          content: '';
          display: none;
          right: 0;
          left: 0;
          bottom: -53px;
          height: 4px;
          background-color: var(--app-blue);
        }

        &.active {
            color: var(--app-blue);
        }

        &.active::after {
          display: block;
        }

        a {
            text-decoration: none;
            color: currentColor;
            font-weight: 600;
            font-size: 0.75rem;

            &:hover {
              color: var(--app-blue);
            }
        }
      }
    }
  }
}
</style>