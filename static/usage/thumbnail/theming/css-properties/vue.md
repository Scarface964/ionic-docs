```html
<style>
  ion-thumbnail {
    --size: 140px;
    --border-radius: 14px;
  }
</style>

<template>
  <ion-thumbnail>
    <img alt="Silhouette of mountains" src="https://ionicframework.com/docs/demos/api/thumbnail/thumbnail.svg" />
  </ion-thumbnail>
</template>

<script lang="ts">
  import { IonThumbnail } from '@ionic/vue';
  import { defineComponent } from 'vue';

  export default defineComponent({
    components: { IonThumbnail },
  });
</script>
```
