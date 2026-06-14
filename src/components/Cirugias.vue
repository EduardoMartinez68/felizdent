<template>
     <v-container>
      <v-row><!-- Representa una fila-->
        <v-col cols="12"> <!-- Representa una columna dentro de la fila-->
     <!-- Imagen con título encima -->
    <div class="cirugia-container">
      <div class="image-section">
        <img class="image-container" src="@/assets/Cirugias/CX.jpg" alt="Cirugía" />
        <div class="title">
          <h1>Cirugías</h1>
        </div>
      </div>
      <p class="description">
        Las cirugías dentales son procedimientos especializados que restauran
        la salud y función de tu sonrisa, brindando soluciones seguras y efectivas para cada necesidad.
          </p>
        </div>

        <div class="container1">
          <div class="container-text">
            <p>
            En la Clínica Dental Felizdent, contamos con especialistas altamente
            capacitados para realizar cirugías dentales y maxilofaciales, abarcando
            desde extracciones complicadas hasta procedimientos reconstructivos
            avanzados. Las cirugías dentales son clave para tratar infecciones
            que no pueden resolverse con tratamientos convencionales, asegurando
            la recuperación de la salud bucal y la estética dental. Estas intervenciones
            se realizan con la más alta precisión y tecnología, garantizando la seguridad
            y el confort del paciente en cada paso del proceso.
            </p>
          </div>
          <div class="img-container">
            <img src="@/assets/Cirugias/CX1.jpg" alt="CX">
          </div>
        </div>

      <div class="procedimientos-container">
       <div class="titul">
       <h2>Contamos con diferentes procedimientos</h2>
    </div>
    </div>
    <div class="procedimiento">
      <div class="procedimiento-text">
        <h3>Retiro de terceros molares</h3>
        </div>
        </div>
    <div class="container2">
          <div class="container-text1">
            <p>
            El retiro de terceros molares, comúnmente conocidos como muelas del juicio, es
            un procedimiento odontológico frecuente. Estas muelas suelen erupcionar entre
            los 17 y 25 años, pero en muchos casos no cuentan con suficiente espacio en la
            boca, lo que puede provocar dolor, infecciones, o dañar los dientes adyacentes.
            En la Clínica Dental Felizdent, realizamos este procedimiento de manera segura 
            y con la tecnología más avanzada, asegurando una recuperación rápida y sin complicaciones.
            Si experimentas molestias o te han recomendado la extracción, nuestros especialistas
            en cirugía oral están aquí para ayudarte.
            </p>
          </div>
          <div class="img-container2">
            <img src="@/assets/Cirugias/CX2.jpg" alt="Cirugia M">
          </div>
        </div>


        <div class="procedimiento">
      <div class="procedimiento-text">
        <h3>Caninos retenidos</h3>
        </div>
        </div>
    <div class="container2">
          <div class="container-text1">
            <p>
            Los caninos retenidos son dientes que no logran emerger de manera natural
            a través de las encías, quedando atrapados parcial o completamente dentro
            del hueso o tejido blando. Este problema es común y puede causar complicaciones
            como malposición de otros dientes, dolor, o incluso quistes. En la Clínica
            Dental Felizdent, nuestros especialistas en cirugía maxilofacial y ortodoncia
            tienen la experiencia y las herramientas necesarias para tratar los caninos
            retenidos mediante técnicas que guían su correcta erupción o, en casos más
            complejos, mediante su extracción. Actuar a tiempo es fundamental para
            prevenir daños mayores y garantizar una alineación dental adecuada.
            </p>
          </div>
          <div class="img-container3">
            <img src="@/assets/Cirugias/CX3.jpg" alt="Cirugia M">
          </div>
        </div>

        <div class="procedimiento">
      <div class="procedimiento-text">
        <h3>Extirpación de quistes o tumores bucales</h3>
        </div>
        </div>
    <div class="container2">
          <div class="container-text1">
            <p>
            La extirpación de quistes o tumores bucales es un procedimiento quirúrgico
            que se realiza para eliminar crecimientos anormales en la boca o mandíbula.
            Estos quistes o tumores pueden ser benignos, pero si no se tratan, pueden
            crecer, desplazar dientes, o dañar los huesos y tejidos circundantes.
            En la Clínica Dental Felizdent, nuestros especialistas en cirugía oral
            están capacitados para realizar este procedimiento de forma segura y
            precisa, utilizando tecnología avanzada para minimizar las molestias
            y garantizar una recuperación rápida. Es fundamental acudir a un profesional
            si notas cualquier bulto o cambio en tu boca, ya que la detección temprana
            es clave para prevenir complicaciones mayores.
            </p>
          </div>
          <div class="img-container4">
            <img src="@/assets/Cirugias/CX4.jpg" alt="Cirugia M">
          </div>
        </div>


      <div class="estetica-container">
     <h1 class="estetica-title">Cirugía estética</h1>
        <p class="intro-text">
         En la Clínica Dental Felizdent ofrecemos diversos procedimientos de cirugía estética
        para mejorar la apariencia facial de nuestros pacientes y ayudarlos a alcanzar sus
        objetivos estéticos.
        </p>
    </div>

    <div class="container3">
    <div class="info-rectangle">
      <h2>Bichectomía</h2>
      <p>Una cirugía que reduce el volumen de las mejillas, resaltando los pómulos y afinando el rostro.</p>
    </div>
  </div>

  <!-- sección de Lipopapada -->
  <div class="container4">
          <div class="info-rectangle">
            <h2>Lipopapada</h2>
            <p>Procedimiento que elimina el exceso de grasa en la zona del cuello y debajo del mentón, proporcionando un contorno más definido.</p>
          </div>
        </div>
    </v-col>
    </v-row>
    </v-container>

