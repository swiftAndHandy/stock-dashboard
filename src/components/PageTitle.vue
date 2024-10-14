<template>
    <section id="page-headline">
        <div class="title-prefix"></div>
        <h1><slot></slot></h1>
    </section>
</template>

<script>
</script>

<style scoped>
#page-headline {
    display: flex;
    align-items: center;
    margin-top: 64px;
    margin-bottom: 48px;
    padding-right: 30px;
    gap: 24px;
    h1 {
        font-size: clamp(2vw, 36px, 4vw);
        font-weight: 500;
    }
}

.title-prefix {
    width: 96px;
    height: 32px;
    border-top-right-radius: 100px;
    border-bottom-right-radius: 100px;
    background: #39DAFF;
}
</style>