<template>
  <div>

    <h2>Kommende hendelser</h2>

        <v-row>
            <v-col cols="4" v-for="event in events" :key="event.id">
                <v-card>
                    <v-card-title>{{ event.title }}</v-card-title>
                    <v-card-text>{{ event.description }}</v-card-text>
                    <v-card-actions>
                        <v-btn block color="success">
                            <v-text>Se mer</v-text>
                        </v-btn>
                    </v-card-actions>
                </v-card>
            </v-col>
        </v-row>

    <h2>Kommende eventer</h2>

        <v-row>
            <v-col cols="12" v-for="update in updates" :key="update.id">
                <v-card>
                    <v-card-title>{{ update.title }}</v-card-title>
                    <v-card-text>{{ update.description }}</v-card-text>
                    <v-card-actions>
                        <v-btn block color="success">
                            <v-text>Se eventside</v-text>
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
                {  id: 1000, title: "Konsert", description: "Jaa9" },
                {  id: 1001, title: "Foredrag", description: "Øyafestivalen" },
                {  id: 1002, title: "Foredrag", description: "Berg Hansen" }
            ],
            updates: [
                {  id: 1000, title: "Konsert", description: "OnklP utsetter til 13.mai" },
                {  id: 1001, title: "Foredrag", description: "Øyafestivalen: Ta med egen PC og utstyr!" },
                {  id: 1002, title: "Foredrag", description: "Berg Hansen: Kom på foredrag!" }
            ]
        }
    }
}


</script>
