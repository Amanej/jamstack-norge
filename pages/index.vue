<template>
<div class="Aligner">
  <div class="Aligner-item">
      <JamstackLogo />
      <p>Her vil det komme en blogg og samleside for <br/>JamStack tilnærmingen til webutvikling i Norge og på norsk.</p>
  </div>
</div>
</template>

<script>
import JamstackLogo from '~/components/JamStackLogo'
export default {
    layout: 'noHeader',
    components: {
        JamstackLogo
    }
}
</script>

<style lang="scss" scoped>
.Aligner {
    display: flex;
    align-items: center;
    min-height: 24em;
    justify-content: center;
    height: 100vh;
    text-align: center;
    div.Aligner-item {
        flex: 1;
        p {
            padding: 20px;
        }
    }
}

</style>