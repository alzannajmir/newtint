<!-- Footer.vue -->
<template>
  <footer>
    <div class="container">
      <img src="image 6.png" alt="" />
      <div class="content d-flex justify-content-between mt-5">
        <div>
          <h3>About Us</h3>
          <p class="lead-about">
            Kami adalah perusahaan yang bergerak di bidang...
          </p>
        </div>
        <div>
          <h3>Shop</h3>
          <p>tiktok.com/NewTint</p>
          <p>shopee.com/NewTint</p>
        </div>
        <div>
          <h3>Contact Us</h3>
          <p>newtint.gmail.com</p>
          <p>+62 837-8236-991</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "Footer",
  // Jika Anda memiliki logika Vue yang perlu ditambahkan, Anda dapat menambahkannya di sini.
};
</script>

<style scoped>
.content {
  justify-content: space-between;
}

.lead-about {
  width: 28.75rem;
}

footer {
  background: #2c2c2c;
  color: #fff;
  padding: 20px 0;
}

footer h3 {
  color: #f1f1f1;
  text-align: justify;
  font-family: Koh Santepheap;
  font-size: 28px;
  font-style: normal;
  font-weight: 700;
  line-height: normal;
}

footer p {
  color: #f1f1f1;
  text-align: justify;
  font-family: Koh Santepheap;
  font-size: 18px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
}
</style>
