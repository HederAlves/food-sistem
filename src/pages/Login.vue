<template>
  <div class="mainContainer">
    <img
      class="imageLogin"
      src="/images/image-login.png"
      alt="imagem de lanches"
    />
    <section class="sectionForm">
      <h1 class="titleLogin">Bem vindo !</h1>
      <p>Faça seu login para continuar</p>
      <form class="loginForm" @submit.prevent="save">
        <i class="inputContainer">
          <img src="/icons/email.png" alt="" />
          <input
            class="inputLogin"
            type="text"
            placeholder="Seu e-mail"
            required="Digite seu Email"
          />
        </i>
        <i class="inputContainer">
          <img class="" src="/icons/password.png" alt="" />
          <input
            class="inputLogin"
            type="text"
            placeholder="Senha"
            required="Digite sua Senha"
          />
        </i>
        <button class="buttonPrimary">Entrar</button>
      </form>
      <span>
        <p class="lineDivision">ou</p>
      </span>
      <button class="buttonGoogle">Entrar com o Google</button>
      <p>Não tem uma conta?<a href="">Cadastre</a></p>
    </section>
  </div>
</template>

<script>
export default {
  name: "app",
};
</script>

<style scoped>
.mainContainer {
  @apply flex;
  color: #9098b1;
}
.imageLogin {
  @apply h-screen;
}
.sectionForm {
  @apply pt-20 pl-72 flex flex-col justify-around items-center;
  height: 560px;
}
.loginForm {
  @apply flex flex-col justify-around h-52;
}
.titleLogin {
  @apply font-bold text-2xl text-black;
}
.inputContainer {
  @apply flex p-2;
  width: 343;
  height: 48px;
  box-sizing: border-box;
  border: solid 2px #ebf0ff;
  border-radius: 5px;
}
.inputLogin {
  position: absolute;
  margin: -8px 0px 0px 36px;
  width: 343;
  height: 44px;
}
.inputLogin:focus {
  box-shadow: 0 0 0 0;
  border: 0 none;
  outline: 0;
}
.buttonPrimary {
  background: #dc9000;
  color: white;
  width: 343px;
  height: 57px;
  border-radius: 5px;
}
.buttonGoogle {
  color: #9098b1;
  width: 343px;
  height: 57px;
  border: solid 2px #ebf0ff;
  border-radius: 5px;
}
span {
  box-sizing: border-box;
  border-top: 2px solid #ebf0ff;
  width: 346px;
  text-align: center;
}
.lineDivision {
  position: absolute;
  margin: -16px 0px 0px 145px;
  background: white;
  padding: 0px 22px 0px 22px;
}
a {
  color: blue;
  font-weight: bold;
  margin-left: 8px;
}
</style>