</template>

<script>
export default {
  name: "Cirugias",
};
</script>

<style scoped>
.cirugia-container {
    padding: 20px;
    font-family: 'Arial', sans-serif;
    margin-top: 110px;
}
.image-section{
    position: relative;
    margin-bottom: 20px;
}
.image-container {
    width: 100%;
    height: auto;
}
.title{
    position: absolute;
    top: 50%;
    left: 10%; /*para alinearlo a la izquierda */
    transform: translateY(-50%);
    color: white;
    background-color:#8A63F1;
    border-radius: 15px;
    padding: 5px 55px; /* Espacio*/

}
.title h1 {
    margin: 0;
    text-align: left; /* Alineación del texto a la izquierda */
    font-size: 2.5em; /* Tamaño del texto */
    font-weight: bold;
}
.description {
    text-align: center;
    margin: 20px 0;
    line-height: 1.6;
    color: #27E1BC;
    font-weight: bold;
    font-size: 1.5em; /* Tamaño del texto */
    margin-top: 20px;
  }
.container1 {
    display: flex; /* alinea los elementos en fila */
    justify-content: space-between; /* espacio entre el texto y la imagen */
    align-items: flex-start;
    padding: 20px;
    margin-top: 120px;
    flex-wrap: wrap;
  }
.container-text {
    width: 100%; /* Asegura que ocupe el 100% en pantallas pequeñas */
    max-width: 450px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
  }
.img-container {
    width: 40%; /* Ajusta el ancho de la imagen */
    max-width: 400px;
    margin-right: 20px; /* Espacio a la derecha de la imagen */
    display: flex;
    align-items: flex-start; 
}
.img-container img {
    width: 100%;
    height: auto;
    margin-top: 0;
    object-fit: contain; 
    
}
.procedimientos-container {
    text-align: center;
    margin-top: 90px;
}
.titul {
    font-size: 1.3em;
}
.titul h2{
  font-weight: bold;

}
.procedimiento {
    display: flex; /* alinea los elementos en fila */
    justify-content: space-between; /* espacio entre el texto y la imagen */
    align-items: flex-start;
    padding: 20px;
    margin-top: 50px;
    flex-wrap: wrap;
}
.procedimiento-text {
    width: 100%; /* Asegura que ocupe el 100% en pantallas pequeñas */
    max-width: 450px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
    margin-bottom: 20px; /* Agrega margen inferior */
}
.procedimiento-text h3{
  font-weight: bold;
}
.container2 {
    display: flex; /* alinea los elementos en fila */
    justify-content: space-between; /* espacio entre el texto y la imagen */
    align-items: flex-start;
    padding: 20px;
    margin-top: -35px;
    flex-wrap: wrap;
  }
.container-text1 {
    width: 100%; /* Asegura que ocupe el 100% en pantallas pequeñas */
    max-width: 450px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
    margin-bottom: 20px; /* Agrega margen inferior */
  }
  .img-container2 {
   position: relative;
   width: 40%; /* Ajusta el ancho de la imagen */
   max-width: 400px;
   margin-right: 20px; /* Espacio a la derecha de la imagen */
   display: flex;
   align-items: flex-start; /* Asegura que la imagen también esté alineada con el texto */
}
.img-container2 img {
    width: 100%;
    height: auto;
    margin-top: 40px;
    object-fit: contain; 
}
/* rectángulo azul detrás de la imagen */
.img-container2::before, .img-container3::before,.img-container4::before{
   content: "";
   position: absolute;
   top: 15px; /* Hace que sobresalga más por la parte superior */
   left: 20px; /* Ajusta la posición horizontal */
   width: 100%;
   height: 80%; /* Ajusta la altura del rectángulo */
   background-color: #27E1BC; 
   z-index: -1; /* Envía el rectángulo detrás de la imagen */
}
.img-container3 {
   position: relative;
   width: 60%; /* ancho de la imagen */
   max-width: 320px;
   margin-right: 20px; /* Espacio a la derecha */
   display: flex;
   align-items: flex-start; /*la imagen también esté alineada con el texto */
}
.img-container3 img {
    width: 100%;
    height: auto;
    margin-top: 40px;
    object-fit: contain; 
}
.img-container4 {
   position: relative;
   width: 40%; /*ancho de la imagen */
   max-width: 300px;
   margin-right: 20px; /* Espacio a la derecha de la imagen */
   display: flex;
   align-items: flex-start; /*la imagen también esté alineada con el texto */
}
.img-container4 img {
    width: 100%;
    height: auto;
    margin-top: 40px;
    object-fit: contain; 
}
.estetica-container {
    padding: 20px;
    margin-top: 10px;
}

