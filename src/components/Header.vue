<template>
    <header>
        <div class="header-container">
                <div class="logo">
                    <img src="../img/dc-logo.png" alt="Logo DC">
                </div>
                <div class="nav-bar">
                    <ul class="menu">
                        <li v-for="(link , index) in links" :key="index">
                            <a :class="{ 'current' :link.current }" href="link.url" >{{ link.text }}</a>
                        </li>
                    </ul>
                </div>  
        </div>
        
    </header>
</template>

<script>
export default {
  name: "Header",
  data: function() {
      return {
          links: [
                    {        
                        text: 'CHARACTERS',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'COMICS',
                        url: '#',
                        current: true,
                    },
                    {
                        text: 'MOVIES',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'TV',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'GAMES',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'COLLECTIBLES',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'VIDEOS',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'FANS',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'NEWS',
                        url: '#',
                        current: false,
                    },
                    {
                        text: 'SHOP',
                        url: '#',
                        current: false,
                    },
                ],
            };
        },
};
</script>

<style lang="scss" scoped>
@import '../style/variables.scss';
.header-container{
        margin:auto;
        padding: 0 20px;
        width: 80%;
        height:140px;
        display: flex;
        justify-content: space-between;
        align-items: center;
        // test
        // background-color:red;
        // line-height: 180px;
        .logo{
                img{
                    width: 80px ;
                    }
        }
        .nav-bar{
                .menu{
                    display: flex;
                        li{
                            font-size: 20px;
                            margin-left: 20px;
                            font-weight: bold;
                        }
                        a{
                            text-decoration: none;
                            line-height: 140px;
                            display: inline-block;
                            color:black;
                                &.current{
                                color:$brand_primary_color;
                                border-bottom: 4px solid $brand_primary_color;
                                
                                }
                        }
                        
                }
        }
        
}
</style>
