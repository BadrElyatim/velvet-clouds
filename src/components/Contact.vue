<template>
    <div class="contact">
        <div class="title">CONTACT</div>
        <p>Fill out the booking form below to ask any questions, or reach out to us directly at <span>help@velvetclouds.com</span> with any questions or concerns. </p>
        <form @submit.prevent="" action="">
            <div class="input-field">
                <label for="">Full Name</label>
                <input type="text" placeholder="Full Name">
            </div>
            <div class="input-field">
                <label for="">Email</label>
                <input type="text" placeholder="Email">
            </div>
            <div class="input-field">
                <label for="">Phone</label>
                <input type="text" placeholder="Phone">
            </div>
            <div class="input-field">
                <label for="">Message</label>
                <textarea placeholder="Message" name="" id="" cols="30" rows="10"></textarea>
            </div>

            <button type="submit">Submit</button>
        </form>
    </div>
</template>

<style scoped>
    .contact {
        max-width: 1500px;
        margin-inline: auto;
        padding: 4em 15em;
        position: relative;
    }

    .contact .title {
        font-family: 'Codystar', sans-serif;
        font-size: 4rem;
        color: #00FF85;
        position: absolute;
        top: 0;
        transform: rotate(270deg) translate(-60%, -300%) ;
    }

    .contact p {
        font-size: 1.25rem;
        margin-bottom: 2em;
    }

    .contact p span {
        text-decoration: underline;
    }

    .contact form .input-field {
        margin-bottom: 1.1em;
    }
    .contact form label {
        display: block;
        font-size: 0.75rem;
        font-weight: bold;
    }

    .contact form input,
    .contact form textarea {
        background-color: #2F2F2F;
        border: none;
        outline: none;
        width: 100%;
        padding: 1em;
        color: #FFF;
    }

    .contact form textarea {
        resize: none;
    }

    .contact form button[type="submit"] {
        background-color: #00FF85;
        border: none;
        padding: .7em 2.4em;
        border-radius: 6px;
        margin-top: .5em;
        cursor: pointer;
        transition: .5s all ease;
    }

    .contact form button[type="submit"]:hover {
        background-color: #FFF;
    }

    @media (max-width: 1200px) {
        .contact {
            padding: 4em 10em;
        }

        .contact .title {
            position: relative;
            transform: none;
            font-size: 3.4rem;
        }
    }
    @media (max-width: 900px) {
        .contact {
            padding-left: 2em;
            padding-right: 2em;
        }

        .contact p {
            font-size: 1.125rem;
        }

    }
    @media (max-width: 500px) {
        .contact form button[type="submit"] {
            width: 100%;
        }
    }
</style>