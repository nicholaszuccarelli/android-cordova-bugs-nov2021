<template>
  <q-input
    v-model="value"
    dense
    autogrow
    outlined
    label="Enter value or select from dropdown"
  >
    <template v-slot:append>
      <q-icon name="mdi-menu-down" />
    </template>

    <q-menu
      no-refocus
      no-focus
      fit
    >
      <q-list dense>
        <q-item v-for="(item, key) in menuItems" :key="key" clickable @click="value = item">
          <q-item-section>
            <q-item-label>
              {{ item }}
            </q-item-label>
          </q-item-section>
        </q-item>
      </q-list>
    </q-menu>
  </q-input>
</template>

<script>
export default {
  data () {
    return {
      value: '',
      menuItems: [
        'Item 1',
        'Item 2',
        'Item 3',
        'Item 4'
      ]
    }
  }
}
</script>
