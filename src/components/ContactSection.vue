<template>
    <section class="text-white mt-20" id="contact">
        <h2 class="text-3xl font-bold text-primary text-left mb-4 px-4 xl:pl-16">::::connect__with__me:::</h2>
        <div class="grid md:grid-cols-2 gap-4 relative px-4 xl:px-16 mt-8" data-aos="zoom-in-up">
            <div>
                <p class="text-white">Lorem ipsum dolor, 
                sit amet consectetur adipisicing elit. Dicta, tempore? Lorem ipsum dolor sit amet consectetur adipisicing elit. Quas alias voluptatum quidem illum magnam.
                Quia optio atque nam dignissimos harum. Lorem ipsum dolor sit, amet consectetur adipisicing elit. Accusamus, enim.</p>
                <div class="col-lg-4 col-md-4 mb-lg-0 mt-7">
                    <div class="flex mb-10 items-center">
                        <div class="p-2 shadow-md"
                        style="background: #23001b; width: 50px; height: 46px;
                        display: flex; justify-content: center; border-radius: 50%;
                        overflow: hidden; backdrop-filter: blur(9px);
                        -webkit-backdrop-filter: blur(9px);"                        
                        >
                            <img src="https://img.icons8.com/metro/50/ffffff/new-post.png" alt="new-post" class="w-6">
                        </div>
                        <div class="ml-5 text-white">
                            <h4>Email</h4>
                            <p>youremail@mail.com</p>
                        </div>
                    </div><!--/.items-center-->
                    <div class="flex mb-10 items-center">
                        <div class="p-2 shadow-md"
                        style="background: #23001b; width: 50px; height: 46px;
                        display: flex; justify-content: center; border-radius: 50%;
                        overflow: hidden; backdrop-filter: blur(9px);
                        -webkit-backdrop-filter: blur(9px);"                        
                        >
                            <img src="https://img.icons8.com/ios-filled/50/ffffff/phone.png" alt="phone" class="w-6">
                        </div>
                        <div class="ml-5 text-white">
                            <h4>Phone</h4>
                            <p>+00 000 00000</p>
                        </div>
                    </div><!--/.items-center-->
                    <div class="flex mb-10 items-center">
                        <div class="p-2 shadow-md"
                        style="background: #23001b; width: 50px; height: 46px;
                        display: flex; justify-content: center; border-radius: 50%;
                        overflow: hidden; backdrop-filter: blur(9px);
                        -webkit-backdrop-filter: blur(9px);"                        
                        >
                            <img src="https://img.icons8.com/ios-filled/50/ffffff/linkedin.png" alt="linkedin" class="w-6">
                        </div>
                        <div class="ml-5 text-white">
                            <h4>LinkedIn</h4>
                            <p>www.linkedin.com</p>
                        </div>
                    </div><!--/.items-center-->
                </div>
            </div>
            <div class="p-4 shadow-lg" 
             style="background: #23001b; width: 100%; height: 100%; border-radius: 20px;
                    overflow: hidden; backdrop-filter: blur(9px);
                    -webkit-backdrop-filter: blur(9px);" >
                <form class="flex flex-col p-2" data-aos="zoom-im-up">
                    <div class="mb-6">
                        <label for="email" class="text-white block mb-2 text-sm font-medium uppercase">your email</label>
                        <input type="email" id="email" class=" bg-secondary placeholder-gray text-gray-100 text-sm rounded-lg block w-full p-2" placeholder="youremail@email.com" name="email">
                    </div>
                    <div class="mb-6">
                        <label for="subject" class="text-white block mb-2 text-sm font-medium uppercase">your subject</label>
                        <input type="email" id="email" class=" bg-secondary placeholder-gray text-gray-100 text-sm rounded-lg block w-full p-2" placeholder="Subject goes here" name="subject">
                    </div>
                    <div class="mb-6">
                        <label for="email" class="text-white block mb-2 text-sm font-medium uppercase">your message</label>
                        <textarea type="email" id="email" class=" bg-secondary placeholder-gray text-gray-100 text-sm rounded-lg block w-full p-2" placeholder="Write your message" name="message">
                        </textarea>
                    </div>
                    <button class="z-1 px-6 md:px-7 py-3 rounded-full sm:w-max flex justify-center text-primary text-lg uppercase border-2 border-primary shadow-md">
                        Send Message
                    </button>
                </form>                            
            </div>
            <div class="bg-gradient-to-tr opacity-25 from-secondary to-primary blur-2xl h-20 w-80 z-0 absolute transform -translate-x-2/3 -translate-1/2"></div>
        </div><!--/.grid-->
    </section>
</template>
<script>
</script>