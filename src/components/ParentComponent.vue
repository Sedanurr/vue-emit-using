<template>
 <ChildComponent @addCats="addCats"></ChildComponent> 
  <div>
    Sepet: {{ countOfItem }}
  </div>
</template>
<script>
import ChildComponent from './ChildComponent.vue';
export default(
{
    data() {
        return {
            countOfItem:0
        }
    },
    components: {
        ChildComponent
    },
    methods: {
       addCats() {
        this.countOfItem += 1
       }
    }

})
</script>
<style>
.clickedStyle{
    color:pink;
    background-color: aqua;
}
</style>