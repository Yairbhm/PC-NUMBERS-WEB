# PC-NUMBERS-WEB:root{
  --color1:rgb(42, 42, 80);
  --color2:rgba(23,180,83,.0788);
  --color3:rgb(124, 123, 167);
  --fondo:#f2f2f2;
  --titulos:33px;
  --margenes:60px;
  --espacios:10px;
  --espacios-contenido:45px; 
}

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body{
    font-family: 'open sans';
    background: var(--fondo);
}

img{
  vertical-align: top;
}

/* PRELOADER */
.hidden{
  overflow: hidden;
}

.centrado{
  position: fixed;
  width: 100vw;
  height: 100vh;
  background: #000;
  z-index: 100;
  display: flex;
  justify-content: center;
  align-items: center;
}

.lds-ring {
  display: inline-block;
  position: relative;
  width: 80px;
  height: 80px;
}

.lds-ring div {
  box-sizing: border-box;
  display: block;
  position: absolute;
  width: 64px;
  height: 64px;
  margin: 8px;
  border: 8px solid #cef;
  border-radius: 50%;
  animation: lds-ring 1.2s cubic-bezier(0.5, 0, 0.5, 1) infinite;
  border-color: #cef transparent transparent transparent;
}
.lds-ring div:nth-child(1) {
  animation-delay: -0.45s;
}
.lds-ring div:nth-child(2) {
  animation-delay: -0.3s;
}
.lds-ring div:nth-child(3) {
  animation-delay: -0.15s;
}

@keyframes lds-ring {
  0% {
    transform: rotate(0deg);
  }
  100% {
    transform: rotate(360deg);
  }
}

/*HEADER*/
header{
  width: 100%;
  height: 300px;
  background: url(images/baner.jpg);
  background-attachment: fixed;
  background-position: center;
  background-size: cover;
}

nav{
  width: 100%;
  position: fixed;
  box-shadow: 0 0 10px 0 rgba(0,0,0, .5);
}

.nav1{
  
  background:transparent;
  height: 80px;
  color: #fff;
}

.nav2{
  background: var(--fondo);
  height: 100px;
  color: #000;
}

.contenedor-nav{
  display: flex;
  margin: auto;
  width: 90%;
  justify-content: space-between;
  align-items: center;
  max-width: 600px;
  height: inherit;
  overflow: hidden;
}

nav .enlaces a{
  display: inline-block;
  padding: 5px 0;
  margin-right: 17px;
  font-size: 17px;
  font-weight: 300;
  text-decoration: none;
  border-bottom: 3px solid transparent;
  color: inherit;
}

nav .enlaces a:hover{
  border-bottom: 3px solid #3924b3;
  transition: 0.6s;
}

.logo, .logo img{height: 80px;}

.icono{
  display: none;
  font-size: 24px;
  padding: 23.5px 20px;
}

.textos{
  width: 100%;
  height: 100%;
  display: flex;
  justify-content: center;
  flex-direction: column;
  align-items: center;
  color:#fff;
  overflow: hidden;
  text-align: center;
}

.textos h1{
  font-size: 35px;
}

.textos h2{
  font-size: 30px; font-weight: 200;
}

/*MAIN*/

.contenedor{
  margin: auto;
  padding: var(--margenes) 0;
  width: 90%;
  max-width: 1000px;
  text-align: center;
  overflow: hidden;
}

.contenedor h3{
  font-size: var(--titulos);
  color: var(--color1);
  margin-bottom: var(--espacios);
  
}


.after::after{
  content:'';
  display: block;
  margin: auto;
  margin-top: var(--espacios);
  width: 200px;
  height: 3px;
  background: var(--color1);
  margin-bottom: var(--espacios-contenido);
}

.card{
  display: flex;
  justify-content: space-between;
  flex-wrap: wrap;
  
  
}

.content-card {
  width: 31%;
  box-shadow: 0 0 8px 0 rgba(0,0,0,.7);
  overflow: hidden;
  height: 360px;
}

