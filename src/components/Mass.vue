<template>
    <div class="container-fluid"  >
        <div class="row">
            <div class="col-6">
                <label class="form-label m-1">Enter Mass </label>
                <input type="text" class="form-control">
                <br>
                <select   class="form-control">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>Kilogram</option>
                    <option>Gram</option>
                    <option>Miligram</option>
                    <option>Tone</option>
                </select>
            </div>
            <div class="col-6 ">
                <label class="form-label m-1">Result</label>
                <input type="text" class="form-control">
                <br>
                <select  class="form-control">
                    <option value="default" placeholder="select " selected>Select Category</option>
                    <option>Kilogram</option>
                    <option>Gram</option>
                    <option>Miligram</option>
                    <option>Tone</option>
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