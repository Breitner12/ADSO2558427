## Maquetado Html Veterinaria

## Index
~~~
<!DOCTYPE html>
<html lang="es-CO">
<head>
    <meta charset="UTF-8">
    <link rel="stylesheet" href="diseños.css">
    <title>perros</title>

</head>
<body>
    <main>
      <header>
        <img src="mascotas.jpg" alt="mascotas"></header>
      <nav>
        <ul>
          <li>Servicios</li>
          <li>Productos</li>
          <li>Guardería</li>
          <li>Promociones</li>
        </ul>
      </nav>
      <section>
        <article><h3>Cuidado y educacion para su perro</h3><br>
          <p>En general, es importante procurar <br> una alimentación saludable para ellos,<br> así como favorecer su actividad física <br> y estimular su socialización. <br> También es fundamental ofrecerle cuidados <br> y revisiones veterinarias para controlar <br> su estado de salud y mejorar su calidad de vida.</p>
          <img src="perro2.jfif" alt="perrito">
          <a href="https.google.com">ir a google</a>
        </article>
        <article>
          <h3>Salir de viaje con su mascota</h3><br>
          <p>Comunícate a tu lugar de destino y asegúrate <br> que tu perro sea bienvenido en el sitio en donde <br> te hospedes.Visita a tu veterinario, asegúrate <br> que sus vacunas estén al día y actualizadas <br> de los registros sanitarios para tu viaje.</p>
          <img src="biglol.png" alt="bonito"> 
          <a href="https.google.com">ir a google</a>
        </article>
      </section>
      <aside>
       <header>Solicitar cita medica</header>
       <ul>
        <li>Mascotas:</li> <input type="ingrese nombre"><br><br>
        <li>Edad:</li> <input type="text"><br><br>
        <li>Raza:</li><input type="ingrese raza"><br><br>
        <li>Fecha:</li><input type="dd/mm/aaaa"><br><br>
        <li>Hora:</li><input type="--:-- ----"><br><br>
        <li>Amo:</li><input type="ingrese Nombre"><br><br>
        <button>Validar cita</button>
       </ul>
      </aside>
      <footer>
        <p>
          Contáctenos <br>
          Linea gratuita: 018000-00001
        </p>
      </footer>
    </main>
</body>
</html>
~~~

## Diseño

~~~
main{
    border: 2px solid white;
    width: 1000px;
    height: 800px;
    margin: auto;

}
header{
    border: 2px solid white;
    height: 150px;
    
}
nav{
    background-color: #184b4a;
    border: 2px solid #184b4a;
    height: 50px;
    border-radius: 0px 0px 10px 10px;
    padding: 0px;
   
    
    
}
section{
    border: 2px solid white;
    height: 500px;
    width: 555px;
    display: inline-block;
    float: left ;
    
}
 
article{
    
    height: 205px;
    width: 540px;
    margin-top: 30px;
    margin-left: 20px;
    background-color: #f8ed72ef;
    border-radius: 10px 10px 0px 0px;
    
    
}

aside{
    background-color: #4a6e6e;
    height: 460px;
    width: 350px;
    display: inline-block;
    margin-left: 85px;
    margin-bottom: 25px;
    margin-top: 30px;
    margin-right: 1px;
    border-radius: 10px 10px 10px 10px;
    
}
footer{
    background-color: #2d9217;
    color: white;
    height: 50px;
    text-align: center;
    border-radius: 0px 0px 10px 10px;
}
header img{
  width: 997px;
  height: 152px;  
 
}
ul li{
   padding: 0px;
    padding-bottom: 15px;
    color: white;
    font-size: 25px;
    padding: 55px;
    display: inline
    
  
     
}
section article  img{

    width: 100px;
    height: 110px;
    margin-left: 75px; 
    border-radius: 10px 10px 10px 10px;
    border: 2px solid black;

    
    
}
h3{
    padding-left: 30px;
    

}
p{
    padding-left: 15px;
    display: inline-block;
    font-size: 13px; 
}

aside header{
      
     background-color: #184b4a;
     height: 35px;
     border-radius: 10px 10px 0px 0px;
     color: white;
     font-size: 20px; 
     text-align: center;
     border-color: #184b4a;

}

aside ul li{

   font-size: 26px;
   padding: 0px;
   margin-right: 2px;

    
}

button{

    width: 150px;
    height: 50px;
    margin-left: 40px;
}

~~~