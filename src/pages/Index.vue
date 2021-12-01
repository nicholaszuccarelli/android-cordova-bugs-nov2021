<template>
  <q-page>
    <div class="container q-pa-md q-gutter-sm">
      <q-btn
        label="Open Sample Dialog"
        color="blue"
        @click="$refs.dialog.open()"
      />
      <template v-for="i in amountOfOptions">
        <QInputWithMenu v-if="i % 3 === 0" :key="i" />
        <QInputSimple v-else-if="i % 3 === 1" :key="i" />
        <ParagraphOfText v-else-if="i % 3 === 2" :key="i" />
      </template>
    </div>

    <QDialogSample ref="dialog" />
  </q-page>
</template>

<script>
import QInputWithMenu from 'components/QInputWithMenu'
import QInputSimple from 'components/QInputSimple'
import ParagraphOfText from 'components/ParagraphOfText'
import QDialogSample from 'components/QDialogSample'

export default {
  name: 'PageIndex',
  components: {
    QInputWithMenu, QInputSimple, ParagraphOfText, QDialogSample
  },
  data () {
    return {
      amountOfOptions: 50
    }
  }
}
</script>

<style lang="scss">
.container {
  margin: 0 auto;
  width: 100%;
  max-width: 700px;
}
</style>
