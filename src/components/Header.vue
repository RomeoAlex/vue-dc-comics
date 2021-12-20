<template>
    <header>
        <div class="logo">
            <img src="../img/dc-logo.png" alt="Logo DC">
        </div>

        <div class="nav-bar">
            <ul class="menu">
                <li></li>
            </ul>
        </div> 
          
    </header>
</template>

<script>
export default {
  name: "Header",
  
  data: function(){
      return {
          links: [
      {        
          text: 'CHARACTERS',
          url:'#',
          current: false,
      },
      {
          text: 'COMICS',
          url:'#',
          current: true,
      },
      {
          text: 'MOVEIS',
          url:'#',
          current: false,
      },
      {
          text: 'TV',
          url:'#',
          current: false,
      },
      {
          text: 'GAMES',
          url:'#',
          current: false,
      },
      {
          text: 'COLLECTIBLES',
          url:'#',
          current: false,
      },
      {
          text: 'VIDEOS',
          url:'#',
          current: false,
      },
      {
          text: 'FANS',
          url:'#',
          current: false,
      },
      {
          text: 'NEWS',
          url:'#',
          current: false,
      },
      {
          text: 'SHOP',
          url:'#',
          current: false,
      },
    ],
    }

}
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">

</style>
