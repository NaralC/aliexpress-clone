<script setup>
import MainLayout from "~/layouts/main-layout.vue";

const products = [
  {
    id: 1,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/82/300/320",
    price: 9999,
  },
  {
    id: 2,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/83/300/320",
    price: 9999,
  },
  {
    id: 3,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/84/300/320",
    price: 9999,
  },
  {
    id: 4,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/52/300/320",
    price: 9999,
  },
  {
    id: 5,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/5/300/320",
    price: 9999,
  },
  {
    id: 6,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/2/300/320",
    price: 9999,
  },
  {
    id: 7,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/23/300/320",
    price: 9999,
  },
  {
    id: 8,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/24/300/320",
    price: 9999,
  },
  {
    id: 9,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/167/300/320",
    price: 9999,
  },
  {
    id: 10,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/96/300/320",
    price: 9999,
  },
  {
    id: 11,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/223/300/320",
    price: 9999,
  },
  {
    id: 12,
    title: "Title 1",
    description: "kuay",
    url: "https://picsum.photos/id/7/300/320",
    price: 9999,
  },
];
</script>

<template>
  <MainLayout>
    <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2 delay-100 duration-200 transition-all">
      <div
        class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4"
      >
        <div v-if="products" v-for="product in products" :key="product">
          <!-- {{ product }} -->
          <ProductComponent :product="product" />
        </div>
      </div>
    </div>
  </MainLayout>
</template>
