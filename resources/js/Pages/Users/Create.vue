<template>
  <layout>
    <div class="container">
      <div class="col-md-6">
        <!-- <div v-if="Object.keys(errors).length > 0" class="alert alert-danger mt-4">
          {{ errors[Object.keys(errors)[0]][0] }}
        </div> -->

        <form action="/users" method="POST" class="my-5" @submit.prevent="createUser">
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
          <div class="form-group">
            <label for="password">Password</label>
            <input type="password" class="form-control" id="password" placeholder="Password" v-model="form.password">
            <div class="text-red-500" v-if="errors.password">{{ errors.password }}</div>
          </div>
          <br>
          <button type="submit" class=" bg-sky-500 btn btn-primary bg">Create User</button>
        </form>
      </div>
    </div>
  </layout>
</template>

<script>
    import Layout from '@/Shared/Layout'
    export default {
        props: {
            errors: Object,
        },
            
        components: {
                Layout,
        },
        data() {
            return {
                form: {
                    name: '',
                    email: '',
                    password: '',
                }
            }
        },
        methods: {
            createUser(){
                this.$inertia.post('/users', this.form)
                    // .then(() => {
                    //     //
                    // })
            }
        }
    }
</script>
