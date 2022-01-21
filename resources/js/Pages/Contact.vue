<template>
    <layout>
        <div id="bg-video" class="w-full h-full bg-contain bg-no-repeat bg-center bg-neutral-800">
            <div id="model1" class="absolute left-1/2 flex flex-col items-center w-40">
                <div id="personImg1" class="w-20"></div>
                <div id="cardNameImg1" class="w-full h-6"></div>
            </div>

            <div id="model2" class="absolute right-1/2 flex flex-col items-center w-40">
                <div id="personImg2" class="w-20"></div>
                <div id="cardNameImg2" class="w-full h-6"></div>
            </div>

            <div id="model3" class="absolute left-1/2 flex flex-col items-center w-40">
                <div id="personImg3" class="w-20"></div>
                <div id="cardNameImg3" class="w-full h-6"></div>
            </div>

            <div id="model4" class="absolute right-1/2 flex flex-col items-center w-40">
                <div id="personImg4" class="w-20"></div>
                <div id="cardNameImg4" class="w-full h-6"></div>
            </div>

            <div id="model5" class="absolute left-1/2 flex flex-col items-center w-40">
                <div id="personImg5" class="w-20"></div>
                <div id="cardNameImg5" class="w-full h-6"></div>
            </div>

            <div id="model6" class="absolute right-1/2 flex flex-col items-center w-40">
                <div id="personImg6" class="w-20"></div>
                <div id="cardNameImg6" class="w-full h-6"></div>
            </div>

            <div id="model7" class="absolute left-1/2 flex flex-col items-center w-40">
                <div id="personImg7" class="w-20"></div>
                <div id="cardNameImg7" class="w-full h-6"></div>
            </div>

            <div id="model8" class="absolute right-1/2 flex flex-col items-center w-40">
                <div id="personImg8" class="w-20"></div>
                <div id="cardNameImg8" class="w-full h-6"></div>
            </div>

        </div>
    </layout>
</template>

