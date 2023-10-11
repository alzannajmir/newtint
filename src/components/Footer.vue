<!-- Footer.vue -->
<template>
  <footer>
    <div class="w-75 mx-auto">
      <img src="/image6.png" alt="gambar6" />
      <div class="content d-flex justify-content-between mt-5 flex-wrap gap-4">
        <div>
          <h3>About Us</h3>
          <p class="lead-about">
            Tinted in Indonesia! Produk yang nyaman untuk dipakai pada negara
            tropis, baik pada musim kemarau maupun musim hujan, tentunya
            menggunakan material yang terbaik di kelasnya, melalui tahapan
            quality control yang teliti, dan diproduksi di konveksi yang
            terpercaya
          </p>
        </div>
        <div>
          <h3>Shop</h3>
          <a class="text-white d-block" href="https://www.tiktok.com/@newtintshop">tiktok.com/NewTint</a>
          <a class="text-white d-block" href="https://shopee.co.id/newtint">shopee.com/NewTint</a>
        </div>
        <div>
          <h3>Contact Us</h3>
          <a>newtint@gmail.com</a>
          <a>+62 837-8236-991</a>
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
@media (max-width: 991.98px) {
  .lead-about {
    display: inline;
  }
}

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
