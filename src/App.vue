<template>
  <NavBar />
  <HeroSection />

  <main class="mx-auto max-w-7xl px-6 py-16">
    <section id="categories" class="mb-12">
      <div class="mb-6 flex items-center justify-between gap-4">
        <div>
          <p class="text-sm font-semibold uppercase tracking-[0.2em] text-indigo-600">Shop by category</p>
          <h2 class="mt-2 text-3xl font-black text-slate-900">Explore the latest drops</h2>
        </div>
        <a href="#featured" class="hidden text-sm font-semibold text-slate-700 underline-offset-4 hover:underline sm:inline">View all</a>
      </div>

      <div class="grid gap-4 sm:grid-cols-2 lg:grid-cols-4">
        <div class="rounded-2xl border border-slate-200 bg-white p-5 shadow-sm">
          <p class="text-sm text-slate-500">Audio</p>
          <h3 class="mt-2 text-xl font-bold text-slate-900">Immersive sound</h3>
        </div>
        <div class="rounded-2xl border border-slate-200 bg-white p-5 shadow-sm">
          <p class="text-sm text-slate-500">Wearables</p>
          <h3 class="mt-2 text-xl font-bold text-slate-900">Smart living</h3>
        </div>
        <div class="rounded-2xl border border-slate-200 bg-white p-5 shadow-sm">
          <p class="text-sm text-slate-500">Photography</p>
          <h3 class="mt-2 text-xl font-bold text-slate-900">Capture more</h3>
        </div>
        <div class="rounded-2xl border border-slate-200 bg-white p-5 shadow-sm">
          <p class="text-sm text-slate-500">Daily carry</p>
          <h3 class="mt-2 text-xl font-bold text-slate-900">Built for travel</h3>
        </div>
      </div>
    </section>

    <section id="featured" class="pb-8">
      <div class="mb-8 text-center">
        <p class="text-sm font-semibold uppercase tracking-[0.2em] text-indigo-600">Featured Products</p>
        <h2 class="mt-2 text-3xl font-black text-slate-900">Hand-picked favorites</h2>
      </div>

      <div class="grid gap-8 sm:grid-cols-2 lg:grid-cols-3">
        <ProductCard v-for="item in products" :key="item.id" :product="item" />
      </div>
    </section>
  </main>

  <footer class="mt-12 bg-slate-900 py-8 text-center text-slate-300">
    <p>© 2026 ShopVue — Built with Vue 3 & Tailwind CSS</p>
  </footer>
</template>

<script setup>
import { ref } from 'vue'
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import ProductCard from './components/ProductCard.vue'

const products = ref([
  {
    id: 1,
    name: 'Wireless Headphones',
    category: 'Audio',
    rating: 4.9,
    description: 'Premium sound quality with active noise cancellation for distraction-free listening.',
    price: 199.99,
    image: 'https://images.unsplash.com/photo-1546435770-a3e426bf472b?auto=format&fit=crop&w=900&q=80',
  },
  {
    id: 2,
    name: 'Smart Watch',
    category: 'Wearables',
    rating: 4.8,
    description: 'Track your health, get notifications, and stay in motion all day long.',
    price: 149.99,
    image: 'https://images.unsplash.com/photo-1523275335684-37898b6baf30?auto=format&fit=crop&w=900&q=80',
  },
  {
    id: 3,
    name: 'Camera Lens',
    category: 'Photography',
    rating: 5.0,
    description: 'Professional-grade optics that capture detailed shots with rich contrast and clarity.',
    price: 299.99,
    image: 'https://images.unsplash.com/photo-1516035069371-29a1b244cc32?auto=format&fit=crop&w=900&q=80',
  },
  {
    id: 4,
    name: 'Gaming Keyboard',
    category: 'Accessories',
    rating: 4.7,
    description: 'RGB-lit mechanical keys crafted for responsive gameplay and comfortable sessions.',
    price: 89.99,
    image: 'https://images.unsplash.com/photo-1511467687858-23d96c32e4ae?auto=format&fit=crop&w=900&q=80',
  },
  {
    id: 5,
    name: 'Bluetooth Speaker',
    category: 'Audio',
    rating: 4.8,
    description: 'Big bass, punchy sound, and up to 20 hours of battery for every outing.',
    price: 59.99,
    image: 'https://images.unsplash.com/photo-1518444065439-e933c06ce9cd?auto=format&fit=crop&w=900&q=80',
  },
  {
    id: 6,
    name: 'Travel Backpack',
    category: 'Daily carry',
    rating: 4.9,
    description: 'Durable storage, smart compartments, and weather-ready protection for every trip.',
    price: 79.99,
    image: 'https://images.unsplash.com/photo-1521572267360-ee0c2909d518?auto=format&fit=crop&w=900&q=80',
  },
])
</script>
