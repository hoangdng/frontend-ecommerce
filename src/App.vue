<template>
  <q-layout view="hHh lpR fFf">
    <q-header class="bg-primary text-white" elevated height-hint="98">
      <div class="flex justify-between q-px-lg q-py-sm">
        <q-avatar>
          <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg" />
        </q-avatar>
        <q-tabs align="left">
          <q-route-tab label="Page One" to="/page1" />
          <q-route-tab label="Page Two" to="/page2" />
          <q-route-tab label="Page Three" to="/page3" />
        </q-tabs>
      </div>
    </q-header>

    <q-page-container>
      <router-view />
    </q-page-container>

    <q-footer class="bg-grey-8 text-white" elevated>
      <q-toolbar>
        <q-toolbar-title>
          <q-avatar>
            <img src="https://cdn.quasar.dev/logo-v2/svg/logo-mono-white.svg" />
          </q-avatar>
          <div>Title</div>
        </q-toolbar-title>
      </q-toolbar>
    </q-footer>
  </q-layout>
</template>

<script>
export default {
  name: "DefaultLayout"
};
</script>
