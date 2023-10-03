<template>
  <div class="Hero position-relative">
    <img class="position-absolute hero-image" src="Hero.png" width="27%">
    <div class="d-flex">
      <div class="w-100">
        <h1 class="first">New</h1>
        <div class="headline2">
          <h4>COLLECTION'S</h4>
          <h1>NewTint Fashion</h1>
          <hr />
          <p>Explore All Apparel</p>
        </div>
      </div>
      <div class="flex-shrink-2 right-side">
        <h1 class="second">Tint</h1>
      </div>
    </div>
  </div>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Black+Ops+One&display=swap");

/* * {
  border: 1px #535353 dashed;
} */

.Hero {
  background: #f1f1f1;
  width: 100%;
  height: 80vh;
}

.hero-image {
  top: 1rem;
  right: 10rem;
}

.right-side {
  background-color: #AAAAAA;
  width: 32.25rem;
  height: 80vh;
}

.first,
.second {
  font-family: Black Ops One;
  font-size: 8.125rem;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.second {
  color: rgba(217, 217, 217, 0.80);
}

.first {
  color: rgba(83, 83, 83, 0.33);
  text-align: end;
}

.headline2 {
  width: max-content;
  text-align: center;
  margin: auto;
}

.headline2 h4 {
  color: #2c2c2c;
  font-family: Alice;
  font-size: 1.5rem;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.headline2 h1 {
  color: #2c2c2c;
  font-family: Belgrano;
  font-size: 3rem;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.headline2 hr {
  background: #2c2c2c;
  height: 0.0625rem;
}

.headline2 span {
  color: #2c2c2c;
  font-family: Belgrano;
  font-size: 1.125rem;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}
</style>
