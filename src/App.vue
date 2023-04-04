<template>
  <!-- <img alt="Vue logo" src="./assets/logo.png"> -->
  <HelloWorld msg="Bienvenido a tu app de Vue JS"/>
  <hr/>
  <BtnAccept></BtnAccept>
  <br>
  <BtnUpload></BtnUpload>
  <br>
  <BtnCustom></BtnCustom>
  <br>
  <BtnIcon></BtnIcon>
  <hr>
  <BtnText texto="Ingresar"></BtnText>
  <BtnText texto="Registrar"></BtnText>
  <BtnText texto="Salir"></BtnText>
  <hr>
  <FormText></FormText>
  <hr>
  <ChangeText></ChangeText>
  <hr>
  <ListHomeworks></ListHomeworks>
  <hr>
  <DataFetch></DataFetch>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import BtnAccept from './components/Boton1.vue'
import BtnUpload from './components/Boton2.vue'
import BtnCustom from './components/Boton3.vue'
import BtnIcon from './components/Boton4.vue'
import BtnText from './components/Boton5.vue'
import FormText from './components/FormText.vue'
import ChangeText from './components/ChangeText.vue'
import ListHomeworks from './components/ListHomeworks.vue'
import DataFetch from './components/DataFetch.vue'

export default {
  name: 'App',
  components: {
    HelloWorld,
    BtnAccept,
    BtnUpload,
    BtnCustom,
    BtnIcon,
    BtnText,
    FormText,
    ChangeText,
    ListHomeworks,
    DataFetch
  }
}
</script>

<style>
/* #app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
} */

@import './assets/css/style.css'
</style>
