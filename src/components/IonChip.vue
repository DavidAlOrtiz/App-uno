<template>
    <ion-chip color="primary">
        <ion-label>Inicial</ion-label>
    </ion-chip>

    <ion-chip>
        <ion-avatar>
            <img src="https://gravatar.com/avatar/dba6bae8c566f9d4041fb9cd9ada7741?d=identicon&f=y">
        </ion-avatar>
        <ion-label>Tu avatarr</ion-label>
        <ion-icon :icon="closeCircle"></ion-icon>
    </ion-chip>
    <ion-chip>
        <ion-icon :icon="heart" color="dark"></ion-icon>
        <ion-label>Default</ion-label>
    </ion-chip>
</template>

<script>
import { IonAvatar, IonChip, IonIcon, IonLabel } from '@ionic/vue';
import { close, closeCircle, heart, pin } from 'ionicons/icons';

import { defineComponent } from 'vue';

export default defineComponent({
    components: { IonAvatar, IonChip, IonIcon, IonLabel },
    setup() {
        return { close, closeCircle, heart, pin }
    }
});
</script>

<style>
</style>