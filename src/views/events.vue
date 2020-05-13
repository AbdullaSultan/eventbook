<template>
    <div>
        <h1>Events</h1>

        <v-row>
            <v-col cols="12" v-for="event in events" :key="event.id">
                <v-card>
                    <v-card-title>{{ event.title }}</v-card-title>
                    <v-card-text>{{ event.description }}</v-card-text>
                    <v-card-actions>
                        <v-btn block color="success">
                            <v-icon>mdi-home</v-icon>
                        </v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
        </v-row>

    </div>
</template>

<script>
export default {
    data(){
        return {
            events: [
                {  id: 1000, title: "Konsert", description: "hei hei hei" },
                {  id: 1001, title: "Presentasjon", description: "hei hei hei" }
            ]
        }
    }
}
</script>