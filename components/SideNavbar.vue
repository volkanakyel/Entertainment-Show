<template>
  <div class="side-navbar">
    <div class="side-navbar__container">
      <div class="side-navbar__nav-items">
        <img class="side-navbar__logo" src="/img/logo.svg" alt="" />
        <img class="side-navbar__nav-icon" src="/img/menu-icon.svg" alt="" />
        <img class="side-navbar__nav-icon" src="/img/movie-icon.svg" alt="" />
        <img class="side-navbar__nav-icon" src="/img/series-icon.svg" alt="" />
        <img class="side-navbar__nav-icon" src="/img/save-icon.svg" alt="" />
      </div>
      <div class="side-navbar__avatar">
        <img src="/img/avatar.svg" alt="" />
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup></script>

<style scoped lang="scss">
.side-navbar {
  margin: 32px;
  top: 0;
  padding: 32px 24px;
  border-radius: 20px;
  background-color: $semi-dark-blue;
  height: 85vh;
  max-height: 960px;
  @media (max-width: 800px) {
    height: auto;
  }
  @media (max-width: 450px) {
    margin: 0;
    border-radius: 0;
  }
  &__logo {
    width: 32px;
    height: 25px;
    cursor: pointer;
  }
  &__container {
    height: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    @media (max-width: 800px) {
      flex-direction: row;
    }
  }
  &__nav-icon {
    width: 20px;
    height: 20px;
    cursor: pointer;
    &:hover {
      fill: #ffff;
    }
  }
  &__nav-items {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 40px;
    @media (max-width: 800px) {
      flex-direction: row;
      gap: 24px;
    }
  }
}
</style>
