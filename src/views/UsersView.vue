<template>
    <div>
        <h1>welcome from {{logo}}</h1>
        <div v-for="user in users" :key="user.id">
            <h1 class="name">{{ user.na }}</h1><br>
            <h2 class="age">{{ user.age }}</h2><br><br><br>
        </div>
    </div>
</template>

<script>
export default {
    name: "UsersView",
    data() {
        return {
            users:[
                {id:1 ,na:"kareem",age:22},
                {id:2 ,na:"omar",age:32},
                {id:3 ,na:"seif",age:13}
            ],
            logo:"welcome"
        }
    },
}
</script>