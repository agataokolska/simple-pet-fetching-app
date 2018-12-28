<template>
    <v-card class="dog-card">
        <v-img
                height="150px"
                :src="dog"></v-img>
        <v-card-actions>
            <v-spacer></v-spacer>
            <v-btn @click="$emit('remove')" icon>
                <v-icon>delete</v-icon>
            </v-btn>
        </v-card-actions>
    </v-card>
</template>

<script>
    export default {
        name: "Dog",
        props: {
            dog: {
                type: String
            }
        }
    }
</script>

<style scoped>

</style>
