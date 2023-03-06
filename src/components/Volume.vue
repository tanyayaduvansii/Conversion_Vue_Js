<template>
    <div class="container-fluid"  >
        <div class="row">
            <div class="col-6">
                <label class="form-label m-1">Enter Volume</label>
                <input type="text" class="form-control">
                <br>
                <select  class="form-control">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>liter</option>
                    <option>Mili Liter</option>
                </select>
                
            </div>
            <div class="col-6 ">
                <label class="form-label m-1">Result</label>
                <input type="text" class="form-control">
                <br>
                <select   class="form-control">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>liter</option>
                    <option>Mili Liter</option>
                </select>
            </div>
        </div>
    </div>
</template>
<script>
export default {
    data() {
         
    }
}
</script>
<style>
 
</style>