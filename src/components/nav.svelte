<script>
    import "../app.css";
</script>

<style>
    #navig{
        background-image: none;
        background-repeat: no-repeat;
        background-position: center;
        background-size: 100% 100%;
        background-color: #111827;
        opacity: 0.8;
    }

    @media only screen and (min-width:768px){
        #navig{
            background-color: #111827;
            background-repeat: no-repeat;
            background-position: center;
            background-size: 100% 100%;
        }
    }
</style>

<!---->
<header class="fixed top-0 w-full h-fit p-[10px] md:w-[300px] md:h-[100%]" id="navig">
    <div class="md:text-[30px] text-[25px] font-bold text-white md:mx-auto md:text-center  md:mt-[100%]">
        <span><i class="las la-wallet"></i></span>
        <span>Apey</span>
    </div>
    <!---->
    <div class="hidden md:text-center text-white md:block md:font-bold md:text-[30px]">
        <span>Welcome Back</span>
    </div>
</header>