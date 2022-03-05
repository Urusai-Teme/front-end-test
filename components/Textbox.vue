<template>
<div id="textboxWrapper" class="col-lg-12 control-section">
    <div class="textbox-label"> Two-way binding</div>
    <div class="col-lg-6">
        <div id="wrapper">
            <ejs-textbox floatLabelType="Auto" placeholder="Enter a value" v-model="value"></ejs-textbox>
        </div>
    </div> 
    <div class="col-lg-6">
        <div id="wrapper">
            <ejs-textbox floatLabelType="Auto" placeholder="Enter a value" v-model="value"></ejs-textbox>
        </div>
    </div>

</div>
</template>

<style scoped>
    #wrapper {
    max-width: 246px;
    margin: 30px auto;
    padding-top: 15px;
    }

    #textboxWrapper .textbox-label {
    text-align: center;
    width: 200px;
    margin: 0 auto;
    font-size: 14px;
    user-select: none;
    font-weight: 500;
    font-family: "Roboto", "Segoe UI", "GeezaPro", "DejaVu Serif", "sans-serif",
        "-apple-system", "BlinkMacSystemFont";
    }
</style>


<script>
import Vue from "vue";
import { TextBoxPlugin } from '@syncfusion/ej2-vue-inputs';
Vue.use(TextBoxPlugin);

export default Vue.extend({
    data: function() {
        return {
            value: null
         }
    }
});

</script>