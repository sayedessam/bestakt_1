<template>
<Layout>
    <br><br>
    <!-- <logo style="fill: teal; width: 50;" /> -->
    <v-container>
    <v-row>
      <v-icon color="teal" size="40">mdi-speedometer</v-icon>
    <h2 class="primary--text">{{ title }} </h2>
    </v-row>
    <p>
      إتجاهات الإيرادات عن عام 2019م
    </p>
    <g-image src="~/assets/img/Chart1.png" width="560%"></g-image>
    </v-container>
 </Layout>
</template>

<script>

import Logo from '~/components/Logo.vue'
  export default {
    data () {
      return {
        title: 'مؤشرات قياس الآداء',
        right: null,
      }
    },
    components: {
      Logo
    }
  }
</script>