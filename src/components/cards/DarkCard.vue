<template>
    <div class="card">
        <slot></slot>
    </div>
</template>

<script>
export default {
    name: 'Cards',
}
</script>

<style scoped>
.card {
    background: #023A6233;
    padding: 20px 32px;
    display: flex;
    gap: 20px;
    border-radius: 16px;
}
</style>