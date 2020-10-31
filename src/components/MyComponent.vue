<template>
    <div id="content">
        <h1>This is my first component</h1>
        <p>Hello My name is{{mypropertyName}} </p>
    </div>
</template>
<script>
export default {
    name: "MyComponent",
    data() {
        return{
            mypropertyName: " Kasidach"
        };
    }
};
</script>
<style>
#content {
    text-align: center;
    color: blue;
}
</style>