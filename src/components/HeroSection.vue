<template>
  <section class="overflow-hidden bg-gradient-to-br from-slate-900 via-slate-800 to-indigo-900 text-white">
    <div class="mx-auto grid max-w-7xl items-center gap-12 px-6 py-20 lg:grid-cols-[1.1fr_0.9fr] lg:py-24">
      <div class="space-y-8">
        <span class="inline-flex items-center rounded-full border border-white/15 bg-white/5 px-3 py-1 text-xs font-semibold uppercase tracking-[0.2em] text-indigo-100">
          New season arrivals
        </span>

        <div class="space-y-5">
          <h1 class="max-w-xl text-4xl font-black leading-tight tracking-tight sm:text-5xl lg:text-6xl">
            Upgrade your setup with smarter essentials.
          </h1>
          <p class="max-w-lg text-lg text-slate-200">
            From immersive audio to everyday carry gear, discover the products that make work, play, and travel feel better.
          </p>
        </div>

        <div class="flex flex-wrap items-center gap-4">
          <button class="rounded-full bg-white px-6 py-3 text-sm font-semibold text-slate-900 transition hover:bg-slate-100">
            Shop now
          </button>
          <button class="rounded-full border border-white/20 bg-white/5 px-6 py-3 text-sm font-semibold text-white transition hover:bg-white/10">
            Explore deals
          </button>
        </div>

        <div class="grid max-w-lg grid-cols-3 gap-4 pt-4 text-left">
          <div>
            <p class="text-2xl font-bold text-white">4.9/5</p>
            <p class="text-sm text-slate-300">Average rating</p>
          </div>
          <div>
            <p class="text-2xl font-bold text-white">12k+</p>
            <p class="text-sm text-slate-300">Happy buyers</p>
          </div>
          <div>
            <p class="text-2xl font-bold text-white">48h</p>
            <p class="text-sm text-slate-300">Fast shipping</p>
          </div>
        </div>
      </div>

      <div class="relative">
        <div class="absolute -left-10 top-10 h-40 w-40 rounded-full bg-indigo-500/40 blur-3xl"></div>
        <div class="absolute -right-10 bottom-8 h-52 w-52 rounded-full bg-cyan-400/30 blur-3xl"></div>

        <div class="relative overflow-hidden rounded-[2rem] border border-white/10 bg-white/5 p-4 shadow-2xl shadow-slate-950/40 backdrop-blur-sm">
          <div class="rounded-[1.5rem] bg-gradient-to-br from-white/10 via-slate-200/10 to-transparent p-4">
            <div class="mb-5 flex items-center justify-between">
              <span class="rounded-full bg-emerald-400/20 px-2.5 py-1 text-xs font-semibold text-emerald-200">Best seller</span>
              <span class="text-sm text-slate-200">Free shipping</span>
            </div>

            <div class="grid gap-4 sm:grid-cols-[1.3fr_0.7fr]">
              <div class="overflow-hidden rounded-2xl bg-slate-200/10 p-3">
                <img
                  src="https://images.unsplash.com/photo-1546435770-a3e426bf472b?auto=format&fit=crop&w=900&q=80"
                  alt="Featured audio device"
                  class="h-64 w-full rounded-xl object-cover"
                />
              </div>

              <div class="space-y-4 rounded-2xl bg-slate-950/40 p-4">
                <div>
                  <p class="text-xs uppercase tracking-[0.2em] text-slate-400">Featured</p>
                  <h2 class="mt-2 text-2xl font-bold text-white">Aero Pro</h2>
                </div>

                <div class="space-y-2 text-sm text-slate-200">
                  <p>Adaptive sound</p>
                  <p>40-hour battery</p>
                  <p>Crystal-clear calls</p>
                </div>

                <div class="flex items-end justify-between gap-4">
                  <div>
                    <p class="text-3xl font-black text-white">$199</p>
                  </div>
                  <button class="rounded-full bg-indigo-500 px-3 py-2 text-sm font-semibold text-white transition hover:bg-indigo-400">
                    Add
                  </button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>
