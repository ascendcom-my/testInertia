<template>
    <layout>
        <div id="bg-video" class="w-full h-full bg-contain bg-no-repeat bg-center bg-neutral-800">
            <div class="absolute right-1/2 flex flex-col items-center w-40">
                
                <img id="personImg" class="w-20" />
                <img id="cardNameImg" class="w-full h-6" />
                
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
        content:url("/images/person1.jpg");
    }

    #cardNameImg{
        content:url("/images/card.Png");
        
    }
</style>

<script>
    import Layout from '@/Shared/Layout'
    import VideoBg from 'vue-videobg'
    export default {
        props: ['foo'],
            components: {
                Layout,
                VideoBg:'video-bg'
            },
        }
</script>

