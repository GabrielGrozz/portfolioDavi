<script setup>
import photo from "../assets/dave.jpg";
</script>

<template>
  <div class="header-container">
    <div class="anchors flex">
      <a class="anchor" href="#projects">Projetos</a>
      <a class="anchor" href="#contact">Contatos</a>
    </div>
    <div class="name-container">
      <h1 class="name">Davi Figueiredo</h1>
    </div>
    <div class="links-container flex">
      <Link name="Linkedin" link="#" :img="linkedinLogo" />
      <Link name="Discord" link="#" :img="discordLogo" />
      <Link name="Twitter" link="#" :img="twitterLogo" />
    </div>
    <div class="main-container flex">
      <div class="photo-name-container flex">
        <img :src="photo" alt="" class="photo" />
      </div>
      <div class="name-about-container flex">
        <div class="about-me">
          <p class="about">
            Olá, meu nome é Davi Figueiredo, tenho 19 anos, e desde os 8 sou apaixonado por jogos eletrônicos e de mesa. Já participei como game designer em gamejams e projetos pessoais enquanto estudo para me graduar na área.<p/>
           
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.links-container {
  flex-direction: row;
  justify-content: end;
  align-items: center;
}

.main-container {
  background-color: rgb(252, 252, 252);
  height: 95vh;
  padding: 0 10vw;
  align-items: center;
}

.photo-name-container {
  display: flex;
  flex-direction: column;
  margin: 20px;
  text-align: center;

  width: auto;
  height: auto;
  max-height: 350px;
  max-width: 350px;
}

.name {
  margin-top: 100px;
}

.name-about-container {
  flex-direction: column;
}

.about{
  font-size: 2em;
}

.photo {
  border-radius: 50%;
  margin-bottom: 30px;
  width: 380px;
  height: 380px;
  border: 5px rgb(161, 161, 161) solid;
  box-shadow: 8px 10px 15px rgb(122, 122, 122);
}

.about-me {
  text-align: center;
  padding: 50px;
}

.anchors {
  margin-top: 15px;
  flex-direction: row;
  justify-content: center;
  text-decoration: none;

}

.anchor {
  font-size: 2em;
  margin: 50px 40px 0 40px;
  transition: .3s;
  color: gray;
}

.anchor:hover{
  color: black;
}

@media screen and (max-width: 1250px) {
  .photo {
    width: 270px;
    height: 250px;
  }
  .about{
    font-size: 1.6em;
  }
}
@media screen and (max-width: 953px) {
  .main-container {
    padding: 0;
    flex-direction: column;
  }
  .about{
    font-size: 1.4em;
  }
}

@media screen and (max-width: 600px) {
  .about{
    font-size: 1.3em;
  }
}

@media screen and (max-width: 470px) {
  .about{
    font-size: .9em;
  }
}

</style>
