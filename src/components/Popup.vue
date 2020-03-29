<template>
<div>


    <v-dialog max-width="600px">
        <v-btn flat slot="activator" class="success">Add new project</v-btn>
        <v-card>
            <v-card-title>
                <h2>Add a New Project</h2>
            </v-card-title>
        </v-card>
    </v-dialog>

    <v-dialog>
        <template v-slot:activator="{ on }">
            <v-btn v-on="on">Add a new project</v-btn>
        </template>
        <v-card>
            <v-card-title>
                <h2>Add a New Project</h2>
            </v-card-title>
            <v-card-text>
                <v-form class="px-3" ref="form">
                    <v-text-field label="title" v-model="title" prepend-icon="mdi-folder" :rules="inputRules"></v-text-field>
                    <v-textarea label="information" v-model="content" prepend-icon="mdi-pencil" :rules="inputRules"></v-textarea>
                    <v-btn text class="success mx-0 mt-3" @click="submit">Add project</v-btn>
                </v-form>
            </v-card-text>
        </v-card>
    </v-dialog>
</div>
    
</template>

<script>
export default {

    data() {
        return {
            title: '',
            content: '',
            inputRules: [
                v => v.length >= 3 || 'Minimum length is 3 characters'
            ]
        }
    },
    methods: {
        submit() {
            if(this.$refs.form.validate()){
                console.log(this.title, this.content);
            }
        }
    }
    
}
</script>