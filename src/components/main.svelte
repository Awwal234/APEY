<script>
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
            <div class="mt-[30px] w-[90%] md:w-[80%]" id="ffont">
                <div class="space-y-[20px] md:block lg:flex md:space-y-[20px] lg:space-x-[100px] lg:space-y-[0px]">
                    <div class="w-[100%]">
                        <div>Your name</div>
                        <div class="mt-[8px]">
                            <input type="text" class="border border-gray-500 rounded-md p-[5px] md:p-[8px] w-[80%] md:w-[100%]" placeholder="enter name"/>
                        </div>
                    </div>
                    <!---->
                    <div class="w-[100%]">
                        <div>Your email</div>
                        <div class="mt-[8px]">
                            <input type="email" class="border border-gray-500 rounded-md p-[5px] md:p-[8px] w-[80%] md:w-[100%]" placeholder="enter email"/>
                        </div>
                    </div>
                    <!---->
                </div>
                <!--passcode-->
                <div class="lg:inline-block mt-[20px] w-[100%] lg:w-[50%]">
                    <div>Your password</div>
                    <div class="mt-[8px]">
                        <input type="password" class="border border-gray-500 rounded-md p-[5px] md:p-[8px] w-[80%] md:w-[100%] lg:w-[85%] visible" placeholder="enter password"/>
                    </div>
                </div>
                <!--terms and conditions-->
                <div class="mt-[15px] text-[12px] font-normal md:text-[12px]">
                    <input type="checkbox" class=""/>
                    <span>By creating an account, you agree to our terms and privacy policy</span>
                </div>
                <!--create account btn-->
                <div class="mt-[30px]">
                    <button class="bg-gray-900 text-white p-[8px] font-bold rounded-md hover:bg-gray-800 focus:outline-none">
                        Create Account
                    </button>
                </div>
            </div>
        </form>
    </div>
</div>