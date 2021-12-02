<template>
  <q-layout view="lHh Lpr lFf">
    <q-header elevated>
      <q-toolbar>
        <DropdownMenu />

        <q-toolbar-title>
          Quasar App
        </q-toolbar-title>

        <div>Quasar v{{ $q.version }}</div>
        <DropdownMenu />
      </q-toolbar>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer>
      <q-toolbar>
        <DropdownMenu />
        <q-space />
        <DropdownMenu />
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>
import DropdownMenu from 'components/DropdownMenu'
export default {
  name: 'MainLayout',
  components: {
    DropdownMenu
  }
}
</script>
