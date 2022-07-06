<template>
  <div class="">
    <!-- HEADER -->
    <div class="w-full relative h-screen overflow-hidden bg-secondary-light ">
      <div class="md:hidden">
        <div id='stars'></div>
        <div id='stars2'></div>
        <div id='stars3'></div>
      </div>

      <div class="fixed top-2 z-50 w-full h-16 text-white flex justify-around px-2 md:px-0 md:justify-center items-center md:space-x-12 " :class="{' transition ease-in-out delay-100 bg-secondary-text bg-opacity-5 drop-shadow-xl backdrop-blur-xl -top-2 my-2': scrollPosition > 10}">
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer" >
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg" :class="{'bg-primary' : activeMenu == 1}"></div>
          <a href="#"><div class="drop-shadow-xl " :class="{'text-primary': activeMenu == 1}">Home</div></a>
        </div>
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer " >
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg" :class="{'bg-primary' : activeMenu == 2}"></div>
          <a href="#about"><div class="drop-shadow-xl" :class="{'text-primary' : activeMenu == 2}">About Me</div></a>
        </div>
        <!-- <div class="hidden md:flex md:flex-col md:items-center md:justify-center hover:opacity-80 hover:text-primary cursor-pointer" >
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg" :class="{'bg-primary' : activeMenu == 3}"></div>
          <a href="#skill"><div class="drop-shadow-xl" :class="{'text-primary' : activeMenu == 3}">Skill</div></a>
        </div> -->
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer" >
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg" :class="{'bg-primary' : activeMenu == 4}"></div>
          <div class="drop-shadow-xl" :class="{'text-primary' : activeMenu == 4}">Projects</div>
        </div>
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer" >
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg" :class="{'bg-primary' : activeMenu == 5}"></div>
          <div class="drop-shadow-xl" :class="{'text-primary' : activeMenu == 5}">Contact</div>
        </div>
      </div>

      <div class="absolute bottom-4  md:inset-0 mx-auto my-auto z-30 h-1/2  w-full md:w-10/12 text-white flex items-center">
        <div class="flex flex-col justify-center w-full md:w-1/2 h-full space-y-4 items-center">
          <div class="flex flex-col w-full items-start px-10 md:px-14">
            <h2 class="text-2xl md:text-3xl text-primary font-black uppercase">Medhy Pradana Putra</h2>
            <div class="border md:border-2 w-3/4  md:mr-8 self-end border-primary"></div>
          </div>
          <div class="flex w-full items-start px-10 md:px-14 ">
            <h2 class="text-xl text-white font-black ">Web Developer | Fullstack Developer</h2>
          </div>
          <div class="flex w-full items-start px-10 md:px-14 ">
            <p class="text-sm text-secondary-text">
              Fullstack developer | Web Developer focused on creating Web applications. <br>I really like different projects that solve real problems.
            </p>
            
          </div>
          <div class="flex justify-around w-full py-10  ">
            <ButtonTransparent/>
            <ButtonSolid text="Portofolio" iconName="circle_down.svg"/>
          </div>
        </div>
      </div>
      
      <div class="hidden md:block absolute bg-secondary-light h-full w-full z-0"></div>

      <div class="hidden md:block absolute transform bg-secondary-dark h-full w-9/12 z-10 overflow-hidden text-white">
      </div>

      <div class="hidden md:block absolute bg-secondary-light w-[200vh] h-[80vh] rotate-[60deg] -top-40 ml-[16rem] transform z-10 overflow-hidden">
        <div class="flex justify-center items-center pt-52 w-screen h-screen ">
          <div class="absolute pt-56 border-4 blur-lg border-primary w-[600px]  h-[600px] rounded-full top-72 ml-[48vh]"></div>
          <div class="absolute pt-56 border-4 blur-md border-primary w-[600px]  h-[600px] rounded-full top-72 ml-[48vh]"></div>
          <div class="absolute pt-56 border-4 blur-sm border-primary w-[600px]  h-[600px] rounded-full top-72 ml-[48vh]"></div>
          <div class="absolute pt-56 border-4 border-primary w-[600px]  h-[600px] rounded-full top-72 ml-[48vh]"></div>
          <div class="absolute pt-56 w-[600px]  h-[600px] rounded-full -bottom-32  ml-[36vh]">
            <img src="~/assets/img/Image_Portfolio.png" class="rotate-[-60deg] " alt="">
          </div>
        </div>
      </div>

      <div class="w-full flex justify-center md:hidden absolute top-28">
        <div class="absolute w-[300px] h-[300px] ">
          
          <div class="absolute blur-xl  border-4 border-primary w-full h-full  rounded-full z-20"></div>
          <div class="absolute blur-lg  border-4 border-primary w-full h-full  rounded-full z-20"></div>
          <div class="absolute blur-md  border-4 border-primary w-full h-full  rounded-full z-20"></div>
          <div class="absolute  border-4 border-primary w-full h-full  rounded-full overflow-hidden z-20 ">
              <img src="~/assets/img/medhy.png" class="absolute transform -rotate-3 left-5 grayscale">
          </div>
        </div>
      </div>
    
    </div>
    <!-- END HEADER -->

    <!-- ABOUT ME -->
    <div class="flex w-full relative h-[50vh] bg-secondary justify-center text-white overflow-hidden" id="about">
      <div class="text-secondary-dark absolute inset-4  font-black z-10">
        <div class=" absolute top-4 md:-right-32 -right-36 text-9xl">ABOUT</div>
      </div>
      <div class="text-secondary-dark absolute inset-4  font-black ">
        <div class=" absolute bottom-0 -left-6 md:w-2/12 space-y-2">
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
          </div>
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
          </div>
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
          </div>
        </div>
      </div>
      <div class="w-full md:px-0 md:w-1/2 h-full flex flex-col items-center space-y-8 z-20">
        <div class="items-center flex flex-col mt-20">
          <span class="text-2xl md:px-40 uppercase font-black">About Me</span>
          <div class="border md:border-2 border-primary w-4/12 md:w-1/12"></div>
        </div>
        <div class="flex w-3/4 justify-center">
          <p class="text-md text-secondary-text text-center">Hello, you can call me <span class="text-primary">Medhy</span> and I am <span class="text-primary">{{getYear}}</span> years old. <br>
              I love coding and i really enjoyed work as <span class="text-primary">Front End Developer</span> <br>I have a creative mind and I always up for <span class="text-primary">new challenges.</span><br>
              Welcome aboard and enjoy the journey.
            </p>
        </div>
      </div>
    </div>
    <!-- END ABOUT ME -->

    <!-- MY SKILLS -->
    <div class="flex w-full relative bg-secondary justify-center text-white" >
      <div class="w-full md:w-3/4  h-full  flex flex-col items-center space-y-8 mb-10 md:p-10">
        <div class="items-center flex flex-col">
          <span class="text-xl  font-black">My Skills</span>
        </div>
        <div class="grid grid-cols-3 md:grid-cols-5 gap-4 md:w-3/4">
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2 hover:opacity-60 transition ease-in-out delay-150 hover:scale-110">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
        </div>
      </div>
    </div>
    <!-- END MY SERVICES -->

    <!-- EDUCATION JOBS -->
    <div class="flex relative w-full bg-secondary justify-center text-white overflow-hidden pb-28" >
      <div class="w-full md:w-3/4 z-20 justify-center flex">
          <div class="w-3/4 md:w-full px-4 flex flex-col md:flex-row md:justify-between py-10 md:px-10 lg:px-40 space-y-4 md:space-y-0 md:divide-y-0 divide-y divide-primary">
              <!-- EDUCATION -->
              <div class="flex flex-col pb-4 md:pb-0 ">
                <label class="text-xl font-black mb-4 text-center">Education</label>
                <div class="space-y-4">
                  <div class="w-full">
                    <div class="w-full md:w-full space-y-1 flex flex-col">
                      <div class="text-sm">January 2020 - December 2020 20200 20200</div>
                      <div class="text-base text-primary">Teknik Komputer Jaringan</div>
                      <div class="text-xs text-secondary-text">SMK Media Informatika 2018 2020</div>
                    </div>
                  </div>
                  <div class="w-full">
                    <div class="w-full md:w-full space-y-1 flex flex-col ">
                      <div class="text-sm">January 2020 - December 2020</div>
                      <div class="text-base text-primary">Teknik Komputer Jaringan</div>
                      <div class="text-xs text-secondary-text">SMK Media Informatika</div>
                    </div>
                  </div>
                </div>
              </div>
              <!-- JOBS -->
              <div class="flex flex-col pt-4 md:pt-0">
                <label class="text-xl font-black mb-4 text-center">Jobs</label>
                <div class="space-y-4">
                  <div class="w-full">
                    <div class="w-full md:w-full space-y-1 flex flex-col ">
                      <div class="text-sm">January 2020 - December 2020</div>
                      <div class="text-base text-primary">Teknik Komputer Jaringan</div>
                      <div class="text-xs text-secondary-text">SMK Media Informatika</div>
                    </div>
                  </div>
                  <div class="w-full">
                    <div class="w-full md:w-full space-y-1 flex flex-col ">
                      <div class="text-sm">January 2020 - December 2020</div>
                      <div class="text-base text-primary">Teknik Komputer Jaringan</div>
                      <div class="text-xs text-secondary-text">SMK Media Informatika</div>
                    </div>
                  </div>
                </div>
              </div>
          </div>
      </div>
      <div class="text-secondary-dark absolute inset-4  font-black">
        <div class=" absolute -top-6 -right-6 md:w-2/12 space-y-2">
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
          </div>
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
          </div>
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
          </div>
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-dark w-4 h-4"></div>
          </div>
        </div>
      </div>
      <div class="text-secondary-dark absolute inset-4 font-black z-10">
        <div class=" absolute bottom-0 -left-14 space-y-2">
          <span class="text-9xl">UT ME</span>
        </div>
      </div>
    </div>
    <!-- END EDUCATION JOBS -->
    

    
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data(){
    return{
      birth: 1995,
      scrollPosition: null,
      activeMenu: 1, // 1,2,3,4
    }
  },
  methods: {
    updateScroll() {
       this.scrollPosition = window.scrollY
       if (this.scrollPosition > 0 && this.scrollPosition < 200) {
          this.activeMenu = 1
       }else if(this.scrollPosition > 650){
          this.activeMenu = 2
       }
    }
  },
  mounted() {
    window.addEventListener('scroll', this.updateScroll);
    
  },
  computed: { 
    getYear () {
      const currentDate = new Date()
      const currentYear = currentDate.getFullYear()
      return currentYear - this.birth
    },

  },
}
</script>
