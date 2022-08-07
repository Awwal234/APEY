<script>
import "../app.css";
var checkboxmssg = "By creating an account, you agree to our <span class='text-indigo-700 font-bold cursor-pointer'>terms</span> and <span class='text-indigo-700 font-bold cursor-pointer'>privacy policy</span>";
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=DM+Sans&family=Poppins:wght@300;400&display=swap');
    #sfont{
        font-family: 'Poppins', sans-serif;
    }
    #ffont{
        font-family: 'Poppins', sans-serif;
    }
    input{
        font-size:13px;
    }
    input::placeholder{
        font-size:13px;
        font-weight:300;
        color:#94a3b8;
    }
    input:focus{
        outline:none;
    }
</style>

<div class="mt-[100px] md:ml-[350px] lg:ml-[400px] md:mt-[60px] md:p-[10px] p-[15px]">
    <div>
        <div id="sfont">
            <span class="font-bold md:text-[30px] text-[26px]">Sign Up</span>
            <div class="font-thin text-slate-700 mt-[4px]">
                Fill in the required form below to signup
            </div>
        </div>
        <!---->
        <form>
            <div class="mt-[30px] w-[90%] md:w-[100%] lg:w-[100%]" id="ffont">
                <div class="lg:flex space-y-[15px] lg:space-x-[90px] lg:space-y-[0px] md:w-[100%] w-[100%]">
                    <div id="sfont" class="">
                        <div class="">
                            <div class="text-[14px] md:text-[14px]">Your name</div>
                            <div class="md:mt-[7px] mt-[8px]">
                                <input type="text" placeholder="your name" class="border border-slate-700 md:p-[8px] p-[10px] w-full rounded-lg"/>
                            </div>
                        </div>
                    </div>
                    <!--form space 2-->
                    <div id="sfont" class="">
                        <div class="">
                            <div class="text-[14px] md:text-[14px]">Email address</div>
                            <div class="md:mt-[7px] mt-[8px]">
                                <input type="email" placeholder="youremail@gmail.com" class="border border-slate-700 md:p-[8px] p-[10px] w-full rounded-lg"/>
                            </div>
                        </div>
                    </div>
                </div>
                <!--form space 3-->
                <div id="sfont" class="mt-[15px]">
                    <div class="">
                        <div class="text-[14px] md:text-[14px]">Password</div>
                        <div class="md:mt-[7px] mt-[8px]">
                            <input type="password" placeholder="at least min 8 characters" class="border border-slate-700 md:p-[8px] p-[10px] w-full rounded-lg"/>
                        </div>
                    </div>
                </div>
                <!---->
                <div class="mt-[15px] text-[12px] md:text-[12px] items-center">
                    <input type="checkbox"/>
                    <span>{@html checkboxmssg}</span>
                </div>
                <!--create btn-->
                <div class="mt-[20px] text-sm text-white font-medium">
                    <button class="bg-slate-800 p-[10px] rounded-lg shadow-md shadow-slate-500 hover:bg-slate-700">
                        Create Account
                    </button>
                </div>
                <div class="w-[100%] mt-[15px] inline-flex items-center">
                    <div class="w-[100%] bg-slate-400 h-[1px]"></div>
                    <div>&nbsp;or&nbsp;</div>
                    <div class="w-[100%] bg-slate-400 h-[1px]"></div>
                </div>
            </div>
        </form>
        <!--end form-->
    </div>
</div>