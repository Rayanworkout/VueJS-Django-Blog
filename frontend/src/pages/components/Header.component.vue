
<template>
    <section class="container">
        <header class="py-2 mt-3 mx-auto">
            <div class="text-center">
                <img src="../../assets/monkey-compressed.png" alt="">
                <p class="my-2">Some Dev / DevOps related small tutorials or useful config files with detailed comments.</p>
            </div>
        </header>
    </section>
</template>

<style scoped>
header {
    display: flex;
    justify-content: center;
    align-items: center;
    max-width: 30%;
}

p {
    font-weight: 600;
}

img {
    width: 160px;
    height: 160px;
    border-radius: 100px;
}


@media (max-width: 768px) {
    header {
        max-width: 100%;
    }
}
</style>