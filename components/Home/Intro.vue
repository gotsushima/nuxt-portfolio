<template>
  <div class="space-y-6">
    <NuxtImg
      src="/logo.png"
      alt="logo"
      class="ring-2 border ring-gray-200 border-gray-300 dark:ring-white/10 dark:border-gray-800 hover:ring-4 transition-all duration-300 bg-gray-200 dark:bg-gray-900 rounded-full h-12 w-12 sm:h-16 sm:w-16"
      sizes="48px sm:64px"
      placeholder
      format="webp"
    />
    <h1
      class="text-xl font-bold tracking-tight text-gray-800 dark:text-gray-100"
    >
      フロントエンドエンジニア
    </h1>
    <p class="text-gray-900 dark:text-gray-200">
      現在、Vue / Nuxt
      を使ったフロントエンド開発のスキルアップに力を入れています。<br />
      実務での使用はまだ少ないですが、個人開発も含めて制作事例のリンクを掲載しています。
    </p>
    <p class="text-gray-900 dark:text-gray-200">
      HTML / CSS / JavaScript / WordPress
      でのWebサイトのコーディング・デザインや、LP・バナーなどWEBマーケティングのクリエイティブにおいて7年の実務経験があります。
    </p>
    <p class="text-gray-900 dark:text-gray-200">
      モバイルアプリのUIデザイン、ShopifyでのECサイトの構築・運営、チュートリアル動画制作、の実務経験もあります。
    </p>
    <p class="text-gray-900 dark:text-gray-200">
      ミュージシャンとして海外での活動経験もあり、基本的な英語はできます。<br />
      大阪在住です。
    </p>
  </div>
</template>

<script setup>
useSeoMeta({
  title: "portfolio",
  description: "",
});
</script>
