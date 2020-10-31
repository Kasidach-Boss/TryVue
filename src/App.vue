<template>
  <div class="container mt-4">
    
      <span> {{getFullName()}} </span>
    <div>
      This content is  in bootstrap's container
    </div>
    
    <button type="button" class="btn btn-primary">Primary</button>
    <button type="button" class="btn btn-secondary">Secondary</button>
    <button type="button" class="btn btn-success">Success</button>
    <button type="button" class="btn btn-danger">Danger</button>
    <button type="button" class="btn btn-warning">Warning</button>
    <button type="button" class="btn btn-info">Info</button>
    <button type="button" class="btn btn-light">Light</button>
    <button type="button" class="btn btn-dark">Dark</button>
    <button type="button" class="btn btn-link">Link</button>
    <button type="button" class="btn btn-secondary">
      <i class="fas fa-address-book"></i>
    </button>
    <button type="button" class="btn btn-success  btn-lg">Success</button>
    <div class="container">
      <div class="alert-success">คุณทำสำเร็จแล้ว</div>
      <div class="alert-warning">เอ๊ะ! มีอะไรแปลกๆ</div>
      <div class="alert-danger">นั่นอันตราย</div>
      <div class="alert-info">รายละเอียดของคุณ</div>
    </div>
    
  </div>
  

</template>

<script>
//import MyComponent from './components/MyComponent.vue'

export default {
  name: 'App',
  data() {
    return{
      MyName: "kASidach",
      MyLastName: "sangThong"
    };
  },
  methods: {
    getName() {
      return (
        this.MyName.charAt(0).toUpperCase()+ this.MyName.slice(1).toLowerCase()
      );
    },
    getLastName(){
      return(
        this.MyLastName.charAt(0).toUpperCase() + this.MyLastName.slice(1).toLowerCase()
      );
    },
    getFullName(){
      return `${this.getName()} ${this.getLastName()}`;
    }
  }
};
</script>

<style >

</style>
