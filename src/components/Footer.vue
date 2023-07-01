<template>
    <footer>
        <div class="wrapper">
            <div class="img-wrapper">
                <img src="./icons/velvet-clouds.png" alt="">
                <img src="./icons/XIDE-logo.png" alt="">
            </div>
            <p>Velvet Clouds Night Drive UK Tour website. All rights reserved © 2023. Designed by <span>XIDE</span>.</p>
        </div>
    </footer>
</template>

<style scoped>

    footer {
        padding: 3em 4em .8em;
        background-color: #1D1D1D;
    }
    footer .wrapper .img-wrapper {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }


    footer p {
        text-align: center;
        margin-top: 3em;
        font-size: 0.875rem;
    }

    footer p span {
        font-weight: bold;
        text-decoration: underline;
    }

    @media (max-width: 600px) {
        footer {
            padding: 3em 2em .8em;
        }

        footer .img-wrapper img {
            height: 70px;
        }
    }
</style>