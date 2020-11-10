<template>
  <div class="container mt-4">
    
      <span> {{getFullName()}} </span>
    <div>
      <h3>This content is  in bootstrap's container</h3>
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
    <div class="container text-center">
      <div class="row">
        <div class="col border"> auto size </div>
        <div class="col border"> auto size </div>
        <div class="col border"> auto size </div>
      </div>
      <div class="row">
        <div class="col border"> auto size </div>
        <div class="col-2 border"> 2/12 size </div>
        <div class="col-6 border"> 6/12 size </div>
      </div>  
    <div class="card" style="width:18rem;" mt-3>
        <img class="card-img-top"
        src="https://cdn.pixabay.com/photo/2014/01/20/15/13/sheep-248632_1280.jpg"
        alt="Card image cap"/>
        <div class="card-body">
            <p class="card-text">This is a sheep.</p>
        </div>
    </div> 
      <div class="row d-block">
        <div class="alert-success">ข้อความนี้แสดงทุกอุปกรณ์</div>
      </div>  
      <div class="row d-none d-md-block">
        <div class="alert-danger">ข้อความนี้แสดงเฉพาะแท็บแล็ต</div>
      </div>

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
