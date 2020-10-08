<template>
  <q-page padding class="flex flex-center row">
    <div class="row col-12">
      <q-card bordered class="my-card bg-orange-1 offset-1 col-10">
      <q-card-section>
        <div class="row items-center no-wrap">
          <div class="col-12">
            <div class="text-h6 flex flex-center">TodoList - Login</div>
          </div>
        </div>
      </q-card-section>

      <q-card-section>
        <div class="row">
          <div class="col-10">
            <q-input type="email" filled outlined label="Informe seu email:"></q-input>
          </div>
          <div class="col-2 q-mt-sm text-center">
            <q-btn round color="primary"  icon="send"/>
          </div>
        </div>
        <div class="text-right col-12">
          <div class="text-center q-mt-xl">ou</div>
          <div class=" text-primary text-subtitle1 text-center">
            <q-btn flat to="/controle/sign-up">Cadastre-se</q-btn>
          </div>
        </div>
      </q-card-section>
    </q-card>
    </div>
  </q-page>
</template>

<script>
export default {
  // name: 'PageName',
}
</script>
