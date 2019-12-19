<template>
  <div id="app">
      <app-navbar/>
   <hello-world/>
      <loading :active.sync="visible" :can-cancel="true">

      </loading>

      <button @click.prevent="open()">Programmatic show</button>
      <button @click.prevent="show()">Component show, cancellable</button>



  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Navabar from './layout/Navabar'
import Loading from 'vue-loading-overlay';
import 'vue-loading-overlay/dist/vue-loading.css';

export default {
  name: 'app',
  components: {
    HelloWorld,
   'app-navbar': Navabar,
      Loading
  },
    data(){
      return{
          visible: false

      }
    },
    methods: {

        open() {
            // console.log('open was clicked, will auto hide');
            let loader = this.$loading.show({
                loader: 'dots'
            });
            setTimeout(() => loader.hide(), 3 * 1000)
        },
        show() {
            // console.log('show was clicked, click to hide');
            // do AJAX here
            this.visible = true
        }

  }
}
</script>

<style>



</style>
