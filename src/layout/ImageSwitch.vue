<template>
    <div>
        <div>
            <h1 class="overlay-img"> say something </h1>
            <img src="img/bg/1.jpg" alt="owner">
        </div>
        <nav role="navigation">
            <b-nav justified class="nav-modify">
                <b-nav-item class="align-self-end mx-auto">
                    <img src="/img/services/investor.svg" class="rounded mx-auto d-block" alt="Many homes">
                    <div>Many homes</div>
                </b-nav-item>
                <b-nav-item class="align-self-end mx-auto">
                    <img src="/img/services/landlord.svg" class="rounded mx-auto d-block" alt="a few home">
                    <div>A few homes</div>
                </b-nav-item>
                <b-nav-item class="align-self-end mx-auto">
                    <img src="/img/services/homeowner.svg" class="rounded mx-auto d-block" alt="one home">
                    <div>One home</div>
                </b-nav-item> 
            </b-nav>
        </nav>
    </div>
</template>

<style>

    .nav-modify {
        margin: 0 30% 0 30%; 
    }

    @media screen and (max-width: 991px){
        .nav-modify {
            margin: 0 20% 0 20%;
        }
    }

    @media screen and (max-width: 765px){
        .nav-modify {
            margin: 0;
        }
    }

    .overlay-img {
        position: absolute;
        top: 30%;

    }
</style>

<script>
export default {
    name: 'image-switch',
    data: function() {
        return { 
            img: {
                John: "1.jpg",
                Kevin: "2.jpg",
                Mary: "3.jpg"
            },
        };
    },
    props: {
        ManyHome: {
            type: Boolean,
            default: false
        },

    }
}
</script>


