<template>
  <layout>
    <div class="container">
      <div class="col-md-6">
        <!-- <div v-if="Object.keys(errors).length > 0" class="alert alert-danger mt-4">
          {{ errors[Object.keys(errors)[0]][0] }}
        </div> -->

        <form action="#" method="PATCH" class="my-5" @submit.prevent="updateUser">
          <div class="form-group">
            <label for="name">Name</label>
            <input type="text" class="form-control" id="name" placeholder="Name" v-model="form.name">
            <div class="text-red-500" v-if="errors.name">{{ errors.name }}</div>
          </div>
          <br>
          <div class="form-group">
            <label for="email">Email</label>
            <input type="email" class="form-control" id="email" placeholder="Email" v-model="form.email">
            <div class="text-red-500" v-if="errors.email">{{ errors.email }}</div>
          </div>
          <br>
          <button type="submit" class=" bg-sky-500 btn btn-primary pr-4 ">Edit User</button>
        </form>

        
          <button @click="deleteUser" class="btn btn-danger px-8 "> Delete User </button>
      </div>
    </div>
  </layout>
</template>

<script>
    import Layout from '@/Shared/Layout'
    export default {
        props: [
            "errors", 'user'
        ],
            
        components: {
                Layout,
        },
        data() {
            return {
                loading: false,
                form: {
                    name: this.user.name,
                    email: this.user.email,
                }
            }
        },
        methods: {
            updateUser(){
                this.$inertia.patch(`/users/${this.user.id}`, this.form)
                    // .then(() => {
                    //     this.loading = false;
                    // })
            },
            deleteUser(){
                if (confirm('Are you sure you want to delete this user?')){
                    this.$inertia.delete(`/users/${this.user.id}`)
                }
            }
        }
    }
</script>
