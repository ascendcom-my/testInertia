<template>
    <layout>
        <div id="bg-video" class="w-full h-full bg-contain bg-no-repeat bg-center bg-neutral-800">
            <div id="model" class="absolute right-1/2 flex flex-col items-center w-40">
                
                <div id="personImg" class="w-20"></div>
                <div id="cardNameImg" class="w-full h-6"></div>
                
            </div>
            <!-- <div class="cardName-container">
                <img id="cardNameImg" class="h-6 w-36">
            </div> -->
        </div>
    </layout>
</template>

<style>

    #bg-video{
        background-image: url("/images/bg1.gif");
        
    }

    #personImg{
        content: url("/images/person1.jpg");
        /* animation: flow 10s linear; */
    }

    #cardNameImg{
        content:url("/images/card.Png");
        /* animation: flow 10000s linear infinite; */
        
    }

    #model{
        animation: flow 10s linear;
    }

    @keyframes flow {
        0% {
            transform: scale(0);
            opacity: 0;
            bottom: 100%;
        }

        25% {
            transform: scale(0.25);
            opacity: 0.25;
            bottom: 75%;
        }

        50% {
            position:absolute;
            transform: scale(0.50);
            opacity: 0.50;
            bottom: 50%;
        }

        75% {
            transform: scale(1);
            opacity: 1;
            bottom: 25%;
        }

        100% {
            transform: scale(1);
            opacity: 1;
            bottom: 25%;
        }
    }
</style>

<script>
    import Layout from '@/Shared/Layout'
    export default {
        props: ['foo'],
            components: {
                Layout
            },
        }
</script>

