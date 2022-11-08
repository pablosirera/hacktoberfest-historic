<template>
  <header class="hero">
    <img
      width="1600"
      height="1131"
      class="img"
      src="https://pbs.twimg.com/card_img/1578125703404433408/NY8_MUvz?format=jpg&name=4096x4096"
    />
  </header>
</template>

<style scoped>
.hero {
  position: relative;
  overflow: hidden;
}
@media (min-width: 750px) {
  .hero {
    height: 45vw;
  }
}
.img {
  display: block;
  width: 100%;
  height: auto;
}
.gradient,
.gradient2 {
  background-image: url('/assets/mesh-gradient.jpg');
  background-size: cover;
  pointer-events: none;
  mix-blend-mode: screen;
  width: 100%;
  height: 100%;
  position: absolute;
  top: 0;
  left: 0;
  z-index: 2;
}
.gradient2 {
  mix-blend-mode: multiply;
  background-size: cover;
}
.overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 10;
  display: flex;
  flex-direction: column;
  align-items: center;
  color: white;
  padding-top: 1rem;
}
.title {
  font-weight: 900;
  font-size: var(--f-u6);
  margin-bottom: 0.5rem;
  margin-top: 0;
}
@media (min-width: 750px) {
  .title {
    font-size: var(--f-u12);
  }
}

.subtitle {
  display: block;
  font-weight: 400;
  font-size: var(--f-d6);
  letter-spacing: -0.0625em;
}
</style>
