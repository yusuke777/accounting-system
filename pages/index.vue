<template>
   <div class="app">
      <h1 class="label">ログインページ</h1>
      <p>下のログインボタンを押してください</p>
      <v-btn @click="pushButtun">ログインボタン</v-btn>
   </div>
</template>

<script>
import firebase from '~/utillis/firebase';

export default {
   components: {

   },
   props: {
      hoge: {
         type: Array,
         default: () => []
      }
   },
   data() {
      return {
         
      };
   },
   computed: {
      
   },
   methods: {
      pushButtun(){
         const provider = new firebase.auth.GoogleAuthProvider();
         firebase.auth().signInWithPopup(provider).then((result) => {
            this.$router.push('/mypage');
            this.$toasted.
         });
      }
   }
}
</script>

<style scoped>
.label {
   margin-bottom: 50px;
}

.app {
  display: flex;
  flex-direction: column;
  align-items: center;
}
</style>