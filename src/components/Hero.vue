<template>
  <div class="Hero position-relative">
    <div>
      <div class="first">New</div>
      <div class="headline2 mx-auto">
        <h4>COLLECTION'S</h4>
        <h1>NewTint Fashion</h1>
        <hr />
        <p>Explore All Apparel</p>
      </div>
      <div>
        <h1 class="second">Tint</h1>
      </div>
    </div>
  </div>
</template>


<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Black+Ops+One&display=swap");
@import url('https://fonts.googleapis.com/css2?family=Alice&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Belgrano&display=swap');

/* * {
  border: 1px #535353 dashed;
} */

.Hero {
  background: #f1f1f1;
  background-image: url('assets/hero.jpg');
  background-size: cover;
  height: 90vh;
  margin-top: 5rem;
}

.first,
.second {
  font-family: 'Black Ops One', cursive;
  font-size: 8.125rem;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.second {
  color: lightgray;
  text-shadow: 2px 2px 3px black;
}

.first {
  color: lightgray;
  text-shadow: 2px 2px 3px black;
  text-align: end;
}

.headline2 {
  width: max-content;
  text-align: center;
  color: whitesmoke;
  text-shadow: 2px 2px 3px black;
}

.headline2 h4 {
  color: whitesmoke;
  font-family: 'Alice', serif;
  font-size: 1.5rem;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.headline2 h1 {
  color: whitesmoke;
  font-family: 'Belgrano', serif;
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
  font-family: 'Belgrano', serif;
  font-size: 1.125rem;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}
</style>
