<script>
import "../app.css";
import { onMount } from 'svelte';
var checkboxmssg = "By creating an account, you agree to our <span class='text-indigo-700 font-bold cursor-pointer'>terms</span> and <span class='text-indigo-700 font-bold cursor-pointer'>privacy policy</span>";

// @ts-ignore
var errboard;
// @ts-ignore
let inp1;
// @ts-ignore
let inp2;
// @ts-ignore
let inp3;
// @ts-ignore
var btn;
var roll = '<i class="las la-sync"></i>';
onMount(()=>
    // @ts-ignore
    btn.addEventListener('click', (e)=>{
        // @ts-ignore
        if(inp1.value.length < 2){
            console.log("name is too short!")
            // @ts-ignore
            errboard.style.display = "block";
            // @ts-ignore
            errboard.innerHTML = "name is invalid !"
            setTimeout(()=>{
                // @ts-ignore
                errboard.style.display="none"
            }, 8000)
            e.preventDefault();
        // @ts-ignore
        }else if(inp2.value.length < 2){
            console.log("email is too short!")
            // @ts-ignore
            errboard.style.display = "block";
            // @ts-ignore
            errboard.innerHTML = "email is invalid !"
            setTimeout(()=>{
                // @ts-ignore
                errboard.style.display="none"
            }, 8000)
            e.preventDefault();
        // @ts-ignore
        }else if(inp3.value.length < 8){
            console.log("password is too short!")
            // @ts-ignore
            console.log(inp3.value.length)
            // @ts-ignore
            errboard.style.display = "block";
            // @ts-ignore
            errboard.innerHTML = "password must be 8 characters !"
            setTimeout(()=>{
                // @ts-ignore
                errboard.style.display="none"
            }, 8000)
            e.preventDefault();
        }else{
            // @ts-ignore
            errboard.style.display = "block";
            // @ts-ignore
            errboard.style.backgroundColor = "#86efac"
            // @ts-ignore
            errboard.innerHTML = `Checking ${roll}`;
        }
    })
);

var loginmssg = 'Login';
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

<div class="mt-[100px] md:ml-[320px] lg:ml-[400px] md:mt-[60px] md:p-[10px] p-[15px] w-[100%] md:w-[50%] lg:w-[70%]">
    <div class="bg-red-300 w-[100%] p-[15px] h-fit text-white font-medium rounded-md hidden shadow-sm shadow-gray-300" bind:this={errboard}></div>
    <!---->
    <div class="mt-[10px]">
        <div id="sfont">
            <span class="font-bold md:text-[30px] text-[26px]">
                Sign Up
                <span><i class="las la-mobile-alt"></i></span>
            </span>
            <div class="font-thin text-slate-700 mt-[4px]">
                Fill in the required form below to signup
            </div>
        </div>
        <!---->
        <form>
            <div class="mt-[30px] w-[90%] md:w-[100%] lg:w-[100%]" id="ffont">
                <div class="lg:flex space-y-[15px] lg:space-x-[90px] lg:space-y-[0px]">
                    <div id="sfont" class="lg:w-[50%]">
                        <div class="">
                            <div class="text-[14px] md:text-[14px]">Your name</div>
                            <div class="md:mt-[7px] mt-[8px]">
                                <input type="text" placeholder="your name" class="border border-slate-700 md:p-[10px] p-[10px] w-full rounded-lg" bind:this={inp1}/>
                            </div>
                        </div>
                    </div>
                    <!--form space 2-->
                    <div id="sfont" class="lg:w-[50%]">
                        <div class="">
                            <div class="text-[14px] md:text-[14px]">Email address</div>
                            <div class="md:mt-[7px] mt-[8px]">
                                <input type="email" placeholder="youremail@gmail.com" class="border border-slate-700 md:p-[10px] p-[10px] w-full rounded-lg" bind:this={inp2}/>
                            </div>
                        </div>
                    </div>
                </div>
                <!--form space 3-->
                <div id="sfont" class="mt-[15px] lg:w-[45%]">
                    <div class="">
                        <div class="text-[14px] md:text-[14px]">Password</div>
                        <div class="md:mt-[7px] mt-[8px]">
                            <input type="password" placeholder="at least min 8 characters" class="border border-slate-700 md:p-[10px] p-[10px] w-full rounded-lg" bind:this={inp3}/>
                        </div>
                    </div>
                </div>
                <!---->
                <div class="mt-[15px] text-[12px] md:text-[12px] items-center">
                    <input type="checkbox"/>
                    <span>{@html checkboxmssg}</span>
                </div>
                <!--create btn-->
                <div class="mt-[20px] text-sm text-white font-semibold">
                    <button class="bg-slate-800 p-[10px] rounded-lg shadow-md shadow-slate-500 hover:bg-slate-700 focus:outline-none" bind:this={btn}>
                        Create Account
                        <span><i class="las la-external-link-alt"></i></span>
                    </button>
                </div>
                <div class="w-[100%] mt-[15px] inline-flex items-center">
                    <div class="w-[100%] bg-slate-400 h-[1px]"></div>
                    <div>&nbsp;or&nbsp;</div>
                    <div class="w-[100%] bg-slate-400 h-[1px]"></div>
                </div>
                <!--other auth method-->
                <div class="mx-auto align-center">
                    <div class="flex mx-auto items-center space-x-[10px] md:space-x-[10px] font-thin">
                        <button class="bg-red-700 w-fit p-[10px] rounded-md text-white text-[10px] md:text-[15px] text-center shadow-md shadow-gray-400">
                            <span><i class="lab la-github"></i></span>
                            <span>Connect with Github</span>
                        </button>
                        <!--2 auth-->
                        <button class="bg-red-700 w-fit p-[10px] rounded-md text-white text-[10px] md:text-[15px] text-center shadow-md shadow-gray-400">
                            <span><i class="lab la-google-plus-g"></i></span>
                            <span>Connect with Google</span>
                        </button>
                    </div>
                </div>
                <!--end auth-->
                <center class="mt-[20px] font-thin text-[15px]">
                    <span>Already have an account? <a href="/" class="font-medium text-red-500">{loginmssg}.</a></span>
                </center>
            </div>
        </form>
        <!--end form-->
    </div>
</div>