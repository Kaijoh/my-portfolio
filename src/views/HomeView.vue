<template>
  <v-card>
    <v-tabs
      v-model="tab"
      bg-color="teal-darken-3"
      stacked
      centered
    >
      <v-tab value="one">
        <v-icon>mdi-home-account</v-icon>
        Home
      </v-tab>
      <v-tab value="two">
        <v-icon>mdi-information</v-icon>
        About
      </v-tab>
      <v-tab value="three">
        <v-icon>mdi-apps</v-icon>
        Projects
      </v-tab>
      <v-tab value="four">
        <v-icon>mdi-phone</v-icon>
        Contacts
      </v-tab>
    </v-tabs>

    <v-container fluid class="home" grid-list-md>
      <v-window v-model="tab">
        <v-window-item value="one" class="homediv">
      
          <div
            class="c1 pa-5"
            elevation="0"
          >
          <v-card-title class="text-h6 text-md-h5 text-lg-h4">
              <h3 class="hh3 ">[/ LETS GO! \]</h3>
              <h2 class="hh2 ">JOHN KAIL J.</h2>
              <h1 class="hh1 pa-5 ml-3">TAUSA</h1>
            </v-card-title>
            <v-card-text >
              <p 
              
              class="cp1 font-weight-bold" >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eligendi perspiciatis, rem modi recusandae error nesciunt adipisci, praesentium consequuntur reprehenderit animi veritatis ipsum voluptatibus fugit qui sunt cupiditate necessitatibus magni sed!</p>
            </v-card-text>
            <v-btn class="ma-5">
              Resume
              <v-tooltip
                activator="parent"
                location="end"
              >Download</v-tooltip>
            </v-btn>
          </div>
            
          <div
            width="500"
            class="c1 pa-5"
            color="transparent"
            elevation="0"
              >
              <v-card-title class="text-h6 text-md-h5 text-lg-h4">Title</v-card-title>
              <v-card-text >
                <p 
                
                class="font-weight-bold" >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Eligendi perspiciatis, rem modi recusandae error nesciunt adipisci, praesentium consequuntur reprehenderit animi veritatis ipsum voluptatibus fugit qui sunt cupiditate necessitatibus magni sed!</p>
              </v-card-text>
              <v-btn>
                Resume
                <v-tooltip
                  activator="parent"
                  location="end"
                >Download</v-tooltip>
              </v-btn>
          </div>
        </v-window-item>
        
        <v-window-item value="two">
          Two Lorem ipsum dolor sit amet consectetur adipisicing elit. Assumenda cumque autem dolorum quas accusantium, ea excepturi fugit qui, possimus modi ex non dolores perspiciatis architecto consequuntur officiis praesentium sapiente. Expedita!
        </v-window-item>

        <v-window-item value="three">
          Three Lorem, ipsum dolor sit amet consectetur adipisicing elit. Laborum repudiandae, deserunt iusto incidunt nesciunt accusamus minima numquam quas est eveniet culpa! Nisi dolor iste necessitatibus optio explicabo impedit aliquid ratione!
        </v-window-item>

        <v-window-item value="four">
          Three Lorem,
        </v-window-item>
      </v-window>
    </v-container>
  </v-card>
</template>

<script>
  export default {
    data: () => ({
      tab: null,
    }),
  }
</script>

<style lang="css">
.home {
  background-color: #202020;
  
  height: 100vh;
  width: 100%;
}

.homediv{
  display: flex;
}

.c1 {
  margin: 250px 10px;
}
.c1 p {
  padding-right: 320px;
  margin-top: 15px;
  color: aliceblue;
  
}

.hh1 {
  font-size: 105px;
}

.hh3 {
  font-size: 25px;
  margin-left: 10px;
  margin-bottom: 30px;
}


</style>