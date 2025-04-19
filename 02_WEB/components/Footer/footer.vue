<template>
  <div class="footer bg-gray-800 text-white pt-6 pb-24 px-16">
    <div class="footer__top flex justify-between py-3">
      <div class="footer__top-left w-[30%]">
        <div class="footer__text">GUNDAM</div>
        <div class="footer__descriptions text-pretty">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla,
          aliquam atque officiis repellendus vitae porro odio in, recusandae cum
          possimus voluptas vel? Quisquam ab alias, ut vel suscipit esse
          exercitationem!
        </div>
      </div>
      <div class="footer__top-right">
        <a href="#" class="footer__logo">
          <!-- <img src="" alt="Logo" class="footer__logo-image" /> -->
          GUNDAM
        </a>
      </div>
    </div>
    <div class="footer__bottom mt-6 flex justify-between">
      <div class="footer__bottom-left w-[20%] flex flex-col gap-3">
        <div class="footer__text">GUNDAM</div>
        <div class="footer__descriptions text-pretty">
          Lorem ipsum dolor sit amet consectetur adipisicing elit. Nulla,
          aliquam atque officiis repellendus vitae porro odio in, recusandae cum
          possimus voluptas vel? Quisquam ab alias, ut vel suscipit esse
          exercitationem!
        </div>
        <div class="footer__email">
          <UInput
            trailing-icon="i-lucide-at-sign"
            placeholder="Điền thông tin email"
            size="xl"
          />
        </div>
      </div>
      <div class="footer__bottom-right flex-auto justify-center align-middle flex gap-20">
        <div class="footer__help flex flex-col gap-2">
          <div class="footer__help-title">Hỗ Trợ</div>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
        </div>
        <div class="footer__shop flex flex-col gap-2">
          <div class="footer__help-title">Cửa hàng</div>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
        </div>
        <div class="footer__company flex flex-col gap-2">
          <div class="footer__help-title">Công ty</div>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
          <ULink class="text-white cursor-pointer" as="button">Link</ULink>
        </div>
      </div>
    </div>
  </div>
</template>

<script lang="ts" setup>
  // 1. 🧩 Imports
  // 2. 🌐 Composables
  // 3. 📦 Props & Emits
  // 4. 🧠 Reactive State
  // 5. 🧮 Computed Properties
  // 6. 🧾 Methods / Functions
  // 7. 🧯 Lifecycle Hooks
</script>

<style></style>
