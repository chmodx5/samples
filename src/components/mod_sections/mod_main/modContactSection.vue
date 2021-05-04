<template>
    <mod-section secHeading='contact me'>
        <v-form v-model="valid">
            <v-container>
            <v-row>
                <v-col
                cols="12"
                md="4"
                >
                <v-text-field
                    v-model="firstname"
                    :rules="nameRules"
                    :counter="10"
                    label="Name"
                    required
                ></v-text-field>
                </v-col>

                
               

                <v-col
                cols="12"
                md="4"
                >
                <v-text-field
                    v-model="email"
                    :rules="emailRules"
                    label="E-mail"
                    required
                ></v-text-field>
                </v-col>

                <v-col
                cols="12"
                md="4"
                >
                 <v-text-field
                    v-model="lastname"
                    :rules="nameRules"
                    :counter="10"
                    label="Subject"
                    required
                ></v-text-field>
                </v-col>

                <v-col
                cols="12"
                md="4"
                >
                 <v-text-field
                    v-model="lastname"
                    :rules="nameRules"
                    :counter="10"
                    label="Message"
                    required
                ></v-text-field>
                </v-col>

            </v-row>
            </v-container>
        </v-form>       
    </mod-section>
</template>

<script>
import modSection from '@/components/mod_sections/mod_slots/modSection.vue'

export default {
    name: 'modContactSection',
    components: {
        modSection
    },
    data: () => ({
      valid: false,
      firstname: '',
      lastname: '',
      nameRules: [
        v => !!v || 'Name is required',
        v => v.length <= 10 || 'Name must be less than 10 characters',
      ],
      email: '',
      emailRules: [
        v => !!v || 'E-mail is required',
        v => /.+@.+/.test(v) || 'E-mail must be valid',
      ],
    }),
}
</script>
