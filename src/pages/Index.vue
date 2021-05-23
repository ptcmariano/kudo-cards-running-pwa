<template>
  <q-page class="flex flex-center">
    <q-card class="my-card">
      <q-toolbar class="bg-blue text-white shadow-2 rounded-borders flex-center">
        <div class="text-h6">Wellcome, {{username}}</div>
      </q-toolbar>
      <q-input filled v-model="username" label="Your name"></q-input>
      <q-card-actions vertical>
        <q-btn flat class="bg-green" @click="enterKudoSession">Enter</q-btn>
      </q-card-actions>
    </q-card>
  </q-page>
</template>

<script>
export default {
  data: () => {
    return {
      username: 'Participant'
    }
  },
  methods: {
    enterKudoSession: () => {
      alert('enter...')
    }
  },
  name: 'PageIndex'
}
</script>
