<template>
<div class="container">
 <a :href="player.profilePageUrl"  class="player" v-for="player in players" :key="player.shirtNumber">
     <img class="pic" :src="player.squadImage" alt="SquadImage">
     <h1>{{player.firstName}}</h1>
     <h1>{{player.surname}}</h1>
     <p>{{player.country}}</p>
     <p>{{player.joinDate}}</p>
     <p>{{player.position}}</p>
     <h2>{{player.shirtNumber}}</h2>
 </a>

</div>
</template>



<script>

export default {
    name: 'Player',
    props: {
        players: Array,
    }
}



</script>

<style scoped>

.player{
    padding: 2rem;
    background-color: #ffffff;
    margin: 2rem;
    border-radius: 1.25rem;
    text-align: center;
    color: #1d1d1d;
    border-top-left-radius: 3.75rem;
    border-top-right-radius: 3.75rem;
    border-bottom-right-radius: 2.5rem;
    border-bottom-left-radius: 2.5rem;
    box-shadow: rgba(50, 50, 93,1) 0px 13px 27px -5px, rgba(0, 0, 0, 0.3) 0px 8px 16px -8px;
    transition: 0.5s all;
}

.player h1{
    color: rgb(44, 44, 44);
    
}
.player h2{
    font-size: 2.5rem;
    color: rgb(47, 39, 59);
}

.player p{
    color: rgb(78, 78, 78);
}

.player:hover{
    scale: 1.1;
    transition: ease-in-out;
    cursor: pointer;
}
.container{
    display: flex;
    justify-content: center;
    flex-wrap: wrap;
}
.pic{
    width: 200px;
    height: 200px;
    background-color: transparent;
}

</style>