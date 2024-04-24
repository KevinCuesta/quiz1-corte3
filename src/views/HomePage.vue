<template>
  <ion-card class="custom-card">
    <ion-card-header>
      <ion-card-title>Crear Usuarios</ion-card-title>
      <ion-card-subtitle>by: kevin Cuesta</ion-card-subtitle>
    </ion-card-header>

    <ion-card-content>

      <InputGeneric id="nombreInput" name="nambe" type="text" placeholder="Ingrese su nombre"/>
      <InputGeneric id="fechaNacimientoInput" fechaNacimiento="date" type="date" placeholder="Seleccione su fecha de nacimiento"/>
      <InputGeneric id="celularInput" celular="tel" type="tel" placeholder="Ingrese su número de celular"/>
      <InputGeneric id="correoInput" correo="email" type="email" placeholder="Ingrese su correo electrónico"/>
      Recuerda Rellenar todos los datos
      <CheckboxGeneric checkboxText="Acepto los términos y condiciones" />
    </ion-card-content>
  </ion-card>
  <ion-card-content class="custom-button">
    <ButtonGeneric id="add" value="Agregar" fill="outline" />
      <ButtonGeneric id="update" value="Modificar" fill="outline" color="success"/>
      <ButtonGeneric id="delete" value="Elimnar" fill="outline" color="danger"/>
      <ButtonGeneric id="search" value="Consultar" fill="outline" color="medium"/>
  </ion-card-content>
 
</template>

<script setup lang="ts">
import {IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle } from '@ionic/vue';
import InputGeneric from '@/components/InputGeneric.vue';
import ButtonGeneric from '@/components/ButtonGeneric.vue';
import CheckboxGeneric from '@/components/CheckboxGeneric.vue';
</script>

<style scoped>
.custom-card {
  background-color: #f0f0f0; /* Color de fondo gris */
}
.custom-button {
  display: flex;
  flex-wrap: wrap;
  justify-content: center;
}

#container {
  text-align: center;
  
  position: absolute;
  left: 0;
  right: 0;
  top: 50%;
  transform: translateY(-50%);
}

#container strong {
  font-size: 20px;
  line-height: 26px;
}

#container p {
  font-size: 16px;
  line-height: 22px;
  
  color: #8c8c8c;
  
  margin: 0;
}

#container a {
  text-decoration: none;
}
</style>
