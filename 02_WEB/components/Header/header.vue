<template>
  <div class="header shadow-md">
    <div class="header__container flex justify-between align-middle px-14">
      <div class="header__left flex gap-4 w-[30%]">
        <UNavigationMenu
          orientation="horizontal"
          :items="itemNavs"
          color="error"
          highlight
          variant="link"
          class="header__menu data-[orientation=vertical]:w-48"
        />
      </div>
      <div class="header__center py-5 w-[40%] text-center">
        <a href="#" class="header__logo">
          <!-- <img src="" alt="Logo" class="header__logo-image" /> -->
          GUNDAM
        </a>
      </div>
      <div class="header__right flex justify-end align-middle gap-4 w-[30%]">
        <div class="header__search py-4">
          <UButton
            icon="i-lucide-search"
            class="rounded-full"
            size="xl"
            color="neutral"
            variant="ghost"
          />
        </div>
        <div class="header__contact flex justify-center py-4">
          <UButton
            icon="ri:question-mark"
            class="rounded-full"
            color="neutral"
            variant="ghost"
          />
        </div>
        <div class="header__avatar py-4">
          <UDropdownMenu
            :items="itemUsers"
            :ui="{
              content: 'w-48',
            }"
            class="cursor-pointer"
          >
            <UAvatar
              v-if="isLogin"
              src="https://github.com/benjamincanac.png"
            />
            <UAvatar v-else icon="si:user-alt-3-line" />
          </UDropdownMenu>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup lang="ts">
  // 1. 🧩 Imports
  import type { NavigationMenuItem, DropdownMenuItem } from "@nuxt/ui";
  // 2. 🌐 Composables

  // 3. 📦 Props & Emits

  // 4. 🧠 Reactive State
  const isLogin = ref<boolean>(true);
  const itemNavs = ref<NavigationMenuItem[][]>([
    [
      {
        label: "Cửa hàng",
        class:
          "font-bold border border-white hover:border-black transition-colors duration-300 cursor-pointer",
        children: [
          {
            label: "High Grade",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Real Grade",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Master Grade",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Perfect Grade",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Super Deformed",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Entry Grade",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Full Mechanics",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Dụng cụ",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Decals",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Sơn",
            description: "",
            icon: "",
            class: "hover:bg-red-200",
          },
        ],
      },
      {
        label: "Mới về",
        class:
          "font-bold border border-white hover:border-black transition-colors duration-300 cursor-pointer",
      },
      {
        label: "Khuyến mãi",
        class:
          "font-bold border border-white hover:border-black transition-colors duration-300 cursor-pointer",
      },
      {
        label: "Trợ giúp",
        class:
          "font-bold border border-white hover:border-black transition-colors duration-300 cursor-pointer",
        children: [
          {
            label: "Hướng dẫn lắp ráp",
            icon: "",
            description: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Chính sách giao hàng",
            icon: "",
            description: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Chính sách đổi trả",
            icon: "",
            description: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Câu hỏi thường gặp (FAQ)",
            icon: "",
            description: "",
            class: "hover:bg-red-200",
          },
          {
            label: "Liên hệ",
            icon: "",
            description: "",
            class: "hover:bg-red-200",
          },
        ],
      },
    ],
  ]);

  const itemUsers = ref<DropdownMenuItem[][]>([
    [
      {
        label: "Benjamin",
        avatar: {
          src: "https://github.com/benjamincanac.png",
        },
        type: "label",
      },
    ],
    [
      {
        label: "Thông tin",
        icon: "i-lucide-user",
      },
      {
        label: "Thanh toán",
        icon: "i-lucide-credit-card",
      },
      {
        label: "Cài đặt",
        icon: "i-lucide-cog",
      },
      {
        label: "Giỏ hàng",
        icon: "i-lucide-shopping-cart",
      },
    ],
    [
      {
        label: "Hỗ trợ",
        icon: "i-lucide-life-buoy"
      }
    ],
    [
      {
        label: "Đăng xuất",
        icon: "i-lucide-log-out",
      },
    ],
  ]);
  // 5. 🧮 Computed Properties
  // 6. 🧾 Methods / Functions
  // 7. 🧯 Lifecycle Hooks
</script>

<style scoped></style>
