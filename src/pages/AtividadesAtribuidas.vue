<template>
  <q-page padding>
    <div class="text-h4 q-mb-md">Atribuidas</div>
    <q-list>
      <q-item v-for="lista in listas" :key="lista.id" clickable v-ripple class="shadow-2 q-mb-md">
        <q-item-section avatar>
          <q-icon color="primary" name="check" />
        </q-item-section>

        <q-item-section>{{lista.title}}</q-item-section>
      </q-item>
    </q-list>
  </q-page>
</template>

<script>
export default {
  name: 'Atribuidas',
  data () {
    return {
      listas: [

      ]
    }
  },
  methods: {
    loadList () {
      this.$axios.get('https://jsonplaceholder.typicode.com/todos')
        .then(respose => {
          this.listas = respose.data
        })
    }
  },
  beforeMount () {
    this.loadList()
  }
}
</script>