.people{
  height: 300px;
}

.content-card img{
  width: 100%;
  height: 100%;
  object-fit: cover;

}

.texto-team{
  height: 10%;
  width: 100%;
  padding: var(--espacios) 0;
}



.servicios{
  display: flex;
  color: rgb(0, 0, 0);
  justify-content: space-between;
  margin: auto;
  flex-wrap: nowrap;
}

.caja-servicios>h4{
  margin-bottom: var(--espacios);
  font-size: 25px;
}

.caja-servicios>p{
  text-align: center;
}


.botones-work{
  overflow: hidden;
}

.botones-work li{
  display: inline-block;
  text-align: center;
  margin-left: var(--espacios);
  margin-bottom: var(--espacios-contenido);
  padding: 6px 12px;
  border: 1px solid var(--color1);
  list-style: none;
  color: var(--color1);

}

.botones-work li:hover{
  background: var(--color1);
  color: #fff;
  cursor: pointer;
}

.botones-work.active{
  background: var(--color1);
  color: #fff;
}

.galeria-work{
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  
}

.galeria-work .cont-work{
  width: 25.01%;
  box-shadow: 0 0 6px rgba(0,0,0,.5);
  height: auto;
  overflow: auto;
  margin-bottom: var(--espacios-contenido);
}

.img-work{
  height: 90%;
  width: 100%;
}

.img-work img{
  height: 100%;
  width: 100%;
  object-fit: cover;
}

.textos-work{
  height: 10%;
}

.textos-work h4{
  line-height: 30px;
  font-weight: 300px;
}

/*FOOTER*/

footer{background:url(images/baner.jpg);}

.marca-logo{
  width: 10%;
  margin: auto;
  margin-bottom: var(--espacios);
}

.marca-logo img{
  width: 55%;
}

.iconos{
  display: flex;
  margin:auto;
  justify-content: space-around;
  width: 100%;
}

.fab{
  font-size: 60px;
  color: #fff;
  margin-bottom: var(--espacios);
  display:inline-block
}

footer p{
  margin-top:var(--espacios)
}

@media screen and (max-width: 700px){
  .nav2{
    color: #fff;
  }

  .icono{
    display: block;
    cursor: pointer
  }

  .enlaces{
    position: fixed;
    top: 80px;
    background: #ffffff;
    left: 0;
    height: 100%;
    transition: 1s;
    width: 0;
    overflow: hidden;

  }

  .enlaces a{
    display: block;
    width: 100%;
    height: 50px;
    padding: 20px;
    text-align: center;
    background: #013364;
    color: #fff;

  }

  .textos>h1{font-size: 30px;}
  .textos>h2{font-size: 25px;}

  .content-card{
    width: 48%;
    margin-bottom:var(--margenes);

  }

  :root{
    --margenes: 30px;
  }
}

@media screen and (max-width:500px){
  :root{
    --espacios-contenido: 25px;
  }

  .content-card{
    width: 90%;
  }

  .caja-servicios{
    width: 90%;
    margin-bottom: var(--margenes);
  }

  .cont-work{
    width: 85%;
  }

.iconos{
  margin: auto;
}

}
 <!-- HECHO POR EL UNIVERSITARIO BRAYHAN EDUARDO HUANCA MAMANI 4to C  --> 

<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>PC NUMBERS</title>
    <link rel="stylesheet" href="estilos.css">
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
    <link href="https://fonts.googleapis.com/css2?family=Open+Sans:wght@700&display=swap" rel="stylesheet">
    <script src="https://kit.fontawesome.com/89228b338c.js" crossorigin="anonymous"></script>
