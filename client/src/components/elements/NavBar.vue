<template>
    <header class="fixed top-0 left-0 w-full font-inter bg-stone-900 text-stone-50 py-4 px-6">
        <div class="flex">
            <i @click="toggleMenu" class="fa-solid fa-bars lg:hidden"></i>
        </div>
        <nav class="lg:block transition-all max-h-[999px] overflow-hidden" :class="{'closed-menu': !isMenuOpen}">
            <ul class="flex flex-col justify-center items-center gap-4 py-3 lg:flex-row">
                <li @click="closeMenu">Home</li>
                <li @click="closeMenu">Blog</li>
            </ul>
        </nav>
    </header>
</template>
<script setup lang="ts">
import {ref} from "vue";

const isMenuOpen = ref(false);

function toggleMenu(): void {
    isMenuOpen.value = !isMenuOpen.value;
}

function closeMenu(): void {
    isMenuOpen.value = false;
}
</script>
<style scoped lang="css">
.closed-menu {
    max-height: 0;
}

@media screen(lg) {
    .closed-menu {
        max-height: 999px;
    }
}
</style>