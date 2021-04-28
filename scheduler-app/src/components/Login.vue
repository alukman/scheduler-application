<template>
   <div>
      <b-row>
         <b-col />
         <b-col>
            <b-input-group prepend="Username" class="inputBox">
               <b-form-input></b-form-input>
            </b-input-group>
            <b-input-group prepend="Password" class="inputBox">
               <b-form-input :type="passwordFieldType" v-model="password"></b-form-input>
               <b-button type="password" @click="switchVisibility"> Show/Hide</b-button>
            </b-input-group>
            <b-button>Login</b-button>
         </b-col>
         <b-col />
      </b-row>
   </div>
</template>

<script>
export default {
    data() {
        return {
            password: "",
            passwordFieldType: "password"
        };
    },
    methods: {
        switchVisibility() {
            this.passwordFieldType = this.passwordFieldType === "password" ? "text" : "password";
        }
    }
};
</script>

<style>
#inputBox {
    margin: 0 0 10px 0;
}
</style>