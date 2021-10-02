<template>
  <section>
    <div class="main">
      <h1>Players</h1>
      <Player :players="players"/>
      

    </div>
 
  </section>
</template>

<script>
import Player from './Player.vue'


export default {
  name: 'PlayerListing',
  components: {
    Player,

  },

  data(){
    return{
      players: []
    }
  },

  created(){
    this.players = [
      {
      country: "Argentina",
      firstName: "Emiliano",
      surname: "Martinez",
      squadImage: 'https://images.webapi.gc.avfcservices.co.uk/077989d0-fe70-11eb-9fd1-8f983c0036a9.png',
      joinDate: "2020-09-16",
      position: "Goalkeeper",
      shirtNumber: "1",
      profilePageUrl: "https://www.premierleague.com/players/4245/Emiliano-Mart%C3%ADnez/overview"
      },
    {
      country: "England",
      firstName: "Tyrone",
      surname: "Mings",
      squadImage: "https://images.webapi.gc.avfcservices.co.uk/fe823660-fe74-11eb-9030-cff3f8b0f409.png",
      joinDate: "2019/8/7",
      position: "Defender",
      shirtNumber: "5",
      profilePageUrl: "https://www.premierleague.com/players/8900/Tyrone-Mings/overview"
    },
    {
      country: "Argentina",
      firstName: "Emiliano",
      surname: "Buendía",
      squadImage: "https://images.webapi.gc.avfcservices.co.uk/fea304d0-fe74-11eb-b150-03522eaa62c1.png",
      joinDate: "2021-06-10",
      position: "Midfielder",
      shirtNumber: "10",
      profilePageUrl: "https://www.premierleague.com/players/26408/Emiliano-Buend%C3%ADa/overview"
    },
    {
      country: "Burkina Faso",
      firstName: "Bertrand",
      surname: "Traoré",
      squadImage: "https://images.webapi.gc.avfcservices.co.uk/fe12d2c0-fe74-11eb-bee9-b358e34aa6cb.png",
      joinDate: "2020-09-16",
      position: "Midfielder",
      shirtNumber: "15",
      profilePageUrl: "https://www.premierleague.com/players/10394/Bertrand-Traor%C3%A9/overview"
    },
    {
      country: "England",
      firstName: "Danny",
      surname: "Ings",
      squadImage: "https://images.webapi.gc.avfcservices.co.uk/fe56b990-fe74-11eb-bee9-b358e34aa6cb.png",
      joinDate: "2021-08-04",
      position: "Forward",
      shirtNumber: "20",
      profilePageUrl: "https://www.premierleague.com/players/8245/Danny-Ings/overview"
    }
    ]
  },

 
  
}



</script>

<style scoped>
.main{
  text-align: center;
  background-image: url(https://cdn.wallpapersafari.com/42/66/F7KA4S.jpg);
  background-position: center;
  background-size: cover;
  height: 100vh;
}

.main h1{
  margin: 0 0 50px 0;
  padding-top: 100px;
  font-size: 100px;
}
</style>
