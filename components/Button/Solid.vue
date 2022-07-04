<template>
  <button
    class="
      px-6
      py-1.5
      text-secondary-font
      rounded-lg
      hover:opacity-80 hover:shadow-md
      flex
      items-center
      space-x-2
      text-black
    "
    :class="{
      'bg-primary': color == 'primary',
    }"
  >
    <div v-if="iconName" class="h-5 w-5 flex justify-center items-center">
      <img
        :src="require('/assets/svg/' + iconName)"
        class="h-full w-full text-white"
      />
    </div>
    <div class="text-sm">{{text}}</div>
  </button>
</template>
<script>
export default {
  data(){
    return{

    }
  },
  props:{
    color:{
      default: 'primary',
      type: String
    },
    text:{
      default: null,
      type: String
    },
    iconName:{
      default: null,
      type: String
    }
    
  }
}
</script>