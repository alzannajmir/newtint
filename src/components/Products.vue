<template>

  <div class="container">
    <div class="d-flex justify-content-center gap-5 mt-5 mb-4">
      <a class="nav-link" :class="{ 'active': selectedCategory === 'T-shirt' }" @click="setCategory('T-shirt')"
        href="#T-Sh  irt">T-shirt</a>
      <hr class="divider mt-1" />
      <a class="nav-link" :class="{ 'active': selectedCategory === 'Pants' }" @click="setCategory('Pants')"
        href="#Pants">Pants</a>
      <hr class="divider mt-1" />
      <a class="nav-link" :class="{ 'active': selectedCategory === 'Jacket' }" @click="setCategory('Jacket')"
        href="#Jacket">Jacket</a>
    </div>
    <div class="row">
      <div class="d-flex flex-wrap justify-content-evenly align-items-center flex-wrap mb-2">
        <div class="col-lg-3 col-md-4 col-sm-4 mt-5 my-5" v-for="card in filteredCards" :key="card.id">
          <div class="card-menu">
            <img :src="card.image" class="card-img-top" alt="Card Image">
            <div class="card-text mt-3">
              <p>{{ card.description }}</p>
            </div>
            <div class="price mb-5">
              <p>{{ card.price }}</p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <!-- <div class="d-flex justify-content-center gap-5 mt-5 mb-4">
  <button @click="prevPage" :disabled="currentPage.value === 0">Previous</button>
  <button @click="nextPage" :disabled="currentPage.value === maxPage - 1">Next</button>
</div> -->
  </div>
</template>

<style scoped>

@import url('https://fonts.googleapis.com/css2?family=Koh+Santepheap&display=swap');

.headline{
  color: #2C2C2C;
font-family: 'Koh Santepheap', serif;
font-size: 48px;
font-style: normal;
font-weight: 700;
line-height: normal;
}

.divider {
  background-color: #2c2c2c;
  width: 1px;
  height: 20px;
}
.card-text {
  font-size: 13px;
}

.card-menu {
  box-shadow: 0px 4px 10px rgba(128, 109, 97, 0.5);
  width: 230px;
  height: 328px;
  margin: auto;
}

.price {
  font-size: 13px;
  color: #2C2C2C;
}
.nav-link:hover {
  color: red;
}

/* Media query untuk ukuran layar di bawah laptop atau desktop */
@media screen and (max-width: 1199px) {
  .card-menu {
    width: 180px;
    height: 250px;
    /* Mengurangi lebar card-menu */
  }

  .card-text {
    font-size: 9px;
    /* Mengurangi ukuran font card-text */
  }

  .price {
    font-size: 12px;
    /* Mengurangi ukuran font price */
  }
}

@media screen and (max-width: 991px) {
  .card-menu {
    width: 150px;
    height: 200px;
    /* Mengurangi lebar card-menu lebih lanjut */
  }

  .card-text {
    font-size: 9px;
    /* Mengurangi ukuran font card-text lebih lanjut */
  }

  .price {
    font-size: 10px;
    /* Mengurangi ukuran font price lebih lanjut */
  }
}
</style>


<script setup>
import { ref, computed } from 'vue';

