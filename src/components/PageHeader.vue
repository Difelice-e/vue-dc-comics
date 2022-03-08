<template>
  <header class="header">
    <div class="container">
      <picture class="logo">
        <img src="../assets/img/dc-logo.png" alt="logo" />
      </picture>

      <nav class="main-nav">
        <ul>
          <li class="nav__item">
            <a href="#">Characters</a>
          </li>
          <li class="nav__item active">
            <a href="#">Comics</a>
          </li>
          <li class="nav__item">
            <a href="#">Movies</a>
          </li>
          <li class="nav__item">
            <a href="#">Tv</a>
          </li>
          <li class="nav__item">
            <a href="#">Games</a>
          </li>
          <li class="nav__item">
            <a href="#">Collectibles</a>
          </li>
          <li class="nav__item">
            <a href="#">Videos</a>
          </li>
          <li class="nav__item">
            <a href="#">Fans</a>
          </li>
          <li class="nav__item">
            <a href="#">News</a>
          </li>
          <li class="nav__item">
            <a href="#">Shop</a>
          </li>
        </ul>
      </nav>
    </div>
  </header>
</template>

<script>
export default {
  name: "PageHeader",
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