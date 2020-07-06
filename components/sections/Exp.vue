<template>
  <section class="section" id="exp">
    <h2 class="section__title">Experience</h2>
    <div class="exp-box">
        <div class="exp-box__item">
            <p>11/2019 - 03/2019</p>
            <p class="font-bold">HRTEC</p>
            <p>Gdynia</p>
        </div>
    <div class="box__item box__item--details">
        <p class="font-bold">Junior Front End Developer</p>
        <p>tworzenie własnych modułów w zespole w metodyce SCRUM
tworzenie testów end-to-end w CypressJS
używane technologie i narzędzia:
JavaScript, VueJS, php, phpstorm / webstorm, openproject, git / gitflow</p>
    </div>
    </div>
  </section>
</template>

<style lang="scss" scoped>


.exp-box {
    display: flex;
    justify-content: center;
}

.box__item--details {
    margin-left: $s4;
}

.box__item {
    width: 50%;
}
.font-bold {
    font-weight: 600;
}
</style>