const cards = ref([
  // BAJU 
  {
    id: 1,
    description: 'Kaos Salur Unisex (Grey)',
    image: 'assets/Baju/Produk1.png',
    price: 'Rp.100.000,.',
    category: 'T-shirt',
  },
  {
    id: 2,
    description: 'Kaos Salur Unisex (Blue)',
    image: 'assets/Baju/Produk2.png',
    price: 'Rp.100.000,.',
    category: 'T-shirt',
  },
  {
    id: 3,
    description: 'Kaos Salur Unisex (Black)',
    image: 'assets/Baju/Produk3.png',
    price: 'Rp.100.000,.',
    category: 'T-shirt',
  },
  {
    id: 4,
    description: 'Kaos Salur Unisex (Coksu)',
    image: 'assets/Baju/Produk4.png',
    price: 'Rp.100.000,.',
    category: 'T-shirt',
  },
  {
    id: 5,
    description: 'Rugby Oversize Pria (Navy)',
    image: 'assets/Baju/Produk5.png',
    price: 'Rp.100.000,.',
    category: 'T-shirt',
  },
  {
    id: 6,
    description: 'Rugby Oversize Pria (Army)',
    image: 'assets/Baju/Produk6.png',
    price: 'Rp.100.000,.',
    category: 'T-shirt',
  },
  {
    id: 7,
    description: 'Rugby Oversize Pria (Grey)',
    image: 'assets/Baju/Produk1.png',
    price: 'Rp.100.000,.',
    category: 'T-shirt',
  },
  {
    id: 8,
    description: 'Rugby Oversize Pria (Blue)',
    image: 'assets/Baju/Produk2.png',
    price: 'Rp.100.000,.',
    category: 'T-shirt',
  },
    
  // CELANA 

  {
    id: 1,
    description: 'Celana Boardshort (Grey)',
    image: 'assets/Pants/Produk1.png',
    price: 'Rp.100.000,.',
    category: 'Pants',
  },
  {
    id: 2,
    description: 'Celana Boardshort (Blue)',
    image: 'assets/Pants/Produk2.png',
    price: 'Rp.100.000,.',
    category: 'Pants',
  },
  {
    id: 3,
    description: 'Celana Boardshort (Black)',
    image: 'assets/Pants/Produk3.png',
    price: 'Rp.100.000,.',
    category: 'Pants',
  },
  {
    id: 4,
    description: 'Celana Boardshort (Coksu)',
    image: 'assets/Pants/Produk4.png',
    price: 'Rp.100.000,.',
    category: 'Pants',
  },
  {
    id: 5,
    description: 'Celana Boardshort (Navy)',
    image: 'assets/Pants/Produk5.png',
    price: 'Rp.100.000,.',
    category: 'Pants',
  },
  {
    id: 6,
    description: 'Celana Boardshort (Army)',
    image: 'assets/Pants/Produk6.png',
    price: 'Rp.100.000,.',
    category: 'Pants',
  },
  {
    id: 7,
    description: 'Celana Boardshort (Grey)',
    image: 'assets/Pants/Produk1.png',
    price: 'Rp.100.000,.',
    category: 'Pants',
  },
  {
    id: 8,
    description: 'Celana Boardshort (Blue)',
    image: 'assets/Pants/Produk2.png',
    price: 'Rp.100.000,.',
    category: 'Pants',
  },

  // PANTS 

  {
    id: 1,
    description: 'Jacket Trucker Pria (Grey)',
    image: 'assets/Jacket/Produk1.png',
    price: 'Rp.100.000,.',
    category: 'Jacket',
  },
  {
    id: 2,
    description: 'Jacket Trucker Pria (Blue)',
    image: 'assets/Jacket/Produk2.png',
    price: 'Rp.100.000,.',
    category: 'Jacket',
  },
  {
    id: 3,
    description: 'Jacket Trucker Pria (Black)',
    image: 'assets/Jacket/Produk3.png',
    price: 'Rp.100.000,.',
    category: 'Jacket',
  },
  {
    id: 4,
    description: 'Jacket Trucker Pria (Coksu)',
    image: 'assets/Jacket/Produk4.png',
    price: 'Rp.100.000,.',
    category: 'Jacket',
  },
  {
    id: 5,
    description: 'Jacket Trucker Pria (Navy)',
    image: 'assets/Jacket/Produk5.png',
    price: 'Rp.100.000,.',
    category: 'Jacket',
  },
  {
    id: 6,
    description: 'Jacket Trucker Pria (Army)',
    image: 'assets/Jacket/Produk6.png',
    price: 'Rp.100.000,.',
    category: 'Jacket',
  },
  {
    id: 7,
    description: 'Jacket Trucker Pria (Grey)',
    image: 'assets/Jacket/Produk1.png',
    price: 'Rp.100.000,.',
    category: 'Jacket',
  },
  {
    id: 8,
    description: 'Jacket Trucker Pria (Blue)',
    image: 'assets/Jacket/Produk2.png',
    price: 'Rp.100.000,.',
    category: 'Jacket',
  },
]);

const currentPage = ref(0);
const pageSize = 8;
const selectedCategory = ref('T-shirt');

function setCategory(category) {
  selectedCategory.value = category;
  currentPage.value = 0;
}

const filteredCards = computed(() => {
  return cards.value.filter(card => card.category === selectedCategory.value);
});

// function prevPage() {
//   if (currentPage.value > 0) {
//     currentPage.value--;
//   }
// }

// function nextPage() {
//   const maxPage = Math.ceil(filteredCards.value.length / pageSize);
//   if (currentPage.value < maxPage - 1) {
//     currentPage.value++;
//   }
// }

</script>