</head>
<body class="hidden"></body>
      
    <header>
        <nav id="nav" class="nav1">
            <div class="contenedor-nav">
                <div class="logo">
                    <img src="images/logo2.png" alt="">
                </div>
                <div class="enlaces" id="enlaces">
                    <a href="#" id="enlace-inicio" class="btn-header">Inicio</a>
                    <a href="#" id="enlace-equipos" class="btn-header">Equipos</a>
                    <a href="#" id="enlace-componentes" class="btn-header">Componentes</a>
                    <a href="#" id="enlace-servicio" class="btn-header">Servicios</a>
                    <a href="#" id="enlace-contacto" class="btn-header">Contacto</a>
                    
                </div>
                <div class="icono" id="open">
                    <span>&#9776;</span>
                </div>
                <div>
                </nav>
                <div class="textos">
                    
                    <h1>Tu tienda virtual de componentes para PC GAMING,</h1>
                    <h2>contamos con los componentes adecuados para armar la PC de tús SUEÑOS Y NECESIDADES</h2>
                </div>
                        
                
    </header>
    <main>
        <section class="team contenedor" id="equipos">
            <h3>Nuestro equipos ya ensamblados</h3>
            <p class="after">🕹Garantía en todos los productos.
                🕹Armado e instalación de Windows. 
                👉Gráfica integrada o tarjeta dedicada.
                🚛Envíos a nivel nacional </p>
            <div class="card">
                <div class="content-card">
                    <div class="people">
                        <img src="images/cpu1.jpg" alt="">
                        </div>
                        <div class="texto-team">
                            <h4>YONE RYZEN 5 PRO 4650 16 GB 480GB SSD T.VIDEO RTX 2060 OC </h4>
                        </div>
                    </div>
                <div class="content-card">
                    <div class="people">
                        <img src="images/cpu2.jpg" alt="">
                        </div>
                        <div class="texto-team">
                            <h4>LUNA INTEL I5-11400F 8GB 240GB SSD T.VIDEO GTX 1650 OC 4GB</h4>
                        </div>
                    </div>
                <div class="content-card">
                    <div class="people">
                        <img src="images/cpu3.jpg" alt="">
                        </div>
                        <div class="texto-team">
                            <h4>CERBERO INTEL I5-11400F 16GB 500GB SSD T.VIDEO RTX 3060 TWIN EDGE OC 12GB</h4>
                            
                        </div>
                    </div>
            </div>

        </section>
        <section class="work contenedor" id="componentes">
            <h3>Nuestros Componentes</h3>
            <p class="after">AL MEJOR PRECIO!, Si! al precio más accesible dentro del mercado</p>
            <div class="botones-work">
                <ul>
                    <li class="filter active" data-nombre='todos'>Todos los componentes</li>
                    <li class="filter" data-nombre='procesadoresamd'>Procesadores Amd</li>
                    <li class="filter" data-nombre='procesadoresintel'>Procesadores Intel</li>
                    <li class="filter" data-nombre='placasamd'>Placas Amd</li>
                    <li class="filter" data-nombre='placasintel'>Placas Intel</li>
                    <li class="filter" data-nombre='rams'>Memorias Ram</li>
                    <li class="filter" data-nombre='gpus'>Targetas de Video</li>
                    <li class="filter" data-nombre='psu'>Fuentes de poder</li>
                    <li class="filter" data-nombre='case'>Case</li>
                </ul>
            </div>
            <div class="galeria-work">
                <div class="cont-work procesadoresintel">
                    <div class="img-work">
                        <img src="images/intel1.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES INTEL</h4>
                    </div>
                </div>
                <div class="cont-work procesadoresintel">
                    <div class="img-work">
                        <img src="images/intel2.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES INTEL</h4>
                    </div>
                </div>
                <div class="cont-work procesadoresintel">
                    <div class="img-work">
                        <img src="images/intel3.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES INTEL</h4>
                    </div>
                </div>
                <div class="cont-work procesadoresintel">
                    <div class="img-work">
                        <img src="images/intel4.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES INTEL</h4>
                    </div>
                </div>
                <div class="cont-work procesadoresintel">
                    <div class="img-work">
                        <img src="images/intel5.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES INTEL</h4>
                    </div>
                </div>
                <div class="cont-work procesadoresintel">
                    <div class="img-work">
                        <img src="images/intel6.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES INTEL</h4>
                    </div>
                </div>
                <div class="cont-work procesadoresamd">
                    <div class="img-work">
                        <img src="images/amd1.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES AMD</h4>
                    </div>
                </div>
                <div class="cont-work procesadoresamd">
                    <div class="img-work">
                        <img src="images/amd2.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES AMD/h4>
                    </div>
                </div>
                <div class="cont-work procesadoresamd">
                    <div class="img-work">
                        <img src="images/amd3.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES AMD</h4>
                    </div>
                </div>
                <div class="cont-work procesadoresamd">
                    <div class="img-work">
                        <img src="images/amd4.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PROCESADORES AMD</h4>
                    </div>
                </div>
                <div class="cont-work placasintel">
                    <div class="img-work">
                        <img src="images/tgi1.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PLACAS INTEL</h4>
                    </div>
                </div>
                <div class="cont-work placasintel">
                    <div class="img-work">
                        <img src="images/tgi2.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PLACAS INTEL</h4>
                    </div>
                </div>
                <div class="cont-work placasintel">
                    <div class="img-work">
                        <img src="images/tgi3.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PLACAS INTEL</h4>
                    </div>
                </div>
                <div class="cont-work placasintel">
                    <div class="img-work">
                        <img src="images/tgi4.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PLACAS INTEL</h4>
                    </div>
                </div>
                <div class="cont-work placasamd">
                    <div class="img-work">
                        <img src="images/tga1.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PLACAS AMD</h4>
                    </div>
                </div>
                <div class="cont-work placasamd">
                    <div class="img-work">
                        <img src="images/tga2.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PLACAS AMD </h4>
                    </div>
                </div>
                <div class="cont-work placasamd">
                    <div class="img-work">
                        <img src="images/tga3.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PLACAS AMD</h4>
                    </div>
                </div>
                <div class="cont-work placasamd">
                    <div class="img-work">
                        <img src="images/tga4.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>PLACAS AMD</h4>
                    </div>
                </div>
                <div class="cont-work rams">
                    <div class="img-work">
                        <img src="images/ram1.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>MEMORIAS RAM</h4>
                    </div>
                </div>
                <div class="cont-work rams">
                    <div class="img-work">
                        <img src="images/ram2.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>MEMORIAS RAM</h4>
                    </div>
                </div>
                <div class="cont-work rams">
                    <div class="img-work">
                        <img src="images/ram3.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>MEMORIAS RAM</h4>
                    </div>
                </div>
                <div class="cont-work rams">
                    <div class="img-work">
                        <img src="images/ram4.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>MEMORIAS RAM</h4>
                    </div>
                </div>
                <div class="cont-work rams">
                    <div class="img-work">
                        <img src="images/ram5.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>MEMORIAS RAM</h4>
                    </div>
                </div>
                <div class="cont-work rams">
                    <div class="img-work">
                        <img src="images/ram6.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>MEMORIAS RAM</h4>
                    </div>
                </div>
                <div class="cont-work rams">
                    <div class="img-work">
                        <img src="images/ram7.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>MEMORIAS RAM</h4>
                    </div>
                </div>
                <div class="cont-work rams">
                    <div class="img-work">
                        <img src="images/ram8.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>MEMORIAS RAM</h4>
                    </div>
                </div>
                <div class="cont-work gpus">
                    <div class="img-work">
                        <img src="images/gpu1.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>TARGETAS DE VIDEO</h4>
                    </div>
                </div>
                <div class="cont-work gpus">
                    <div class="img-work">
                        <img src="images/gpu2.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>TARGETAS DE VIDEO</h4>
                    </div>
                </div>
                <div class="cont-work gpus">
                    <div class="img-work">
                        <img src="images/gpu3.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>TARGETAS DE VIDEO</h4>
                    </div>
                </div>
                <div class="cont-work gpus">
                    <div class="img-work">
                        <img src="images/gpu4.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>TARGETAS DE VIDEO</h4>
                    </div>
                </div>
                <div class="cont-work psu">
                    <div class="img-work">
                        <img src="images/fuente1.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>FUENTES DE PODER</h4>
                    </div>
                </div>
                <div class="cont-work psu">
                    <div class="img-work">
                        <img src="images/fuente2.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>FUENTES DE PODER</h4>
                    </div>
                </div>
                <div class="cont-work psu">
                    <div class="img-work">
                        <img src="images/fuente3.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>FUENTES DE PODER</h4>
                    </div>
                </div>
                <div class="cont-work psu">
                    <div class="img-work">
                        <img src="images/fuente4.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>FUENTES DE PODER</h4>
                    </div>
                </div>
                <div class="cont-work psu">
                    <div class="img-work">
                        <img src="images/fuente5.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>FUENTES DE PODER</h4>
                    </div>
                </div>
                <div class="cont-work psu">
                    <div class="img-work">
                        <img src="images/fuente6.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>FUENTES DE PODER</h4>
                    </div>
                </div>
                <div class="cont-work case">
                    <div class="img-work">
                        <img src="images/case1.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>CASE</h4>
                    </div>
                </div>
                <div class="cont-work case">
                    <div class="img-work">
                        <img src="images/case2.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>CASE</h4>
                    </div>
                </div>
                <div class="cont-work case">
                    <div class="img-work">
                        <img src="images/case3.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>CASE</h4>
                    </div>
                </div>
                <div class="cont-work case">
                    <div class="img-work">
                        <img src="images/case4.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>CASE</h4>
                    </div>
                </div>
                <div class="cont-work case">
                    <div class="img-work">
                        <img src="images/case5.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>CASE</h4>
                    </div>
                </div>
                <div class="cont-work case">
                    <div class="img-work">
                        <img src="images/case6.jpg" alt="">
                    </div>
                    <div class="textos-work">
                        <h4>CASE</h4>
                    </div>
                </div>

                
                

                
            </div>
            
    
        
        </section>
        <section class="about" id="servicio">
            <div class="contenedor">
                <h3>Tambien te ofrecemos....</h3>
                <p class="after"></p>
                <div class="servicios">
                    <div class="caja-servicios">
                        <img src="images/armar.png" alt="">
                        <h4>EMSAMBLAJES</h4>
                        <p>segun los componentes que elijas</p>
                    </div>
                    <div class="caja-servicios">
                        <img src="images/cotizar (2).png" alt="">
                        <h4>COTIZACIONES</h4>
                        <p>nos preocupamos por tu cartera</p>
                    </div>
                    <div class="caja-servicios">
                        <img src="images/delivery (2).png" alt="">
                        <h4>DELIVEY</h4>
                        <p>donde quiera que te encuentres</p>
                    </div>
                </div>
            </div>
        </section>

    </main>
    <footer id="contacto">
        <div class="footer contenedor">
            <div class="marca-logo">
            </div>
            <div class="iconos">
                <a href="https://www.youtube.com/channel/UCzUzkkbW-JijlJEwKXKchag" target=_"blank">
                <i class="fab fa-youtube"></i>
            </a>
               
            
            <a href="https://www.facebook.com/PC-numbers-100875138412602/" target=_"blank">
                <i class="fab fa-facebook"></i>
            </a>
             
            <a href="https://wa.me/59173290572" target=_"blank">
                <i class="fab fa-whatsapp-square"></i>
            </a>
            </div>

        </div>
        
        
    </footer>
    <script src="js/jquery.js"></script>
    <script src="js/main.js"></script>
    <script src="js/filtro.js"></script>
    
    
</body>
</html>