<style>

    #bg-video{
        
        background-image: url("/images/bg1.gif");
        transition: background-image 2s linear;
    }

    #bg-video.changeBg2{
        background-image: url("/images/bg2.gif");
    }

    #bg-video.changeBg3{
        background-image: url("/images/bg3.gif");
    }


    #model1{
        opacity: 0;
        bottom: 80%;
        scale: 0;
        transition: bottom 3s, opacity 3s, transform 3s;
        transition-timing-function: ease-out;
        /* animation: flow 10s linear; */
    }

    #model1.active {
        transform: scale(1.5);
        opacity: 2;
        bottom: 25%;
        /* bottom: 500px; */
    }

    #model1.past {
        opacity: 0;
        /* bottom: 500px; */
    }

     #model2{
        opacity: 0;
        bottom: 80%;
        scale: 0;
        transition: bottom 3s, opacity 3s, transform 3s;
        transition-timing-function: ease-out;
        /* animation: flow 10s linear; */
    }

    #model2.active {
        transform: scale(1.5);
        opacity: 2;
        bottom: 25%;
        /* bottom: 500px; */
    }

    #model2.past {
        opacity: 0;
        /* bottom: 500px; */
    }

     #model3{
        opacity: 0;
        bottom: 80%;
        scale: 0;
        transition: bottom 3s, opacity 3s, transform 3s;
        transition-timing-function: ease-out;
        /* animation: flow 10s linear; */
    }

    #model3.active {
        transform: scale(1.5);
        opacity: 2;
        bottom: 25%;
        /* bottom: 500px; */
    }

    #model3.past {
        opacity: 0;
        /* bottom: 500px; */
    }

     #model4{
        opacity: 0;
        bottom: 80%;
        scale: 0;
        transition: bottom 3s, opacity 3s, transform 3s;
        transition-timing-function: ease-out;
        /* animation: flow 10s linear; */
    }

    #model4.active {
        transform: scale(1.5);
        opacity: 2;
        bottom: 25%;
        /* bottom: 500px; */
    }

    #model4.past {
        opacity: 0;
        /* bottom: 500px; */
    }
    
     #model5{
        opacity: 0;
        bottom: 80%;
        scale: 0;
        transition: bottom 3s, opacity 3s, transform 3s;
        transition-timing-function: ease-out;
        /* animation: flow 10s linear; */
    }

    #model5.active {
        transform: scale(1.5);
        opacity: 2;
        bottom: 25%;
        /* bottom: 500px; */
    }

    #model5.past {
        opacity: 0;
        /* bottom: 500px; */
    }

     #model6{
        opacity: 0;
        bottom: 80%;
        scale: 0;
        transition: bottom 3s, opacity 3s, transform 3s;
        transition-timing-function: ease-out;
        /* animation: flow 10s linear; */
    }

    #model6.active {
        transform: scale(1.5);
        opacity: 2;
        bottom: 25%;
        /* bottom: 500px; */
    }

    #model6.past {
        opacity: 0;
        /* bottom: 500px; */
    }

     #model7{
        opacity: 0;
        bottom: 80%;
        scale: 0;
        transition: bottom 3s, opacity 3s, transform 3s;
        transition-timing-function: ease-out;
        /* animation: flow 10s linear; */
    }

    #model7.active {
        transform: scale(1.5);
        opacity: 2;
        bottom: 25%;
        /* bottom: 500px; */
    }

    #model7.past {
        opacity: 0;
        /* bottom: 500px; */
    }

     #model8{
        opacity: 0;
        bottom: 80%;
        scale: 0;
        transition: bottom 3s, opacity 3s, transform 3s;
        transition-timing-function: ease-out;
        /* animation: flow 10s linear; */
    }

    #model8.active {
        transform: scale(1.5);
        opacity: 2;
        bottom: 25%;
        /* bottom: 500px; */
    }

    #model8.past {
        opacity: 0;
        /* bottom: 500px; */
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

        var personUrl = ["person1.jpg",
                     "person2.jpg",
                     "person3.jpg",
                     "person4.jpg",
                     "person5.jpg",
                     "person6.jpg",
                     "person7.jpg",
                     "person8.jpg"];

    $(document).ready(function() {

        $("#personImg1").css("content","url(/images/"+ personUrl[0] + ")");
        $("#cardNameImg1").css("content","url(/images/card.PNG)");

        $("#personImg2").css("content","url(/images/"+ personUrl[1] + ")");
        $("#cardNameImg2").css("content","url(/images/card.PNG)");

        $("#personImg3").css("content","url(/images/"+ personUrl[2] + ")");
        $("#cardNameImg3").css("content","url(/images/card.PNG)");

        $("#personImg4").css("content","url(/images/"+ personUrl[3] + ")");
        $("#cardNameImg4").css("content","url(/images/card.PNG)");

        $("#personImg5").css("content","url(/images/"+ personUrl[4] + ")");
        $("#cardNameImg5").css("content","url(/images/card.PNG)");

        $("#personImg6").css("content","url(/images/"+ personUrl[5] + ")");
        $("#cardNameImg6").css("content","url(/images/card.PNG)");

        $("#personImg7").css("content","url(/images/"+ personUrl[6] + ")");
        $("#cardNameImg7").css("content","url(/images/card.PNG)");

        $("#personImg8").css("content","url(/images/"+ personUrl[7] + ")");
        $("#cardNameImg8").css("content","url(/images/card.PNG)");
        

        
        $("#model1").addClass("active");

         var nextImgIndex = 2;
         var totalLength = personUrl.length;
         var prevImgIndex = 1;
         

         setInterval(function() {
            if(nextImgIndex > 4){
                $("#bg-video").addClass("changeBg2");
            }
            if(nextImgIndex > personUrl.length){
                $("#bg-video").addClass("changeBg3");
            }
            $("#model"+ prevImgIndex ).addClass("past");
            $("#model"+ nextImgIndex ).addClass("active");
            prevImgIndex = nextImgIndex;

            nextImgIndex++;


         },3000);

        // for (var n = 0; n < personUrl.length; n++){
            // $("#personImg").css("content","url(/images/"+ personUrl[n] + ")");
            // $("#cardNameImg").css("content","url(/images/card.PNG)");

        //     // setInterval(function() {
        //     //     nextShow(n);
        //     // },3000);

        //     // $("#model").removeClass("active");

        // }
        
    });

    

    var backgroundUrl = ["/images/bg1.gif",
                         "/images/bg2.gif",
                         "/images/bg3.gif"];

    

    function nextShow(currentIndex){
        // $("#personImg").css("content","url(/images/"+ personUrl[currentIndex] + ")");
        
      
    }
</script>

