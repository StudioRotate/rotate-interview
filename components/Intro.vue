<template>
  <section class="Intro">
    <div class="Intro__wrapper">
      <h1 class="Intro__title">
        Rotate° Interview
      </h1>
      <h2 class="Intro__subtitle">Please read the README before you start.</h2>
    </div>
  </section>
</template>

<style>
@font-face {
  font-family: "Brown";
  font-weight: normal;
  font-style: normal;
  src: url("/fonts/lineto-brown-regularwoff2") format("woff2"),
       url("/fonts/lineto-brown-regularwoff") format("woff");
}

@font-face {
  font-family: "Leighton";
  font-weight: normal;
  font-style: normal;
  src: url("/fonts/leighton-light.woff2") format("woff2"),
       url("/fonts/leighton-light.woff") format("woff");
}

.Intro {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.Intro__wrapper {
  max-width: 1600px;
  padding-right: 35px;
  padding-left: 35px;
  margin-right: auto;
  margin-left: auto;
}

.Intro__title,
.Intro__subtitle {
  margin-bottom: 30px;
}

.Intro__title {
  font-family:  "Brown", system-ui;
  font-size: 60px;
  color: #333333;
}

.Intro__subtitle {
  font-family:  "Leighton", system-ui;
  font-size: 14px;
  letter-spacing: 0.0625em;
  line-height: 1.7;
  color: #999999;
}

@media screen and (min-width: 800px) {
  .Intro__container {
    padding-right: 80px;
    padding-left: 80px;
  }

  .Intro__title {
    font-size: 100px;
  }

  .Intro__subtitle {
    font-size: 16px;
    letter-spacing: 0.0625em;
    line-height: 26px;
  }
}
</style>
