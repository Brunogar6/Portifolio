<template>
    <div class="wrapper">
        <div class="main-container">
            <div class="container-one">
                <div class="profile">
                    <img src="../assets/1679498267997.jpeg" alt="">
                    <h1>Bruno Garcez</h1>
                    <p>Desenvolvedor PHP</p>
                </div>
                <div class="social-links">
                    <div class="link">
                        <a href="https://github.com/Brunogar6">
                            <img src="../assets/github-mark.png" alt="">
                            <h2>GitHub</h2>
                        </a>
                    </div>
                    <div class="link">
                        <a href="https://www.linkedin.com/in/bruno-garcez-3084b126b/">
                            <img src="../assets/linkedin-icon.png" alt="">
                            <h2>Linkedin</h2>
                        </a>
                    </div>
                </div>
            </div>
            <div class="container-two">
                <div class="about-me">
                    <h1>Sobre Mim</h1>
                    <p style="text-align: justify">Possuo experiência de 2 anos adquirida no último estágio que exerci, no qual trabalhei no site da empresa adquirindo experiência em HTML, CSS e javascript.
                        Além disso , desenvolvi sistemas afim de facilitar o trabalho dos usuários da empresa, nos quais melhorei minhas habilidades em PHP utilizando o framework laravel.
                        Também desempenhei nesta organização uma papel de atendimento ao usuário, auxiliando nos problemas computacionais do mesmo.</p>
                </div>
                <div class="technology-section">
                    <h1>Tecnologias Estudadas</h1>
                    <div class="logos">
                        <img src="../assets/mongodb.png" alt="">
                        <img src="../assets/laravel-icon.png" alt="">
                        <img src="../assets/logo-vue.svg" alt="">
                        <img src="../assets/postgre.png" alt="">
                        <img src="../assets/html.png" alt="">
                        <img src="../assets/css.png" alt="">
                    </div>
                </div>
                <div class="button-container">
                    <div class="projects-button">
                        <a href="https://cursos.alura.com.br/user/garcez-cpm2012/fullCertificate/3035191dd8463f35042a1e634a015028">Cursos</a>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "MainCard"
}
</script>

<style scoped>
  .wrapper{
      display: flex;
    justify-content: center;
  }
  img{
    height: 20px;
  }

  .main-container{
      display: flex;
      flex-direction: row;
      background-color: #A0D4FF;
      border-radius: 25px;
      width: 60%;
  }

  .container-one{
      background-color: #1292EE;
      padding: 2.5%;
      width: 60%;
      border-radius: 25px;
  }

  .profile img {
      height: 5rem;
      border-radius: 50%;
  }

  .link a{
      text-decoration: none;
      color: #2c3e50;
      font-size: 10px;
  }

  .link img{
      height: 2rem;
  }

  .container-two{
      margin: 2.5%;
      width: 70%;
  }

  .about-me{
      text-align: left;
  }

  .logos img{
      height: 2.5rem;
  }

  .button-container{
      margin-top: 5%;
      display: flex;
      flex-direction: row;
      justify-content: center;
      align-items: center;
  }

  .projects-button{
      background-color: #005CA4;
      border-radius: 15px;
      padding: 5px;
      margin: 5px;
  }

  .projects-button a{
      text-decoration: none;
      color: #fff;
  }
  
  @media only screen and (max-width: 950px) {
      .main-container{
          width: 95%;
      }
  }

</style>