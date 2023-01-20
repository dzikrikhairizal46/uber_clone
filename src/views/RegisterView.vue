<template>
    <div class="w-full max-w-sm mx-auto">
      <form @submit.prevent="handleRegister" class="bg-white rounded-lg p-6">
        <h2 class="text-lg font-medium mb-4">Register</h2>
        <div class="mb-4">
          <label class="block text-gray-700 font-medium mb-2">Name</label>
          <input v-model="name" class="w-full border border-gray-400 rounded-lg p-2" type="text" placeholder="John Doe" />
        </div>
        <div class="my-4">
            <label class="block text-gray-700 font-medium mb-2">Email</label>
            <input v-model="email" class="w-full border border-gray-400 rounded-lg p-2" type="email" placeholder="example@mail.com" />
        </div>
        <div class="my-4">
            <label class="block text-gray-700 font-medium mb-2">Password</label>
            <input v-model="password" class="w-full border border-gray-400 rounded-lg p-2" type="password" placeholder="********" />
        </div>
        <div class="my-4">
            <label class="block text-gray-700 font-medium mb-2">Confirm Password</label>
            <input v-model="password_confirmation" class="w-full border border-gray-400 rounded-lg p-2" type="password" placeholder="********" />
        </div>
        <div class="my-4">
            <button class="bg-black text-white py-2 px-4 rounded-lg hover:bg-gray-800">Register</button>
        </div>
        </form>
    </div>
</template>
    <script>
    export default {
        data() {
            return {
            name: '',
            email: '',
            password: '',
            password_confirmation: '',
            }
        },
        methods: {
            submitForm() {
            // handle form submission logic here
            }
        }
    }
    </script>
<style scoped>
.container {
  max-width: 400px;
  margin: 0 auto;
  padding: 2rem;
  background-color: #fff;
  border-radius: 1rem;
}
</style>