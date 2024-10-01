<template>
    <div class="product-card">
        <slot name="header"></slot>
        <br>
        <slot name="body"></slot>
        <br>
        <slot name="footer"></slot>
    </div>
</template>

<script setup>
</script>

<style>
.product-card {
    border: 1px solid #ccc;
    border-radius: 8px;
    padding: 16px;
    background-color: #f9f9f9;
    box-shadow: 0 2px 5px rgba(0, 0, 0, 0.1);
}

.product-card h3 {
    margin: 0 0 10px;
    font-size: 1.5em;
}

.product-card h4 {
    margin: 0 0 15px;
    font-size: 1.1em;
}

.product-card button {
    padding: 10px 15px;
    border: none;
    border-radius: 5px;
    background-color: #007bff;
    color: white;
    cursor: pointer;
}

.product-card button:hover {
    background-color: #0056b3;
}
</style>
