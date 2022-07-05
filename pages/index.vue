<template>
  <div class="scrollbar-hide ">
    <!-- HEADER -->
    <div class="w-full relative h-screen overflow-hidden">
      <div class="fixed top-4 z-50 w-full h-16 text-white flex justify-center items-center space-x-12" :class="{' transition ease-in-out delay-100 bg-secondary-text bg-opacity-5 drop-shadow-xl backdrop-blur-xl top-0 ': scrollPosition > 50}">
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer">
          <div class="h-1.5 w-1.5 rounded-full bg-primary drop-shadow-lg"></div>
          <a href="#"><div class="drop-shadow-xl text-primary">Home</div></a>
        </div>
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer">
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg"></div>
          <a href="#about"><div class="drop-shadow-xl">About Me</div></a>
        </div>
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer">
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg"></div>
          <a href="#skill"><div class="drop-shadow-xl">Skill</div></a>
        </div>
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer">
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg"></div>
          <div class="drop-shadow-xl">Projects</div>
        </div>
        <div class="flex flex-col items-center justify-center hover:opacity-80 hover:text-primary cursor-pointer">
          <div class="h-1.5 w-1.5 rounded-full  drop-shadow-lg"></div>
          <div class="drop-shadow-xl">Contact</div>
        </div>
      </div>

      <div class="absolute inset-0 mx-auto my-auto z-30 h-3/4 w-10/12 text-white flex items-center">
        <div class="flex flex-col justify-center w-1/2 h-full space-y-4 items-center">
          <div class="flex flex-col w-full items-start  px-14 ">
            <h2 class="text-3xl text-primary font-black uppercase">Medhy Pradana Putra</h2>
            <div class="border-2 w-3/4  mr-8 self-end border-primary"></div>
          </div>
          <div class="flex w-full items-start px-14 ">
            <h2 class="text-3xl text-white font-black ">Web Developer | Fullstack Developer</h2>
          </div>
          <div class="flex w-full items-start px-14 ">
            <p class="text-sm text-secondary-text">
              Fullstack developer | Web Developer focused on creating Web applications. I really like different projects that solve real problems.
            </p>
            
          </div>
          <div class="flex justify-around w-full py-10  ">
            <ButtonTransparent/>
            <ButtonSolid text="Portofolio" iconName="circle_down.svg"/>
          </div>
        </div>

        
        
      </div>
      
      <div class="absolute bg-secondary-light h-full w-full z-0"></div>

      <div class="absolute transform bg-secondary-dark h-full w-9/12 z-10 overflow-hidden text-white">
      </div>

      <div class="absolute bg-secondary-light w-[200vh] h-[80vh] rotate-[60deg] -top-40 ml-[16rem] transform z-10 overflow-hidden">
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
        
      
    </div>
    <!-- END HEADER -->

    <!-- ABOUT ME -->
    <div class="flex w-full relative h-[50vh] bg-secondary justify-center text-white overflow-hidden" id="about">
      <div class="text-secondary-textdark absolute inset-4  font-black ">
        <div class=" absolute top-4 -right-32 text-9xl">ABOUT</div>
      </div>
      <div class="text-secondary-textdark absolute inset-4  font-black ">
        <div class=" absolute bottom-0 -left-6 w-1/12 space-y-2">
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
          </div>
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
          </div>
          <div class="flex space-x-2">
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
            <div class=" rounded-full bg-secondary-textdark w-4 h-4"></div>
          </div>
        </div>
      </div>
      <div class="w-1/2 h-full  flex flex-col items-center space-y-8 ">
        <div class="items-center flex flex-col mt-20">
          <span class="text-2xl px-40 uppercase font-black">About Me</span>
          <div class="border-2 border-primary w-1/12"></div>
        </div>
        <div class="flex w-3/4">
          <p class="text-md text-secondary-text text-center">Hello, you can call me <span class="text-primary">Medhy</span> and I am <span class="text-primary">{{getYear}}</span> years old. <br>
              I love coding and i really enjoyed work as <span class="text-primary">Front End Developer</span> <br>I have a creative mind and I always up for <span class="text-primary">new challenges.</span><br>
              Welcome aboard and enjoy the journey.
            </p>
        </div>
      </div>
    </div>
    <!-- END ABOUT ME -->

    <!-- MY SKILLS -->
    <div class="flex w-full relative bg-secondary justify-center text-white " id="skill">
      <div class="w-3/4 h-full  flex flex-col items-center space-y-8 mb-10 p-10">
        <div class="items-center flex flex-col">
          <span class="text-xl  font-black">My Skills</span>
        </div>
        <div class="grid grid-cols-5 gap-4 w-3/4">
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
            <div class="bg-secondary-light p-5 rounded flex flex-col items-center space-y-2">
              <img src="~/assets/img/vue.png" class="w-5 h-5" alt="">
              <span class="text-primary">Vue.js</span>
            </div>
        </div>
      </div>
    </div>
    <!-- END MY SERVICES -->
    
  </div>
</template>

<script>
export default {
  name: 'IndexPage',
  data(){
    return{
      birth: 1995,
      scrollPosition: null
    }
  },
  methods: {
    updateScroll() {
       this.scrollPosition = window.scrollY
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
