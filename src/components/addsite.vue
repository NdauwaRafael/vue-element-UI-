<template>
    <el-main>
        <el-form ref="form" :model="siteFrm"  size="medium">
            <el-form-item label="Service name">
                <el-input v-model="siteFrm.name"></el-input>
            </el-form-item>

            <el-form-item label="Service Location">
                <el-input v-model="siteFrm.location"></el-input>
            </el-form-item>

            <el-form-item label="Service Category">
                <el-input v-model="siteFrm.category"></el-input>
            </el-form-item>

            <el-form-item label="Service Description">
                <el-input type="textarea" v-model="siteFrm.desc"></el-input>
            </el-form-item>

            <el-form-item>
                <el-button type="success">Register service</el-button>
            </el-form-item>

        </el-form>
    </el-main>
</template>

<script>
    import ElFormItem from "../../node_modules/element-ui/packages/form/src/form-item.vue";

    export default {
        components: {ElFormItem},
        data() {
            return {
                siteFrm: {
                    name: '',
                    location: '',
                    category: '',
                    desc: ''


                }
            };
        },
        methods: {
            onSubmit() {
                console.log('submit!');
            }
        }
    };
</script>

<style>

</style>