<script setup>
    import { ref } from 'vue';
    const isNavbarOpened = ref(false)

    const hamburger = ref(null)
    const cross = ref(null)
    const nav = ref(null)
    const showNavbar = () => {
        nav.value.style.display = 'block'
        document.body.style.overflowY = 'hidden';
    }
    const removeNavbar = () => {
        nav.value.style.display = 'none'
        document.body.style.overflowY = 'visible';
    }
</script>

<template>
    <header>
        <img class="arrow" src="./icons/component1.svg" alt="">
        <img ref="hamburger" @click="showNavbar" class="hamburger" src="./icons/hamburger-menu.svg" alt="">

        <nav ref="nav">
            <img @click="removeNavbar" ref="cross" class="cross" src="./icons/cross.svg" alt="">

           <div>
                <ul class="left">
                    <li>INFO</li>
                    <li>SCHEDULE</li>
                    <li>CONTACT</li>
                </ul>
                <ul class="right">
                    <li><img src="./icons/instagram.svg" alt=""></li>
                    <li><img src="./icons/twitter.svg" alt=""></li>
                    <li><img src="./icons/spotify.svg" alt=""></li>
                </ul>
           </div>
            
        </nav>

        <div class="content">
            <div>
                <p>NIGHT DRIVE</p>
                <h1>UK Tour</h1>
                <p class="location"><span>04 MAY - 17 MAY</span><br />London, Glasgow,<br />Birmingham & Manchester</p>
                <div class="btns">
                    <button>TICKETS</button>
                    <button>MORE INFO</button>
                </div>
                <img class="velvet-clouds" src="./icons/velvet-clouds.png" alt="">
            </div>
        </div>
        <img src="./icons/pattern.svg" alt="" class="top-pattern">

        <img src="./icons/pattern.svg" alt="" class="pattern">
    </header>
</template>

<style scoped>
    header {
        background-image: url('@/assets/header.jpg');
        background-repeat: no-repeat;
        background-size: cover;
        background-position: center;
        height: 100vh;
        position: relative;
        overflow: hidden;
    }

    header .arrow {
        position: absolute;
        left: 50%;
        bottom: 10px;
        transform: translateX(-50%);
    }

    header .hamburger {
        display: none;
        margin-left: auto;
        padding: 1em 2em;
        z-index: 10;
        position: relative;
    }
    header .cross {
        display: none;
        margin-left: auto;
    }

    header img.pattern {
        transform: translate(-15%, 30%) rotate(180deg);
        height: 200px; 
        bottom: 0;
        position: absolute;
    }

    header img.top-pattern {
        transform: translateX(-50%);
        height: 200px;
        top: 0;
        position: absolute;
        left: 55%;

    }

    
    /* Nav bar */
    header nav div {
        display: flex;
        justify-content: space-between;
        align-items: center;
        width: 100%;
        padding: 0 4em;
        height: 10vh;
        display: flex;
        align-items: center;
    }

    header nav ul li {
        display: inline-block;
    }

    header nav ul.left li {
        margin-inline: 1em;
        font-weight: bold;
        font-size: .875rem;
    }
    header nav ul.right li {
        margin-inline: .28em;
    }
    header nav ul.right li img {
        height: 38px;
    }
    /* Content */
    header .content {
        height: 90vh;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }

    header .content div {
        position: relative;
        /* z-index: -1; */
    }

    header .content .velvet-clouds {
        position: absolute;
        top: 0;
        left: 0;
        transform: translate(-50%, -84%);
    }

    header .content p:first-child {
        font-weight: 500;
        font-size: 3.31rem;
    }

    header .content h1 {
        font-size: 10rem;
        font-weight: 400;
        line-height: .8;
        position: relative;
        left: -7.6px;
    }

    header .content p.location {
        font-weight: 400;
        font-size: 1.75rem;
        margin-top: .7em;
        line-height: 1.1;
    }
    header .content p.location span{
        font-weight: bold;
        font-size: 1.75rem;
    }

    header .content .btns {
        margin-top: 2.4em;
    }
    header .content .btns button {
        font-size: .93rem;
        font-weight: bold;
        margin-right: 1em;
        max-width: 158px;
        width: 100%;
        padding-top: .8em;
        padding-bottom: .8em;
        border: none;
        border-radius: 6px;
    }

    header .content .btns button:first-child {
        background-color: #00FF85;
    }





    @media (max-width: 1600px) {
   
   header img.top-pattern {
       height: 150px;
   }
}
@media (max-width: 1400px) {
   header img.pattern {
       width: 100%;
       height: auto;
   }
   header img.top-pattern {
       height: 100px;
   }
}

@media (max-width: 1000px) {
   header .content p:first-child {
       font-size: 2.06rem !important;
   }

   header .content .velvet-clouds {
       transform: translate(-20px, -93%) !important;
   }

   header .content h1 {
       font-size: 6.12rem;
   }
   header .content p.location {
       font-size: 1.4rem;

   }

   header .content .btns button {
       max-width: none;
       margin-top: 1em;
   }
}

@media (max-width: 800px){

   header .hamburger {
       display: block;
   }
   header .cross {
       display: block;
   }
   /* header nav .left,
   header nav .right {
       display: none !important;
   } */
   header nav {
    /* padding: 2em; */
    width: 100%;
    height: 100vh;
    background-color: #1D1D1D;
    padding: 1em 2em;
    display: none;
    position: fixed;
    top: 0;
    z-index: 10;
   }
   header nav div {
    width: 100%;
    height: 100%;
    
    flex-direction: column;
    justify-content: space-around;
    display: flex !important;
   }

   header nav .left {
    margin-bottom: 9em;
   }

   header nav .left li {
    display: block;
    text-align: center;
    margin-bottom: 4em;
   }
}
</style>