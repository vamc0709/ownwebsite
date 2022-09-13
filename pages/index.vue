<template>
    <div class="title">
    <!-- <h1>Log App</h1> -->
    <div class="login-page">
      <form @submit.prevent="login">
        <p class="title-1">Email :</p>
        <input
          type="email"
          v-model="email"
          placeholder="Enter email"
          required
        /><br /><br />
        <p class="title-2">Password :</p>
        <input
          type="password"
          v-model="password"
          placeholder="Enter password"
          required
        />
        <br /><br />
        <button class="button" type="submit" @click="login">
          Login
        </button>
      </form>
    </div>
      <!-- <div class="modal">
        <h1 class="modal_title">Allow notifications</h1>
        <div class="modal_actions">
          <a href="#" class="modal_action">Allow</a>
          <button class="modal_action modal_action--negative" type="button">
            Block
          </button>
        </div> -->
      <!-- </div> -->
    
  </div>

  <!-- <el-form :label-position="labelPosition" label-width="100px" :model="formLabelAlign">
  <el-form-item label="Name">
    <el-input v-model="formLabelAlign.name"></el-input>
  </el-form-item>
  </el-form>-->
</template> 

<script>
export default {
    data() {
    return {
      email: '',
      password: '',
      formLabelAlign: {
        name: ''
      }
}
    }
//     data() {
//       return {
//         labelPosition: 'right',
//       };
//     }
  }
</script>

<style>
/* @import url("//unpkg.com/element-ui@2.15.8/lib/theme-chalk/index.css");
.el-form{
    background-color: black;
} */
</style>