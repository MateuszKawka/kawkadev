<template>
  <header class="header">
    <div>
      <h1 class="header__title">Mateusz Kawka</h1>
      <p class="header__subtitle">Junior Front End <br><span>Developer</span></p>
    </div>

    <button class="cv-download">Download CV</button>
  </header>
</template>

<style lang="scss" scoped>
.header {
    width: 100%;
    height: 100vh;
    display: flex;
    justify-content: space-around;
    align-items: center;
    flex-wrap: wrap;
    background: url("/Header.jpg") center no-repeat;
    background-size: cover;
    padding: 0 5rem;
    color: #fff;
}

.header__title {
    font-size: $font-large;
}

.header__subtitle {
    font-size: $font-large;
}

.cv-download {
    width: 132px;
    height: 132px;
    background: $details;
    color: #fff;
    border: none;
}
</style>