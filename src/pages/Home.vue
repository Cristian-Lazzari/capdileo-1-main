
<script >
  
  export default {
  

    data(){
        return{     
            carouselMain:[
                {
                    img : "",
                    paragrafo : "",
                    link : "",
                    titolo : "",
                },
                {
                    img : "",
                    paragrafo : "",
                    link : "",
                    titolo : "",
                },
                {
                    img : "",
                    paragrafo : "",
                    link : "",
                    titolo : "",
                }
            ]
           
        }
    },
    
  }
</script>


<template>

<main>
    <div class="left-main">
        <img src="" alt="">
    </div>
    <div class="right-main">
        <div class="top-right">
            <h2>titolo paragrafo</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Quaerat nobis rerum autem eligendi facilis officiis mollitia fugit, voluptates numquam iusto. Sint maxime natus voluptatibus, quisquam ipsum corporis? Aliquam, ea nisi.</p>
        </div>
        <div class="bottom-right">
            <div class="left-bottom">
                <h3>orari d'apertura</h3>
                <div class="container">
                    <div class="container-giorni">
                        <span>lunedi</span>
                        <span>martedi</span>
                        <span>mercoledi</span>
                        <span>giovedi</span>
                        <span>venerdi</span>
                        <span>sabato</span>
                        <span>domenica</span>
                    </div>
                    <div class="container-orari">
                        <span>chiuso</span>
                        <span>16-22</span>
                        <span>16-22</span>
                        <span>16-22</span>
                        <span>16-22</span>
                        <span>16-22</span>
                        <span>16-22</span>
                    </div>
                </div>
            </div>
            <div class="right-bottom">
                <h3>dove trovarci</h3>
                <h4>Via lorem ipsum 12, 34900 Citta</h4>
                <img src="../assets/img/maps.png" alt="">
            </div>
        </div>
    </div>
</main>
  
</template>

<style lang="scss" scoped>
@use '../assets/styles/general.scss' as *;

main{
    display: flex;
    
    .left-main{
    background-color: red;
    width: 75%;
    background: url(../assets/img/bigimage.png);
    }
    
    .right-main{
        background-color: #EBD59B;
        height: 50%;
        width: 25%;

        .top-right{
            padding: 5rem 3rem;
            h2{
                color: black;
                font-size: 27px;
                text-transform: uppercase;
            }
            p{
                color: black;
                font-size: 25px;
                padding-top: 2rem;
            }
        }
        .bottom-right{
            background-color: #4D0404;
            display: flex;
            justify-content: space-between;
            padding: 1rem;
            
            .left-bottom{
                width: 50%;
                h3{
                    padding: .5rem;
                    font-size: 22px;
                    text-transform: uppercase;
                }
                
                .container{
                    display: flex;
                    justify-content: space-between;
                    padding: 1rem;
                }
                .container-giorni, .container-orari{
                    display: flex;
                    flex-direction: column;
                    font-size: 20px;
                }
                
            }
            .right-bottom{
                display: flex;
                flex-direction: column;
                align-items: center;
                gap: 1rem;
                h3{
                    text-align: center;
                    padding: .5rem;
                    font-size: 22px;
                    text-transform: uppercase;
                }
                h4{
                    text-align: center;
                }
                img{
                    width: 200px;
                    
                }
            }
        }
    }
}
</style>
