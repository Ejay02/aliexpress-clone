<template>
  <main-layout>
    <div id="IndexPage" class="mt-4 max-w-[1200px] mx-auto px-2">
      <div
        v-if="products"
        class="grid xl:grid-cols-6 lg:grid-cols-5 md:grid-cols-4 sm:grid-cols-3 grid-cols-2 gap-4"
      >
        <div v-for="product in products" :key="product">
          <ProductComponent :product="product" />
        </div>
      </div>
    </div>
  </main-layout>
</template>

<script setup>
import mainLayout from "../layouts/mainLayout.vue";

const products = [
  {
    id: 1,
    title: "Product 1",
    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    url: "https://picsum.photos/id/7/800/800",
    price: 9.99,
  },
  {
    id: 2,
    title: "Product 2",
    description:
      "Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris.",
    url: "https://picsum.photos/id/71/800/800",
    price: 19.99,
  },
  {
    id: 3,
    title: "Product 3",
    description:
      "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.",
    url: "https://picsum.photos/id/72/800/800",
    price: 14.99,
  },
  {
    id: 4,
    title: "Product 4",
    description:
      "Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
    url: "https://picsum.photos/id/73/800/800",
    price: 29.99,
  },
  {
    id: 5,
    title: "Product 5",
    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    url: "https://picsum.photos/id/74/800/800",
    price: 9.99,
  },
  {
    id: 6,
    title: "Product 6",
    description:
      "Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris.",
    url: "https://picsum.photos/id/75/800/800",
    price: 19.99,
  },
  {
    id: 7,
    title: "Product 7",
    description:
      "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.",
    url: "https://picsum.photos/id/76/800/800",
    price: 14.99,
  },
  {
    id: 8,
    title: "Product 8",
    description:
      "Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
    url: "https://picsum.photos/id/77/800/800",
    price: 29.99,
  },
  {
    id: 9,
    title: "Product 9",
    description: "Lorem ipsum dolor sit amet, consectetur adipiscing elit.",
    url: "https://picsum.photos/id/78/800/800",
    price: 999,
  },
  {
    id: 10,
    title: "Product 10",
    description:
      "Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris.",
    url: "https://picsum.photos/id/79/800/800",
    price: 1999,
  },
];
</script>
