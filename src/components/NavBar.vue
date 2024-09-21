<template>
  <v-app-bar app color="brown" dark flat class="px-12">
    <v-btn>
        <v-icon color="white" left class="mr-2">fas fa-signature</v-icon>RJSC
    </v-btn>
    <v-spacer></v-spacer>
    <v-btn text @click="scroll('home')" class="text-white">Home</v-btn>
    <v-btn text @click="scroll('about')" class="text-white">About</v-btn>
    <v-btn text @click="scroll('portfolio')" class="text-white">Portfolio</v-btn>
    <v-btn text @click="scroll('services')" class="text-white">Services</v-btn>
    <v-btn text @click="scroll('biog')" class="text-white">Biog</v-btn>
    <v-btn text @click="scroll('blog')" class="text-white">Blog</v-btn>
    <v-btn text @click="scroll('contact')" class="text-white">Contact</v-btn>
  </v-app-bar>
</template>

<script>
export default {
    methods: {
        scroll(refName){
            const element = document.getElementById(refName);
            element.scrollIntoView({behavior: 'smooth'});
        }
    }

}
</script>

<style>

</style>