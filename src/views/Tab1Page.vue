<template>
  <ion-page>
    <ion-header>
      <ion-toolbar>
        <ion-title>foto
        </ion-title>
      </ion-toolbar>
    </ion-header>
    <ion-content :fullscreen="true">
      <ion-fab vertical="buttom" horizontal="center" slot="fixed">

        <ion-fab-button @click="takePhoto()">


      <ion-tab-button tab="tab2" href="/tabs/tab2">
        <ion-icon :icon="camera" />
      </ion-tab-button>

        </ion-fab-button>
      </ion-fab>
    </ion-content>

      <!--<ExploreContainer name="Tab 1 page" />-->

  </ion-page>
</template>

<script setup lang="ts">
import { images, square, triangle } from 'ionicons/icons';
import {
  //IonPage,
  IonHeader,
  IonFab,
  IonFabButton,
  IonIcon,
  IonToolbar,
  IonTitle,
  IonContent,
  IonGrid,
  IonRow,
  IonCol,
  IonImg,
} from '@ionic/vue';
import { camera, trash, close } from 'ionicons/icons';
import { usePhotoGallery } from '../components/composables/usePhotoGalerry';

const { takePhoto } = usePhotoGallery();

//import ExploreContainer from '@/components/ExploreContainer.vue';
</script>
