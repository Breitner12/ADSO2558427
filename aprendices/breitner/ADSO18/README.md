## Maquetado html banco 


## Index

~~~
<!DOCTYPE html>
<html lang="es-CO">
<head>
    <meta charset="UTF-8">
    <title>Banco</title>
    <link rel="stylesheet" href="diseños2.css">
</head>
<body>
    <main>
        <header> <img src="banco.jpg" alt="bank"></header>
        <nav><ul>
          <li>.Creditos.</li>
          <li>.leasing.</li>
          <li>.Ahorros.</li>
          <li>Servicio al cliente.</li>
      </ul>
</nav>
        <section>
          <article class="arriba">
            <header class="titulo" id="dosb">INGRESA A TU CUENTA</header>
            <form>
            <ul>
                <li><label>Cuenta: </label>
                    <input type="text"><br><br>
                </li>
                <li><label>Tipo: </label>
                    <input type="text"><br><br>
                </li>
                <li><label>Clave: </label>
                    <input type="text"><br><br>
                </li>
            </ul>
            <button>Ingresar</button>
            </form>
        </article>
        <article class="abajo">
            <ul>
                <li class="tarjeta">TRANSACCIONES</li>
                <li class="lol">Banca personal</li>
                <li class="lol">Banca empresarial</li>
                <li class="lol">Banca seguros</li>
                <li class="lol">Pago de facturas</li>
                <li class="tarjeta">TARJETAS DE CREDITO</li>
                <li class="lol">Credi Visa</li>
                <li class="lol">Credi Mastercard</li>
            </ul>
        </article>
    </section>
    <aside>
        <article id="superiorizquierda">
            <header class="titulo"  id="topizquierda">SOLICITA NUESTROS PRODUCTOS</header>
            <img src="tarjeta.jpg" alt="no hay tarjeta">
            <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Veniam maxime</p>
        </article>
        <article id="superior">
            <header class="titulo"  id="topderecha">AHORRRO ESTUDIANTIL</header>
            <img src="libros.jpg" alt="no libros">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Consequat</p>
        </article>
        <article id="inferior">
            <header class="titulo">CREDITOS VIHICULOS</header>
            <img src="llaves.jpg" alt="no hay llaves">
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Rerum mollitia </p>
        </article>
        <article id="inferiorderecha">
            <header class="titulo">CREDITOS HIPOTECARIO</header>
            <img src="casita.jpg" alt="no tengo casa">
            <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nemo laborum sequ</p>
        </article>
    </aside>
    <footer>
        <p>
            contactenos
            <br>
            linea gratuita 018000-00001
                <br>
                Banco entidad financiera - Todos los derechos reservados.
            </p>
        </footer>
    </main>
</body>
</html>
~~~

## Diseño

~~~
main{
    height: 840px;
    margin: auto;
    width: 850px;
}
header{
    height: 173px;
    border-bottom: 10px solid black;
}
header img{
    border-radius: 15px 15px 0px 0px;
    width: 849px;
    height: 173px;
}
nav{
    background-color: #eec13b;
    border-radius: 0px 0px 10px 10px;
    height: 65px;
    padding-bottom: 10px;
    border-top: 10px solid black;
}
nav ul{
    padding-top: 25px;
}
*{
    margin: 0;
    padding: 0;
}

ul li{
    border-right: 2px solid white;
    color: black;
    display: inline;
    font-size: 20px;
    padding: 8px 50px;
}
section{
    float: left;
    height: 490px;
    padding-top: 10px;
    width: 283px;
}
.arriba{
    background-color: #b2b2b2;
    border-radius: 15px 15px 0px 0px;
    height: 190px;
    margin-bottom: 10px;
    width: 272px;
}
.arriba ul li{
    border-right: 0px;
    font-size: 18px;
    padding: 10px 20px;    
}
.arriba input{
    height: 15px;
    width: 150px;
}
.arriba button{
    background-color: #a88210;
    border: 2px solid black;
    border-radius: 5px;
    color: black;
    display: block;
    margin-right: auto;
    margin-left: auto;
    width: 90px;
}
.titulo{
    background-color: #232323;
    border: 1px solid black;
    color: #eee9e9;
    height: 40px;
    text-align: center;
    width: 270px;
}
#dosb{
    border-radius: 15px 15px 0px 0px;
}
.abajo{
    background-color: #232323;
    height: 275px;
    width: 275px;
}
.abajo ul li{
    display: block;
    font-size: 15px;
    text-align: center;
}
.lol{
    color: #e4e3e3;
    margin-bottom: 1px solid #a3a3a3;
    border-bottom: 1px solid #343434;
}
.tarjeta{
    background-color: black;
    color: #ebb821;
}
aside{
    float: right;
    height: 475px;
    width: 560px;
    padding-top: 10px;
}
article{
    background-color: #f7f7f7;
    height: 233px;
    width: 270px;
    display: inline-block;
}
#superiorizquierda{
    margin-bottom: 10px;
    border-radius: 15px 0px 0px 0px;
}
#superior{
    margin-bottom: 10px;
    border-radius: 0px 15px 0px 0px;
    float: right;
}
#inferior{
    border-radius: 0px 0px 0px 15px;
}
#inferiorderecha{
    border-radius: 0px 0px 15px 0px;
    float: right;
}
aside img{
    height: 110px;
    width: 240px;
    border-radius: 10px;
}
aside article{
    text-align: center;
}
footer{
    background-color: #1b1b1b;
    border-radius: 0px 0px 15px 15px;
    height: 70px;
    color:#a3a3a3;
    clear: both;
    text-align: center;
    padding-top: 10px;
}
~~~