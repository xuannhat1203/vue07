<template>
    <CartChildren>
        <template #header>
            <h3>Thông tin sản phẩm</h3>
        </template>
        <template #body>
            <h4>Lorem ipsum dolor sit amet consectetur adipisicing elit. Pariatur maxime omnis velit sed tempora doloribus vitae sint beatae obcaecati repudiandae?</h4>
        </template>
        <template #footer>
            <button>Xem chi tiết</button>
        </template>
    </CartChildren>
</template>
<script setup>
import CartChildren from './CartChildren.vue';
</script>