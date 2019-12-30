<template>
<Layout>
    <br><br>
   
    <v-container>
    <v-row>
      <v-icon color="teal" size="40">mdi-briefcase-upload</v-icon>
    <h2 class="primary--text">{{ title }} </h2>
     
         
    </v-row>
    <ul v-for="(n,i) in items" :key="i" class="services">
                <li> <span style="text-indent: 30px;">
                  {{itemsList[0].price}} - </span>
                  {{ n }} 
                </li>
              </ul>
              <br>
              <hr>
              <br>
               <h2 class="text-center primary--text">
     الإحترافية - السرعة - الدقة - أسعار في المتناول
   </h2>
   
    </v-container>
 </Layout>
</template>

<script>


  export default {
    data () {
      return {
        title: 'الخدمات',
        itemsList: [
          { name:'المشتريات', price: '100 دولار أمريكى / شهر', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},
          { name: '', price: '', text: ''},

        ],
         items: [
        'المشتريات',
        'مراقبة المخزون',
        'إصدار فواتير العملاء',
        'المحاسبة',
        'إدارة النقد والحسابات البنكية',
        'إصدار القوائم المالية',
        'التقارير الإدارية',
        'الموازنات التقديرية',
        'دراسات جدوى المشروعات',
        'المرتبات',
        'مؤشرات قياس الأداء',
        'الإجراءات والسياسات'
      ]
       
      
      }
    },
    components: {
    
    }
  }
</script>