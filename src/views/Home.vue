<template>
  <div>
    <mod-hero
      colored-heading= "visual designer"
      heading= "websited development.Redifined."
      text= "we will give you a website that worksk for you as intended"
      btn-text= "view more"
      btn-link = "/"
    ></mod-hero>
    <mod-about-section 
      section-heading= "about kwenda"
      img= "https://source.unsplash.com/random"
      lazy-img= ""
      img-alt= ""
      :info="myInfo"
      heading= "lorem df sd fas d"
      text= "eDGASK SD  fdsjfh cgd hfd gfj jh gdghd ghdjh fjhkf jhdf gjh dghd jhfdgd gd gjdjgd jgd gd jd gdjgd t uf ukf yfk uyf kuyfyuk fykfjh fjf "
      btn-text= "donwlaod cv"
      btn-link= "/home"
    ></mod-about-section>
    <mod-services-section
      :services="services"
    ></mod-services-section>
    <mod-portfolio-section></mod-portfolio-section>
    <mod-contact-section></mod-contact-section>
  </div>
</template>

<script>

import modHero from '@/components/mod_sections/mod_hero/modHero.vue'
import modAboutSection from '@/components/mod_sections/mod_main/modAboutSection.vue'
import modServicesSection from '@/components/mod_sections/mod_main/modServicesSection.vue'
import modPortfolioSection from '@/components/mod_sections/mod_main/modPortfolioSection.vue'
import modContactSection from '@/components/mod_sections/mod_main/modContactSection.vue'
//import modHeroOne from '@/components/mod_sections/mod_hero/modHeroOne.vue'

export default {
  name: 'Home',
  components: {
    modHero,
    modAboutSection,
    modServicesSection,
    modPortfolioSection,
    modContactSection
  },
  data(){
    return{
      myInfo:[
        {
            icon: 'mdi-gift',
            title: 'birthday',
            info: '02.06.1900',
        },
        {
            icon: 'mdi-book-open-outline',
            title: 'study',
            info: '02.06.1900',
        },
        {
            icon: 'mdi-earth',
            title: 'website',
            info: 'www.dummy.com',
        },
        {
            icon: 'mdi-pac-man',
            title: 'interest',
            info: 'reading',
        },
        {
            icon: 'mdi-map-marker',
            title: 'location',
            info: '402, random location',
        },
      ],
      services: [
        {
            icon: 'mdi-earth',
            heading: 'something somthing',
            desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Delectus porro suscipit rerum commodi labore debitis nesciunt quibusdam est ipsum voluptatum?',
            link: '/'
        },
        {
            icon: 'mdi-earth',
            heading: 'something somthing',
            desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Delectus porro suscipit rerum commodi labore debitis nesciunt quibusdam est ipsum voluptatum?',
            link: '/'
        },
        {
            icon: 'mdi-earth',
            heading: 'something somthing',
            desc: 'Lorem ipsum dolor, sit amet consectetur adipisicing elit. Delectus porro suscipit rerum commodi labore debitis nesciunt quibusdam est ipsum voluptatum?Lorem ipsum dolor, sit amet consectetur adipisicing elit. Delectus porro suscipit rerum commodi labore debitis nesciunt quibusdam est ipsum voluptatum?',
            link: '/'
        },
      ]
    }
  }
}
</script>

<style lang="scss" scoped>
   

</style>