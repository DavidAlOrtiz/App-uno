<template>
    <div>
        <h2></h2>
        <ion-button @click="presentarAlerta()">Mostrar Alerta</ion-button>
    </div>
</template>

<script >
import {  IonButton, alertController } from '@ionic/vue';
import { defineComponent } from 'vue';
export default defineComponent({
    components: {IonButton},
    methods:{
        async presentarAlerta(){
            const alert = await alertController.create({
                cssClass:'my-custom-class',
                header:"Mensaje privado",
                subHeader:"Estas utilizando vue y ionic",
                message:"Esta es una aalerta ",
                buttons: ["ok"]
            });
            await alert.present();
            const {role} = await alert.onDidDismiss();
            console.log('onDidDissmis resolvio la alerta', role)
        }
    },
 
});
</script>

<style  scoped>
.my-custom-class{
    --background:#e5e5e5;
}
</style>