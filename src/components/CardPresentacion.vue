<template>
    <ion-card>
        <ion-card-header>
            <ion-card-subtitle>Diseño UI aionic</ion-card-subtitle>
            <ion-card-title>Curso de aplicaciones hibridas</ion-card-title>
        </ion-card-header>

        <ion-card-content>
            Diseño de apps Hibirdas desarrolladas con vue ionic ademas de otros elementos de tecnologias
            para backend
        </ion-card-content>
    </ion-card>
</template>

<script>
import { IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle } from '@ionic/vue';
// pin, walk, warning, wifi, wine
import {  warning } from 'ionicons/icons';
import { defineComponent } from 'vue';

export default defineComponent({
    // IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle, 
    // IonIcon, IonItem, IonLabel
    components: { IonCard, IonCardContent, IonCardHeader, IonCardSubtitle, IonCardTitle, },
    setup() {
        return { warning };
    }
});
</script>

<style lang="scss" scoped>
</style>