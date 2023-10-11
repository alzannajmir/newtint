<template>
    <div class="advantage pt-4 py-2">
        <div class="w-75 mx-auto d-flex flex-wrap justify-content-evenly align">
            <div>
                <img src="/advantage1.png" alt="advantage-1">
                <strong>Quality Material</strong>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
            <div>
                <img src="/advantage2.png" alt="advantage-2">
                <strong>Eye Catching Design</strong>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
            <div>
                <img src="/advantage3.png" alt="advantage-3">
                <strong>Affordable Price</strong>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit.</p>
            </div>
        </div>
    </div>
</template>

<style scoped>
.advantage {
    background-color: #535353;
}

.advantage div div {
    display: flex;
    flex-direction: column;
    width: max-content;
    text-align: center;
    color: #F1F1F1;
}

img {
    width: 5rem;
    align-self: center;
}

strong {
    margin-top: 1.25rem;
    font-size: 1.125rem;
}

p {
    width: 15.625rem;
    font-size: 0.8rem;
}
</style>
