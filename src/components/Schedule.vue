<template>
    <div class="schedules">
        <div class="wrapper">
            <div class="title">SCHEDULE</div>

            <div class="schedule">
                <p><span>04 MAY</span> - The O2, London</p>
                <button>TICKETS</button>
            </div>
            <div class="schedule">
                <p><span>06 MAY</span> - The O2,  London</p>
                <button>TICKETS</button>
            </div>
            <div class="schedule">
                <p><span>07 MAY</span> - The O2, London</p>
                <button>TICKETS</button>
            </div>
            <div class="schedule">
                <p><span>13 MAY</span> - OVO Hydro, Glasgow</p>
                <button>TICKETS</button>
            </div>
            <div class="schedule">
                <p><span>14 MAY</span> - Resorts World, Birmingham</p>
                <button>TICKETS</button>
            </div>
            <div class="schedule">
                <p><span>16 MAY</span> - AO Arena, Manchester</p>
                <button>TICKETS</button>
            </div>
            <div class="schedule">
                <p><span>17 MAY</span> - AO Arena, Manchester</p>
                <button>TICKETS</button>
            </div>
            
        </div>
    </div>
</template>

<style scoped>

    .schedules {
        padding-right: 10em;
        margin-top: 4em;
        max-width: 1500px;
        margin-inline: auto;
    }

    .schedules .wrapper {
        position: relative;

    }
    .schedules .title {
        font-family: 'Codystar', sans-serif;
        font-size: 4rem;
        color: #00FF85;
        position: absolute;
        transform: rotate(270deg) translate(-43%, 140%) ;
        top: 0;
        right: 100%;
    }

    .schedules .wrapper {
        width: fit-content;
        margin-left: auto;
    }

    .schedule {
        display: flex;
        justify-content: space-between;
        align-items: center;
        background-image: linear-gradient(to right,#818181 60%,rgba(0,0,255,0) 10%);
        background-position: top;
        background-size: 9px 1px;
        background-repeat: repeat-x;
    }

    .schedule p {
        font-size: 1.75rem;
        padding-top: .3em;
        padding-bottom: .3em;
    }

    .schedule p span {
        font-weight: bold;
    }

    .schedule button {
        border: none;
        padding: .6em 2em;
        border-radius: 6px;
    }

    @media (max-width: 900px) {
        .schedules .title {
            position: relative;
            transform: none;
            font-size: 3.5rem;
            right: 0;
        }

        .schedules {
            padding-left: 2em;
            padding-right: 2em;
        }

        .schedules .wrapper {
            margin-left: 0;
            margin-right: 0;
            width: auto;
        }

        .schedule {
            flex-direction: column;
            margin-top: 1em;
            padding: .9em 0;
        }

        .schedule p {
            font-size: 1.3125rem;
        }

        .schedule button {
            width: 100%;
        }
    }
</style>