<template>
    <div class="info">
        <div>INFO</div>
        <p class="first">Experience a transcendent musical odyssey as Velvet Clouds, the captivating post-rock band renowned for their atmospheric soundscapes, embarks on an unforgettable UK tour. </p>
        <p class="last">Join us between May 4th and May 17th for an immersive journey into the depths of sound and emotion. Velvet Clouds will weave their enchanting melodies, pulsating rhythms, and soaring crescendos, enveloping you in a symphony of ethereal beauty.<br /><br />Step into a world where music transcends boundaries and transports you to realms unknown. Through their latest album and timeless favorites, Velvet Clouds will captivate your senses, evoking powerful emotions and leaving an indelible mark on your soul. </p>
    </div>
</template>

<style scoped>

    .info {
        padding: 4em 15em;
        position: relative;
        max-width: 1500px;
        margin-inline: auto;
    }
    .info p.first {
        font-size: 3rem;
        line-height: 1.1;
    }

    .info p.last {
        font-size: 1.25rem;
        margin-top: 2em;
        line-height: 1.1;
    }

    .info div {
        font-family: 'Codystar', sans-serif;
        font-size: 4rem;
        color: #00FF85;
        position: absolute;
        top: 0;
        transform: rotate(270deg) translate(-70%, -180%) ;
    }

    @media (max-width: 1500px) {
        .info p.first {
            font-size: 2rem;
        }

        .info p.last {
            font-size: 1.125rem;
        }
    }

    @media (max-width: 1200px) {
        .info {
            padding: 4em 10em;
        }
    }
    @media (max-width: 1000px) {
        .info {
            padding: 4em 3em;
        }

        .info div {
            position: relative;
            transform: none;
            font-size: 3.4rem;
        }

        .info p.first {
            font-size: 1.5rem;
        }

        .info p.last {
            font-size: 1rem;
        }
    }
</style>