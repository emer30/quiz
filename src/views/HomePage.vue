<template>
  <ion-page>
  

    <ion-content  :fullscreen="true" >
      <ion-header collapse="condense">
        <ion-toolbar>
          <ion-title size="large"></ion-title>
        </ion-toolbar>
      </ion-header>
      <div id="login-container">
        
      
        <div id="description">
          <h1>¡BIENVENIDO! </h1>
          <p> Por favor ingrese sus datos o relice la acción que desea.</p>
        </div>
        <div id="login-form">
          <InputGeneric id="nombre" value="emerson" label="nombre: " type="text" />
          <InputGeneric id="fecha" type="date" label="fecha de nacimiento: " />
          <InputGeneric id="celular"  value="3209886223" type="text" label="number: " />
          <InputGeneric id="correo" value="ingrese correo" type="text" label="correo: " />
    
         </div>

        <div>
          <ButtonGeneric id="btnAgregar" value="Agregar" />
          <ButtonGeneric id="btnModificar" value="Modificar" />
          <ButtonGeneric id="btnEliminar" color="danger" value="Eliminar" />
          <ButtonGeneric id="btnConsultar" value="Consultar" />
        </div>
             </div>

    </ion-content>
  </ion-page>
  <CardGeneric id = "mensaje" value = "APERTURA DE CLIENTES" subtitulo="CLIENTES"  header = "Cabeza"></CardGeneric>

</template>

<script setup lang="ts">
import { IonContent, IonHeader, IonPage, IonTitle, IonToolbar } from '@ionic/vue';
import InputGeneric from '@/components/InputGeneric.vue';
import ButtonGeneric from '@/components/ButtonGeneric.vue';
import CardGeneric from '@/components/CardGeneric.vue';
</script>

<style scoped>
#login-container {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  height: 100%;
}


#cart-image {
  margin-bottom: 20px;
  width: 100px;
}

#description {
  margin-bottom: 20px;
  text-align: center;
}

#description p {
  margin: 0;
  padding: 10px; 
}

#login-form {
  max-width: 300px;
  width: 100%;
}
</style>