.estetica-title {
    background-color: #27E1BC; 
    color: rgb(0, 0, 0); 
    padding: 20px;
    margin: 0 auto; /* Centra el fondo horizontalmente */
    text-align: left; /* Alinea el texto a la izquierda */
    max-width: 1220px; 
    width: 100%; /* Asegura que ocupe todo el espacio disponible */
    box-sizing: border-box; /* para que  el padding no afecte el tamaño del contenedor */
    font-weight: bold;
}

.intro-text {
    text-align: center;
    margin: 5vw 0;
    line-height: 1.4; /* espaciado entre líneas */
    font-weight: bold;
    font-size: 1.8em; /* Tamaño del texto*/
    max-width: 800px; /* para el ancho */
    margin-left: auto; 
    margin-right: auto;
}
.container3 {
  position: relative; 
  width: 420px; /* Ajusta el tamaño */
  margin: 40px 300px 20px auto; /* Margen alrededor del contenedor */
  float: right; /* Alinea el contenedor a la derecha */
}
.info-rectangle {
  background-color: #27E1BC;
  padding: 20px 20px; 
}
.info-rectangle h2 {
  margin-bottom: 10px;
  font-size: 1.5rem;
  color: #000000;
  font-weight: bold; /* Texto en negrita */
  text-align: center;
}
.info-rectangle p {
  font-size: 1rem;
  color: #000000;
  text-align: justify;
}
/* rectángulo verde detrás del texto de bichectomia y lipopapada */
.container3::before, .container4::before{
   content: "";
   position: absolute;
   top: -25px; /* Hace que sobresalga más por la parte superior */
   left: 30px; /* Ajusta la posición horizontal */
   width: 100%;
   height: 100%; /* Ajusta la altura del rectángulo */
   background-color: #8A63F1; 
   z-index: -1; /* Envía el rectángulo detrás de la imagen */
}
.container4 {
  position: relative; 
  width: 450px; /*  tamaño  */
  margin: 60px 600px 20px auto; /* Margen alrededor del contenedor */
  float: right; /* Alinea el contenedor a la derecha */
}
/* Media Queries para dispositivos pequeños */
@media (max-width: 1280px) {
  .title {
    position: absolute; 
    left: 4%; /* Alinea el título al borde izquierdo */
    top: 50%; /* Centra verticalmente el título */
    transform: translateY(-50%); /* Ajusta la posición vertical */
    padding: 8px 20px;
    background-color: #8A63F1;
   
    color: white;
    text-align: left; /* Asegura que el texto esté alineado a la izquierda */
  }
  .title h1 {
    font-size: 1.9em;
  }
  .titul{
    font-size: 1.2em;
  }
  .description {
    font-size: 1.2em;
  }
  .container1, .container2, .container3, .container4 {
    flex-direction: column;
    align-items: center;
  }
  .container-text{
    max-width: 100%;
    margin-top:-80px;
    font-size: 1.3em;
  }
  .container-text1 {
    max-width: 100%;
    font-size: 1.3em;
  }
  .img-container{
    width: 100%;
    max-width: none;
    margin-right: 0;
    margin-top:20px; 

  }.img-container2, .img-container3, .img-container4 {
    width: 100%;
    max-width: none;
    margin-right: 0;
  }
  .procedimiento-text {
    max-width: 100%;
    text-align: center;
    font-size: 1.3em;
  }
  .container3 {
    width: 90%; /* Ocupa todo el ancho disponible en pantallas pequeñas */
    margin: 20px auto; /* Centra el contenedor */
    float: none; /* Elimina el flotado para centrar */
  }
  .container4{
    width: 90%; /* Ocupa todo el ancho disponible en pantallas pequeñas */
    margin: 20px auto; /* Centra el contenedor */
    float: none; /* Elimina el flotado para centrar */
    margin-top:60px;
  }
  .estetica-title{
    text-align: center;
  }
  .intro-text{
    font-size: 1.5em;
    
  }
  .info-rectangle p{
    font-size: 1.3em;
  }
  
}
/* Media Queries para dispositivos medianos */
@media (min-width: 769px) and (max-width: 1280px) {
  .container1, .container2 {
    flex-direction: row;
    justify-content: space-around;
  }
  .container-text, .container-text1 {
    max-width: 100%;
  }
  .container3 {
    width: 90%; /* Ocupa todo el ancho disponible en pantallas pequeñas */
    margin: 20px auto; /* Centra el contenedor */
    float: none; /* Elimina el flotado para centrar */
  }
  .container4{
    width: 90%; /* Ocupa todo el ancho disponible en pantallas pequeñas */
    margin: 20px auto; /* Centra el contenedor */
    float: none; /* Elimina el flotado para centrar */
    margin-top:60px;
  }
  
}
/* Para pantallas más pequeñas */
@media (max-width: 240px) {
    .title {
        font-size: 0.5em; /* Reduce aún más el tamaño del texto */
        padding: 4px 6px; /* Ajusta el padding */
        background-color:#8A63F1; 
    }
}
</style>