<template>
    <div class=" mx-auto my-5 w-75">
        <div class="d-flex flex-wrap justify-content-between align-items-center gap-3">
            <div class="info-1 text-center d-flex flex-column justify-content-center flex-fill">
                <h2 class="text-center">Summer Sale</h2>
                <h1>Discount</h1>
                <div class="discount d-flex justify-content-between align-items-start px-1">
                    <hr>
                    <p class="mt-1">Up to 30%</p>
                    <hr>
                </div>
                <a href="https://shopee.co.id/newtint" class="w-50 mx-auto text-center bg-dark text-white fw-bold">Shop Now</a>
            </div>
            <div class="info-2 d-flex justify-content-end align-items-center flex-fill p-2">
                <div class="text-center">
                    <h3>Summer Sale</h3>
                    <h1>Get 30% Discount</h1>
                    <a href="https://shopee.co.id/newtint" class="px-4 py-2">Get Now</a>
                </div>
                <img class="info2-img" src="/information.png" alt="info">
            </div>
        </div>
    </div>
    <div class=" mx-auto mb-4 w-75">
        <div class="info-3 flex-fill p-2">
            <h1 class="text-center">NewTint</h1>
            <div class="d-flex justify-content-center gap-5">
                <img class="logo3" src="/logo.png" alt="logo">
                <p>Welcome to New Tint Official Store! Ready to Tint Your Days? <br><br> Jam Operasional Toko:
                    Senin-Minggu, <br>
                    09.00 – 19.00 WIB </p>
            </div>
        </div>
    </div>
</template>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Sofia&display=swap');

/* * {
    border: 1px dashed gray;
} */

@media (max-width: 991.98px) {

    .info2-img,
    .logo3 {
        display: none;
    }
}

.info-1,
.info-2,
.info-3 {
    background-color: #D9D9D980;
    height: 15rem;
}

.info-3 p {
    width: fit-content;
}

.info-3 h1 {
    color: #2C2C2C;
    font-family: Black Ops One;
    font-size: 4rem;
    font-weight: 400;
}

.info-2 h3 {
    color: #2C2C2C;
    font-family: Sofia;
    font-size: 1.5rem;
    font-weight: 400;
}

.info-2 h1 {
    color: #2C2C2C;
    font-family: Sanchez;
    font-size: 3rem;
    font-style: italic;
    font-weight: 400;
    line-height: normal;
}

.info-2 button {
    border: #2C2C2C 2px dashed;
    color: #2C2C2C;
    text-align: justify;
    font-family: Koh Santepheap;
    font-size: 1.75rem;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

.info-2 img {
    height: 15rem;
}

.info-1 h2 {
    color: #2C2C2C;
    text-align: justify;
    font-family: Sofia;
    font-size: 2.375rem;
    font-style: normal;
    font-weight: 400;
    line-height: normal;
}

.info-1 h1 {
    color: #2C2C2C;
    text-align: center;
    font-family: Poppins;
    font-size: 3.875rem;
    font-style: normal;
    font-weight: 700;
    line-height: normal;
}

.discount hr {
    border: 1px black dashed;
    width: 5rem;
}

.discount p {
    color: #2C2C2C;
    text-align: justify;
    font-family: Sanchez;
    font-size: 1.125rem;
    font-style: italic;
    font-weight: 400;
    line-height: normal;
}
</style>