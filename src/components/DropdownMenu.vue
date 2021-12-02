<template>
  <q-btn label="Dropdown" color="teal">
    <q-menu>
      <q-card style="min-width: 300px;">
        <q-list>
          <q-item v-for="i in 5" :key="i">
            <q-item-section>
              <q-item-label>Item {{ i }}</q-item-label>
            </q-item-section>
          </q-item>
        </q-list>
      </q-card>
    </q-menu>
  </q-btn>
</template>

<script>
export default {
}
</script>
