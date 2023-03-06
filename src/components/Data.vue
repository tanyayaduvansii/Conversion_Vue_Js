<template>
    <div class="container-fluid "  >
        <div class="row">
            <div class="col-6">
                <label class="form-label m-1">Enter Data</label>
                <input type="text" class="form-control">
                <br>
                <select  class="form-control">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>Bit Per Second</option>
                    <option>kiloyte Per Second</option>
                    <option>MegaByte Per Second</option>
                    <option>GegaByte Per Second</option>
                    <option>TeraByte Per Second</option>
                </select>
                
            </div>
            <div class="col-6 ">
                <label class="form-label m-1">Result</label>
                <input type="text" class="form-control">
                <br>
                <select class="form-control">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>Bit Per Second</option>
                    <option>kiloyte Per Second</option>
                    <option>MegaByte Per Second</option>
                    <option>GegaByte Per Second</option>
                    <option>TeraByte Per Second</option>
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