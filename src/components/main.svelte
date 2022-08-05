<script>
    import { not_equal } from "svelte/internal";
import "../app.css";
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=DM+Sans&family=Poppins:wght@300;400&display=swap');
    #sfont{
        font-family: 'Poppins', sans-serif;
    }
    #ffont{
        font-family: 'Poppins', sans-serif;
    }
    input::placeholder{
        font-size:13px;
        font-weight:300;
        color:#e5e7eb;
    }
    input:focus{
        outline:none;
    }
</style>

<div class="mt-[100px] md:ml-[350px] lg:ml-[400px] md:mt-[60px] p-[10px]">
    <div>
        <div id="sfont">
            <span class="font-bold md:text-[30px] text-[26px]">Sign Up</span>
        </div>
        <!---->
        <form>
            <div class="mt-[30px] w-[80%]" id="ffont">
                <div class="space-y-[20px] md:block lg:flex md:space-y-[20px] lg:space-x-[100px] lg:space-y-[0px]">
                    <div class="">
                        <div>Your name</div>
                        <div class="mt-[8px] md:w-[100%]">
                            <input type="text" class="border border-gray-200 rounded-md p-[5px] md:p-[8px] w-[80%] md:w-[120%]" placeholder="enter name"/>
                        </div>
                    </div>
                    <!---->
                    <div class="">
                        <div>Your email</div>
                        <div class="mt-[8px] md:w-[100%]">
                            <input type="email" class="border border-gray-200 rounded-md p-[5px] md:p-[8px] w-[80%] md:w-[120%]" placeholder="enter email"/>
                        </div>
                    </div>
                    <!---->
                </div>
                <!--passcode-->
                <div class="lg:inline-block mt-[20px]">
                    <div>Your password</div>
                    <div class="mt-[8px] md:w-[100%]">
                        <input type="password" class="border border-gray-200 rounded-md p-[5px] md:p-[8px] w-[80%] md:w-[120%] visible" placeholder="enter password"/>
                    </div>
                </div>
                <!--terms and conditions-->
                <div class="mt-[15px] text-[12px] font-normal md:text-[12px]">
                    <input type="checkbox" class=""/>
                    <span>By creating an account, you agree to our terms and privacy policy</span>
                </div>
                <!--create account btn-->
                <div class="mt-[30px]">
                    <button class="bg-gray-900 text-white p-[8px] font-bold rounded-md">
                        Create Account
                    </button>
                </div>
            </div>
        </form>
    </div>
</div>