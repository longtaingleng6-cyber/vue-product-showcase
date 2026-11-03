<template>
  <nav class="sticky top-0 z-50 border-b border-slate-200 bg-white/80 backdrop-blur-md">
    <div class="mx-auto flex max-w-7xl items-center justify-between px-6 py-4">
      <div class="flex items-center gap-3">
        <div class="flex h-10 w-10 items-center justify-center rounded-xl bg-slate-900 text-lg font-bold text-white shadow-lg shadow-slate-900/20">
          S
        </div>
        <div>
          <p class="text-lg font-bold tracking-tight text-slate-900">ShopVue</p>
          <p class="text-xs text-slate-500">Curated essentials</p>
        </div>
      </div>

      <div class="hidden items-center gap-8 md:flex">
        <a href="#featured" class="text-sm font-medium text-slate-600 transition hover:text-slate-900">Featured</a>
        <a href="#categories" class="text-sm font-medium text-slate-600 transition hover:text-slate-900">Categories</a>
        <a href="#trending" class="text-sm font-medium text-slate-600 transition hover:text-slate-900">Trending</a>
        <a href="#reviews" class="text-sm font-medium text-slate-600 transition hover:text-slate-900">Reviews</a>
      </div>

      <div class="flex items-center gap-3">
        <button class="hidden rounded-full border border-slate-200 px-4 py-2 text-sm font-medium text-slate-700 transition hover:border-slate-300 hover:bg-slate-50 sm:inline-flex">
          Search
        </button>
        <button class="inline-flex items-center rounded-full bg-slate-900 px-4 py-2 text-sm font-semibold text-white shadow-lg shadow-slate-900/20 transition hover:bg-slate-700">
          Start shopping
        </button>
      </div>
    </div>
  </nav>
</template>
