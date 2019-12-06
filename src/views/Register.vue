<template>
    <div>
        <div class="card-cont">
            <el-card shadow="hover">
                <div class="app_title card-title">
                    <h2>Crea una cuenta</h2>
                </div>
                <div class="card-body">
                    <el-form ref="registerData" :model="registerData" >
                        <!-- input correo -->
                        <el-form-item  
                        >
                            <el-input v-model="registerData.name" placeholder="Nombre"></el-input>
                        </el-form-item>
                        
                        <!-- input passsword -->
                        <el-form-item 
                        >
                            <el-input v-model="registerData.password" show-password placeholder="Contraseña"></el-input>
                        </el-form-item>

                        <div class="action_form">
                            <el-button type="primary" @click="register()">Primary</el-button>
                        </div>
                        
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
            registerData:{
                name:'',
                password:'',
            }
        }
    },
    methods:{
        register(){
            if(registerData.name && registerData.password){
                
            }
            else{
                console.log(
                    "todos los campos son requeridos"
                )   
            }
        }
    }
}
</script>

<style lang="stylus" >
    @import'../Stylus/main.styl'
    .app_title
        font-family myriad-bold
        font-size 1.5em
        padding 20px 0
        display flex
        justify-content center
        align-items center
        h2
            font-weight 400
    .card-cont
        background-color base_color
        height 100vh
        display flex
        justify-content center
        align-items center
    .el-card
        flex 0 0 35%
    .action_form
        display flex
        justify-content center
        .el-button
            width 100%
            padding: 15px 0;

</style>
