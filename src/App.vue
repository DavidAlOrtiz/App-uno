<template>
  <ion-app>
    <ion-menu side="start" menu-id="first" content-id="main">
      <ion-header>
        <ion-toolbar color="primary">
          <ion-title>Menu personalisado</ion-title>
        </ion-toolbar>
      </ion-header>
      <ion-content>
        <ion-list>
          <ion-item>Archivos</ion-item>
          <ion-item>Fotos</ion-item>
          <ion-item>Red social</ion-item>
          <ion-item>Tus preferencias</ion-item>
          <ion-item>Mis contactos</ion-item>
        </ion-list>
      </ion-content>
    </ion-menu>

    
    <ion-router-outlet id="main"/>
  </ion-app>
</template>

<script >
import { IonApp, IonRouterOutlet,IonMenu,IonHeader,IonTitle,IonToolbar,IonItem, IonList, IonContent, } from "@ionic/vue";
import { defineComponent } from "vue";

export default defineComponent({
  name: "App",
  components: {
    IonApp,
    IonRouterOutlet,
    IonMenu,
    IonHeader,
    IonTitle,
    IonToolbar,
    IonItem,
    IonList, 
    IonContent
    
  },
});
</script>