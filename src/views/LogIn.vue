<template>
    <div>
        <div class="">
            <el-card shadow="hover">
                <div class="card-body">
                    <el-form ref="singData" :model="singData" label-position="top">
                        <!-- input correo -->
                        <el-form-item label="Correo" 
                            
                        >
                            <el-input v-model="singData.name" placeholder="Nombre"></el-input>
                        </el-form-item>
                        
                        <!-- input passsword -->
                        <el-form-item label="Contraseña"
                        >
                            <el-input v-model="singData.password" show-password placeholder="Contraseña"></el-input>
                        </el-form-item>
                    </el-form>
                </div>
            </el-card>
        </div>

    </div>
</template>

<script>
export default {
    data() {
        return {
            singData:{
                name:'',
                password:'',
            }
        }
    },
}
</script>

<style lang="stylus" scoped>
    body
        background black

    .card-body
        background-color red
</style>
