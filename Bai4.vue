<template>
  <div class="container mx-auto">
    <h1 class="text-center mb-4">Danh sách sản phẩm</h1>
    <div class="row g-4">
      <!-- Gutter (khoảng cách) giữa các cột -->
      <!-- Sản phẩm 1 -->
      <div class="col-12 col-md-6 col-lg-4">
        <div class="card h-100">
          <!-- h-100 để các thẻ card có chiều cao bằng nhau -->
          <img
            :src="products[0].image"
            alt="Hình ảnh sản phẩm"
            class="card-img-top"
          />
          <div class="card-body d-flex flex-column">
            <h3 class="card-title">{{ products[0].name }}</h3>
            <p class="card-text">{{ products[0].description }}</p>
            <p class="card-text">Giá: {{ products[0].price }} VND</p>
            <button class="btn btn-success mt-auto">Mua ngay</button>
            <!-- mt-auto đẩy nút xuống cuối -->
          </div>
        </div>
      </div>

      <!-- Sản phẩm 2 -->
      <div class="col-12 col-md-6 col-lg-4">
        <div class="card h-100">
          <img
            :src="products[1].image"
            alt="Hình ảnh sản phẩm"
            class="card-img-top"
          />
          <div class="card-body d-flex flex-column">
            <h3 class="card-title">{{ products[1].name }}</h3>
            <p class="card-text">{{ products[1].description }}</p>
            <p class="card-text">Giá: {{ products[1].price }} VND</p>
            <button class="btn btn-success mt-auto">Mua ngay</button>
          </div>
        </div>
      </div>

      <!-- Sản phẩm 3 -->
      <div class="col-12 col-md-6 col-lg-4">
        <div class="card h-100">
          <img
            :src="products[2].image"
            alt="Hình ảnh sản phẩm"
            class="card-img-top"
          />
          <div class="card-body d-flex flex-column">
            <h3 class="card-title">{{ products[2].name }}</h3>
            <p class="card-text">{{ products[2].description }}</p>
            <p class="card-text">Giá: {{ products[2].price }} VND</p>
            <button class="btn btn-success mt-auto">Mua ngay</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
// Dữ liệu sản phẩm
const products = [
  {
    name: 'Mèo',
    description: 'Mèo siêu đẹp',
    price: 5000000000,
    image: 'https://cataas.com/cat/says/Hello',
  },
  {
    name: 'Mèo',
    description: 'Mèo siêu đẹp',
    price: 5000000000,
    image: 'https://cataas.com/cat/says/Hello',
  },
  {
    name: 'Mèo',
    description: 'Mèo siêu đẹp',
    price: 5000000000,
    image: 'https://cataas.com/cat/says/Hello',
  },
]
</script>
