<template>
  <q-dialog
    v-model="dialogOpen"
  >
    <q-card>
      <q-toolbar>
        <q-toolbar-title>Sample Dialog.</q-toolbar-title>
      </q-toolbar>
      <div class="q-gutter-md q-pa-md">
        <div>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Accusantium aliquam consectetur culpa et excepturi
          facilis fugiat fugit labore magnam necessitatibus numquam, odit quibusdam rem, repellat sequi similique soluta
          suscipit voluptatem?
        </div>
        <div>A accusamus accusantium aliquam aperiam assumenda, commodi consectetur cum doloremque eligendi enim est
          excepturi facilis illo iste iusto natus neque officia qui quidem quod reiciendis sapiente sed! Cum, inventore,
          soluta.
        </div>
        <QInputSimple />
        <div>Beatae dolor labore nam. Ad aspernatur corporis dignissimos et eum fuga ipsam iste, laborum laudantium natus,
          nemo obcaecati provident quae quaerat quas quisquam ratione reprehenderit sint temporibus voluptatem! Quaerat,
          ullam?
        </div>
        <div>Aliquam aliquid consectetur, consequatur cupiditate delectus deleniti deserunt distinctio et ex explicabo fugit
          incidunt, inventore itaque iusto labore magni molestias mollitia numquam porro quibusdam recusandae rem
          repellendus repudiandae rerum voluptas.
        </div>
        <QInputWithMenu />
        <div>Adipisci architecto earum error facilis iusto magnam magni quasi tempora temporibus totam. Assumenda enim
          excepturi exercitationem harum illum, recusandae ut. Animi labore nisi non nostrum officia quisquam ratione sit
          voluptatem.
        </div>
      </div>
      <q-toolbar>
        <q-space />
        <q-btn
          v-close-popup
          label="Close"
          color="blue"
        />
      </q-toolbar>
    </q-card>
  </q-dialog>
</template>

<script>
import QInputWithMenu from 'components/QInputWithMenu'
import QInputSimple from 'components/QInputSimple'

export default {
  components: {
    QInputSimple, QInputWithMenu
  },
  data () {
    return {
      dialogOpen: false
    }
  },
  methods: {
    open () {
      this.dialogOpen = true
    }
  }
}
</script>
