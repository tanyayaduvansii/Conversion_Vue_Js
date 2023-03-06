<template>
    <div class="container-fluid">
        <div class="row">
            <div class="col-6 ">
                <label class="form-label m-1">Enter Area</label>
                <input type="text" class="form-control" v-model="val" placeholder="Enter Value.....">
                <br>
                <select class="form-control" @change="get_area"  v-model="type">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>Square Kilometer</option>
                    <option>Square Meter</option>
                    <option>Square Mile</option>
                    <option>Square foot</option>
                    <option>Hectare</option>
                </select>

            </div>
            <div class="col-6 ">
                <label class="form-label m-1">Result</label>
                <input type="text" class="form-control" placeholder="Result..... " :value="result" >
                <br>
                <select class="form-control" v-model="res" @change="get_area" >
                    <option value="default" placeholder="select "  selected>Select Category</option>
                    <option  >Square Kilometer</option>
                    <option  >Square Meter</option>
                    <option  >Square Mile</option>
                    <option  >Square foot</option>
                    <option  >Hectare</option>
                </select>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
        return {
            val: '',
            result:''
        }
    },
    methods: {
        get_area() {
            if(this.type == "Square Kilometer" && this.res =="Square Meter" ){
                 this.result = this.val*100000;
                console.log("***8", this.result)
                console.log("***8",this.val)
            }
             
            
        }
    }
}
</script>
<style></style>