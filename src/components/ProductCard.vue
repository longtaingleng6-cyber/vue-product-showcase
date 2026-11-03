<script setup>
defineProps({
  product: {
    type: Object,
    required: true,
  },
})

const formatPrice = (value) =>
  new Intl.NumberFormat('en-US', {
    style: 'currency',
    currency: 'USD',
  }).format(value)
</script>

<template>
  <article class="group overflow-hidden rounded-[1.75rem] border border-slate-200 bg-white shadow-sm transition duration-300 hover:-translate-y-1 hover:shadow-xl">
    <div class="relative overflow-hidden">
      <img
        :src="product.image"
        :alt="product.name"
        class="h-56 w-full object-cover transition duration-500 group-hover:scale-105"
      />
      <span class="absolute left-4 top-4 rounded-full bg-white/85 px-2.5 py-1 text-xs font-semibold text-slate-700 shadow-sm">
        New arrival
      </span>
    </div>

    <div class="space-y-5 p-5">
      <div class="flex items-start justify-between gap-3">
        <div>
          <h3 class="text-xl font-bold text-slate-900">{{ product.name }}</h3>
          <p class="mt-1 text-sm text-slate-500">{{ product.category }}</p>
        </div>
        <span class="rounded-full bg-emerald-50 px-2.5 py-1 text-xs font-semibold text-emerald-700">
          {{ product.rating }} ★
        </span>
      </div>

      <p class="text-sm leading-6 text-slate-600">{{ product.description }}</p>

      <div class="flex items-center justify-between gap-4">
        <div>
          <p class="text-2xl font-black text-slate-900">{{ formatPrice(product.price) }}</p>
        </div>

        <button class="rounded-full bg-slate-900 px-4 py-2 text-sm font-semibold text-white transition hover:bg-slate-700">
          Add to cart
        </button>
      </div>
    </div>
  </article>
</template>
