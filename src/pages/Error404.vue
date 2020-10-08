<template>
  <div class="fullscreen bg-blue text-white text-center q-pa-md flex flex-center">
    <div>
      <div style="font-size: 20vh">
        404
      </div>

      <div class="text-h2" style="opacity:.4">
        <h4>Eitxa bixiga, alguém errou alguma coisa.</h4>
        <h5>Tente outra página que tentaremos melhorar daqui.</h5>
      </div>

      <q-btn
        class="q-mt-xl"
        color="white"
        text-color="blue"
        unelevated
        to="/"
        label="Go Home"
        no-caps
      />
    </div>
  </div>
</template>

<script>
export default {
  name: 'Error404'
}
</script>
