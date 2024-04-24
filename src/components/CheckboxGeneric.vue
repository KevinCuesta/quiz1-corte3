<template>
  <ion-checkbox v-model="isChecked">{{ checkboxText }}</ion-checkbox>
</template>

<script lang="ts">
import { IonCheckbox } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  components: { IonCheckbox },
  props: {
    checkboxText: {
      type: String,
      required: true 
    }
  },
  data() {
    return {
      isChecked: false
    };
  }
});
</script>

