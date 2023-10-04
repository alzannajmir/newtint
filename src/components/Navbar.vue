<template>
  <nav class="navbar navbar-expand-lg bg-white">
    <!-- Tambahkan class "bg-white" -->
    <div class="container">
      <a class="navbar-brand" href="#">NewTint</a>
      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNavAltMarkup"
        aria-controls="navbarNavAltMarkup" aria-expanded="false" aria-label="Toggle navigation">
        <span class="navbar-toggler-icon"></span>
      </button>
      <div class="collapse navbar-collapse" id="navbarNavAltMarkup">
        <div class="navbar-nav ms-auto">
          <a class="nav-link" aria-current="page" href="#">Jacket</a>
          <a class="nav-link" href="#">T-shirt</a>
          <a class="nav-link" href="#">Pants</a>
          <a class="nav-link" href="#">Contact</a>
        </div>
      </div>
    </div>
  </nav>
</template>

<style scoped>
@import url("https://fonts.googleapis.com/css2?family=Black+Ops+One&display=swap");
@import url('https://fonts.googleapis.com/css2?family=Koh+Santepheap&display=swap');

.navbar-brand {
  width: 211.397px;
  height: 44px;
  flex-shrink: 0;
  color: #2c2c2c;
  font-family: 'Black Ops One', cursive;
  font-size: 48px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}

.nav-link {
  color: #2c2c2c;
  font-family: 'Koh Santepheap', serif;
  font-size: 20px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
}
</style>
