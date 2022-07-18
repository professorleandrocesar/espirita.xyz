<template>
<div>    
<Nav/>
<NavTop/>

  <div class="main mainTree"> 
    <nuxt-link to="evangelho-segundo-o-espiritismo">
    
    <i class="fas fa-bible"></i> O Evangelho Segundo o Espiritismo
    </nuxt-link>
  </div>

  <div v-html='contentTree'></div>

<Footer/>
</div>
</template>
<script>
export default {
data() {
        return {
            content: ``,
            contenticonone: ``,
            contenticontwo: ``,
            contentTwo: '',
            finalidades: ``,
            aplicar: '',
            aplicarTwo: '',
            aplicarTree: '',
            aplicarFour: '',
            aplicarFive: '',
            aplicarSix: ''
        }
    },
  methods: {
    personal() {
      this.content = `
      <div class="main mainOne">
      <a href="https://instagram.com/professorleandrocesar" class=''>
        <i class="fab fa-instagram-square"></i> Instagram
      </a>
      <a href="https://professorleandrocesar.com" class=''>
        <i class="fas fa-globe"></i> Site
      </a>
      <a href="https://youtube.com/leandrocesarcosta" class=''>
        <i class="fab fa-youtube"></i> Youtube
      </a>
    <a href="https://blog.professorleandrocesar.com">
      <i class="fas fa-blog"></i> Blog
    </a>
  </div>
      `,
      this.aplicar= true,
      this.aplicarTwo= false,
      this.contentTwo = ``,
      this.contentTree = ``
    },
    deep() {
        this.contentTwo = `
        <div class="main mainTwo">
      <a href="https://instagram.com/deepacupuntura" class=''>
        <i class="fab fa-instagram-square"></i> Instagram
      </a>
      <a href="https://deepacupuntura.com" class=''>
        <i class="fas fa-globe"></i> Site
      </a>
      <a href="https://www.youtube.com/channel/UCRaQUE-GsQ4GglE8hElm17w" class=''>
        <i class="fab fa-youtube"></i> Youtube
      </a>
  </div>
      `,
      this.content = ``,
      this.contentTree = ``,
      this.aplicar= false,
      this.aplicarTwo= true
    },
    espirita() {
        this.contentTree = `
        <div class="main mainTree">
      <a href="https://instagram.com/espirita.xyz" class=''>
        <i class="fab fa-instagram-square"></i> Instagram
      </a>
      <a href="https://espirita.xyz" class=''>
        <i class="fas fa-globe"></i> Site
      </a>
  </div>
      `,
      this.content = ``,
      this.contentTwo = ``,
      this.aplicar= false,
      this.aplicarTwo= true
    }
  }
}
</script>