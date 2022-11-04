<template>
    <div class="container">
        <div class="row content mb-3">
            <div class="col-lg order-lg-2 ps-lg-5 ms-lg-5">
                <picture class="ps-lg-5">
                    <source media="(max-width:400px)" :srcset="mobileBG">
                    <source media="(min-width:401px)" :srcset="desktopBG">
                    <img :src="mobileBG" alt="webImage" style='height: 100%; width: 100%; object-fit: contain;'>
                </picture>
            </div>
            <div class="col-lg order-lg-1 text-center text-lg-start pt-5">
                <h1>Make remote work</h1>
                <p class="mt-3 mt-lg-5 px-2 ps-lg-0 pe-lg-5 lead">Get your team in sync, no matter your location.
                    Streamline processes, create team rituals, and watch
                    productivity soar.</p>
                <button class="btn px-4 py-2 px-lg-0 py-lg-0 mt-3 mt-lg-5 mb-lg-5"> Learn more</button>
                <div class="row mt-5 px-2">
                    <div class="col">
                        <img :src="databiz" alt="databiz" style='height: 100%; width: 100%; object-fit: contain;'>
                    </div>
                    <div class="col"> <img :src="audiophile" alt="audiophile" style='height: 100%; width: 100%; object-fit: contain;'></div>
                    <div class="col"> <img :src="meet" alt="meet" style='height: 100%; width: 100%; object-fit: contain;'> </div>
                    <div class="col"><img :src="maker" alt="maker" style='height: 100%; width: 100%; object-fit: contain;'> </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script setup>
import mobileBG from '../assets/images/image-hero-mobile.png'
import desktopBG from '../assets/images/image-hero-desktop.png'
import databiz from '../assets/images/client-databiz.svg'
import audiophile from '../assets/images/client-audiophile.svg'
import meet from '../assets/images/client-meet.svg'
import maker from '../assets/images/client-maker.svg'
</script>

<style  scoped>
h1 {
    font-weight: 700;
    font-size: 5rem;
}

p {
    font-weight: 500;
    color: var(--Medium-Gray);
}

.content {
    padding: 3rem 6rem;
}

.btn {
    background-color: var(--Almost-Black);
    color: var(--Almost-White);
    font-weight: 500;
    border-radius: 13px;
}

.btn:hover {
    background-color: var(--Almost-White);
    color: var(--Almost-Black);
    border: 1px solid var(--Almost-Black);
}

@media only screen and (max-width: 700px) {

    h1 {
        font-size: 3rem;
    }
    .col{
        width: 25%;
    }
}

@media only screen and (max-width: 400px) {
    .col-lg {
        padding: 0rem;
    }

    .content {
        padding: 0;
    }

    h1 {
        font-size: 2.3rem;
    }
}

@media only screen and (min-width: 720px) {
    .btn {
        height: 3.5rem;
        width: 9.5rem;
        font-weight: 500;
        font-size: 1.2rem;
    }
}
</style>