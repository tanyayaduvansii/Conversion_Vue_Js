<template>
    <div class="container-fluid"  >
        <div class="row">
            <div class="col-6">
                <label class="form-label m-1">Enter Speed</label>
                <input type="text" class="form-control">
                <br>
                <select   class="form-control">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>Mile Per Hour</option>
                    <option>Foot Per Second</option>
                    <option>Meter Per Second</option>
                    <option>KiloMeter Per Second</option>
            
                </select>
                
            </div>
            <div class="col-6 ">
                <label class="form-label m-1">Result</label>
                <input type="text" class="form-control">
                <br>
                <select  class="form-control">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>Mile Per Hour</option>
                    <option>Foot Per Second</option>
                    <option>Meter Per Second</option>
                    <option>KiloMeter Per Second</option>
            
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