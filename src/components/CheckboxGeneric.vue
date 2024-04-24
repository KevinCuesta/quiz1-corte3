<template>
  <ion-checkbox v-bind="$attrs" :id="id" :color="color" :disabled="disabled" :type="type">{{ value }}</ion-checkbox>
</template>

<script lang="ts">
import { IonCheckbox } from '@ionic/vue';
import { defineComponent } from 'vue';

export default defineComponent({
  components: { IonCheckbox },
  props: {
    id:{
      type: String,
      requiered: true
    },
    value: {
      type: String,
      required: true 
    },
    name: String,
    color: String,
    disable: Boolean,
    tpe: String 
  },
  data() {
    return {
      isChecked: false
    };
  }
});
</script>

