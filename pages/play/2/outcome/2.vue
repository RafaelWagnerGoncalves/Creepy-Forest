<template>
    <div>
        <BadEnding :title="['b. Pega o bilhete e foge para bem longe','> O homem lhe alcançou enquanto você tentava pegar o bilhete e lhe acertou uma marretada. Você morreu.']"/>
    </div>
</template>

<script>
import BadEnding from '../../../../src/components/BadEnding.vue'

export default {

  components: {
    BadEnding,

  },
}
</script>

<style>

</style>