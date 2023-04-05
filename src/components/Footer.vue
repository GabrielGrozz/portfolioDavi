<script>
import linkedin from "../assets/linkedin.png";
import whatsapp from "../assets/whatsapp.png";
import itch from "../assets/itch.png";
import email from "../assets/email.png"

export default {
  name: "Footer",
  data() {
    return {
      whatsapp: whatsapp,
      linkedin: linkedin,
      itch: itch,
      email: email

    };
  },
};
</script>
<template>
  <div class="footer">

    <div class="contact" id="contact">

      <div class="whats">
        <img :src="whatsapp" width="50" height="50" alt="whatsapp" />

        <p class="link">(51) 98020-2003</p>
      </div>
      <div class="email">
        <img :src="email" alt="email">

        <p class="mail">davifigu21@gmail.com</p>
      </div>


      <div class="linkedin">
        <img :src="linkedin" alt="linkedin" />

        <a href="https://www.linkedin.com/in/davi-fig/" class="link">Linkedin</a>
      </div>

      <div class="linkedin">
        <img :src="itch" alt="linkedin" />

        <a href="https://kklavi.itch.io" class="link">Itch.io</a>
      </div>

    </div>

  </div>
</template>

<style scoped>
img{
  margin-right: 10px;
}

.footer {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 400px;
  background: rgb(22, 22, 22);
  flex-direction: column;
}

.text {
  font-family: Arial, Helvetica, sans-serif;
  color: white;
}

.contact {
  text-align: center;
  color: white;
  font-size: 2em;
  flex-direction: column;
}

.link {
  text-decoration: none;
  color: white;
}

.linkedin{
  margin: 6px;
}
.whats{
  display: flex;
  flex-direction: row;
}
.email{
  display: flex;
  flex-direction: row ;
  width: 48px;
  height: 48px;
  margin-left:-40px ;
}

.mail{
  color: white;
}
</style>
