<template>
  <header class="header">
    <div class="header__left">
      <div class="menu-toggle"></div>
      <a
        href="/"
        class="logo d-block  d-lg-none"
      >
        <img
          src="/images/logohotel.png"
          alt="TravelerWP"
        >
      </a>
    </div>
    <div class="header__center"></div>
    <div class="header__right"></div>
  </header>
</template>
<style scoped lang="scss">
.header {
  padding: 0 30px;
  padding-top: 18px;
  padding-bottom: 18px;
  position: relative;
  border-bottom: 1px solid var(--light-grey-color, #eaeef3);
  .header__left {
    display: flex;
    align-items: center;
    .menu-toggle {
      background: url(/images/icon-map.svg) center center no-repeat;
      width: 24px;
      height: 20px;
      margin-right: 10px;
      cursor: pointer;
      display: none;
    }
  }
}

@media screen and (max-width: 991px) {
    .header__left {
        .logo {
            margin-left: 60px;
        }
        .menu-toggle {
            display: block !important;
        }
    }
}
</style>