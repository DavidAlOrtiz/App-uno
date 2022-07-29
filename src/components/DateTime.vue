<template>
  <ion-item>
    <ion-label>MMMM</ion-label>
    <ion-datetime
      display-format="MMMM"
      value="2012-12-15T13:47:20.789"
    ></ion-datetime>
  </ion-item>

  <ion-item>
    <ion-label>D MMM YYYY H:mm</ion-label>
    <ion-datetime
      display-format="D MMM YYYY H:mm"
      min="1997"
      max="2010"
      value="2005-06-17T11:06Z"
    ></ion-datetime>
  </ion-item>
  <ion-item>
    <ion-label>Specific days/months/years</ion-label>
    <ion-datetime
      month-values="6,7,8"
      year-values="2014,2015"
      day-values="01,02,03,04,05,06,08,09,10, 11, 12, 13, 14"
      display-format="DD/MMM/YYYY"
    ></ion-datetime>
  </ion-item>
</template>

<script>
import { IonDatetime, IonItem, IonLabel } from "@ionic/vue";
export default({
  components: { IonDatetime, IonItem, IonLabel},
});
</script>

<style>
</style>