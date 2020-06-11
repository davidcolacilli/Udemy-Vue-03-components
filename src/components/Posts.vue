<template>
    <table class="table table-dark">
        <thead>
            <tr>
                <th scope="col">ID</th>
                <th scope="col">User</th>
                <th scope="col">Message</th>
            </tr>
        </thead>
        <tbody>
            <tr v-for="post in posts" :key="post.id">
                <th scope="row">{{post.id}}</th>
                <td>{{post.user}}</td>
                <td>{{post.message}}</td>
            </tr>
        </tbody>
    </table>
</template>
<script>

export default {
    name: "Posts",
    props: {},
    data() {
        return {
            posts: [
                {
                    id: 1,
                    user: "Juan",
                    message: "First kick"
                },
                {
                    id: 2,
                    user: "Pedro",
                    message: "Ouch!"
                },
                {
                    id: 3,
                    user: "Chuck",
                    message: "There's no third kick ;)"
                }

            ]
        }
    }
}
</script>
<style scoped>

</style>