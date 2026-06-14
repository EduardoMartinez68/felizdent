<template>
    <v-container>
     <v-row>
       <v-col cols="12">
    <!-- Imagen con título encima -->
   <div class="Tratamientos-container">
     <div class="image-section">
       <img class="image-container" src="@/assets/Tr/Tra1.jpg" alt="Tratamientos" />
       <div class="title">
         <h1>Tratamientos Generales</h1>
       </div>
     </div>
   </div>

   <v-col cols="12">
    <div class="titul">
    <div class="titulQ"> ¡Contamos con diferentes procedimientos!</div>
    </div>
    </v-col>

     <div class="container2">
    <div class="img-container2">
    <img src="@/assets/Tr/Tra2.jpg" alt="Limpiezas Dentales">
    </div>

    <div class="procedimiento">
      <div class="procedimiento-text">
        <h3>Limpiezas Dentales</h3>
          <div class="container-text1">
            <p>
            La limpieza dental es un procedimiento preventivo que elimina la placa bacteriana,
            el sarro y las manchas superficiales en los dientes, ayuda a prevenir enfermedades
            periodontales (de las encías), caries, y mantiene la salud bucal en óptimas condiciones.
            </p>
          </div>
          </div>
        </div>
    </div>

    <div class="procedimiento">
      <div class="procedimiento-text1">
        <h3>Resinas Dentales</h3>
    <div class="container2">
          <div class="container-text2">
            <p>
            Las resinas son materiales de color similar al diente natural, usados para restaurar
            dientes dañados por caries, fracturas o para mejorar la estética dental. Se aplican
            en cavidades pequeñas o medianas.
            </p>
          </div>
         </div>
          </div>
          <div class="img-container3">
            <img src="@/assets/Tr/Tra3.jpg" alt="Resinas">
          </div>
        </div>

        <div class="container2">
    <div class="img-container2">
    <img src="@/assets/Tr/Tra4.jpg" alt="Extracciones">
    </div>

    <div class="procedimiento">
      <div class="procedimiento-text">
        <h3>Extracciones Dentales</h3>
          <div class="container-text1">
            <p>
            La extracción es el procedimiento de remover un diente que no se puede
            restaurar, ya sea por caries extensa, fractura o infección. También
            es común en casos de dientes retenidos o apiñamiento dental.
            </p>
          </div>
          </div>
        </div>
    </div>

    <div class="procedimiento">
      <div class="procedimiento-text1">
        <h3>Prótesis Fijas</h3>
    <div class="container2">
          <div class="container-text2">
            <p>
            Son restauraciones dentales permanentes diseñadas para reemplazar uno o varios dientes
            perdidos. Están cementadas o fijadas de forma segura.
            </p>
          </div>
         </div>
          </div>
          <div class="img-container3">
            <img src="@/assets/Tr/Tra5.jpg" alt="Prótesis">
          </div>
        </div>

        <div class="container2">
    <div class="img-container2">
    <img src="@/assets/Tr/Tra6.jpg" alt="Prótesis Removibles">
    </div>

    <div class="procedimiento">
      <div class="procedimiento-text">
        <h3>Prótesis Removibles</h3>
          <div class="container-text1">
            <p>
            Son dispositivos dentales que se pueden retirar y reemplazar a voluntad, diseñados
            para pacientes que han perdido varios o todos sus dientes. Permiten recuperar
            la función masticatoria, mejoran la estética
            </p>
          </div>
          </div>
        </div>
    </div>

    <div class="procedimiento">
      <div class="procedimiento-text1">
        <h3>Placas Totales</h3>
    <div class="container2">
          <div class="container-text2">
            <p>
            Las placas totales, también conocidas como dentaduras completas, son prótesis
            removibles diseñadas para reemplazar todos los dientes en una arcada
            (superior o inferior). Están hechas de acrílico y se ajustan a la encía del paciente.
            </p>
          </div>
         </div>
          </div>
          <div class="img-container3">
            <img src="@/assets/Tr/Tra7.jpg" alt="Placas totales">
          </div>
        </div>

        <v-col cols="12">
        <p class="description2">
            "Cuidar tu sonrisa hoy, es garantizar tu salud mañana."
        </p>
        <div class="img-container4">
          <img src="@/assets/Tr/Tra8.jpg"   alt="Diente" />
        </div>
      </v-col>

    
   </v-col>
   </v-row>
   </v-container>

</template>

<script>
export default {
 name: "Tratamientos",
};
</script>

<style scoped>
.Tratamientos-container {
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
    position: absolute; /* Para el título */
    top: 50%; /* Centrar verticalmente */
    left: 50%; /* Centrar horizontalmente */
    transform: translate(-50%, -50%); /* Ajusta el centro del texto */
    background-color:#8A63F1; 
    color: white; 
    padding: 5px 18px; /* Espacio*/
    text-align: center;
    font-size: 1.3em; /* Tamaño del texto */
    font-weight: bold;
    border-radius: 17px;

}
.title h1 {
   margin: 0;
   font-weight: bold;
}
.titul{
  padding: 20px;
  margin-top: -40px;
  font-family: 'Arial', sans-serif;
  text-align: center; 
}
.titulQ{
  display: inline-block; /* Se ajusta al tamaño del texto */
  border-bottom: 3px solid #ccc; /* Solo aplica un borde debajo */
  padding: 10px; /* Añade espacio alrededor del texto */
  margin: 20px auto; /* Centra el elemento */
  font-weight: bold;
  font-size: 1.5em;
  text-align: center;
  font-weight: bold;
  
}
.img-container2 {
   position: relative;
   width: 40%; /* Ajusta el ancho de la imagen */
   max-width: 320px;
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
    max-width: 400px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
    margin-bottom: 20px; /* Agrega margen inferior */
}
.procedimiento-text h3{
  font-weight: bold;
  text-align: center; /* Centrar el título */
  width: 100%; /* Asegura que ocupe el 100% del ancho disponible */
  margin-top:-40px; 
}
.container2 {
    display: flex; /* alinea los elementos en fila */
    justify-content: space-between; /* espacio entre el texto y la imagen */
    align-items: flex-start;
    padding: 20px;
    margin-top: 60px;
    flex-wrap: wrap;
  }
.container-text1 {
    width: 100%; /* Asegura que ocupe el 100% en pantallas pequeñas */
    max-width: 450px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
    margin-top:10px; 
  }
/* rectángulo azul detrás de la imagen */
.img-container2::before{
   content: "";
   position: absolute;
   top: 15px; /* Hace que sobresalga más por la parte superior */
   left: 20px; /* Ajusta la posición horizontal */
   width: 100%;
   height: 80%; /* Ajusta la altura del rectángulo */
   background-color: #27E1BC; /* Color azul */
   z-index: -1; /* Envía el rectángulo detrás de la imagen */
}
.img-container3 {
   position: relative;
   width: 60%; /* Ajusta el ancho de la imagen */
   max-width: 320px;
   margin-right: 20px; /* Espacio a la derecha de la imagen */
   display: flex;
   align-items: flex-start; /* Asegura que la imagen también esté alineada con el texto */
   margin-top:15px;
}
.img-container3 img {
    width: 100%;
    height: auto;
    margin-top: 40px;
    object-fit: contain; 
}
.img-container3::before{
   content: "";
   position: absolute;
   top: 15px; /* Hace que sobresalga más por la parte superior */
   left: 20px; /* Ajusta la posición horizontal */
   width: 100%;
   height: 80%; /* Ajusta la altura del rectángulo */
   background-color: #8A63F1; /* Color azul */
   z-index: -1; /* Envía el rectángulo detrás de la imagen */
}
.procedimiento-text1 h3{
  font-weight: bold;
  text-align: center; /* Centrar el título */
  width: 100%; /* ocupa el 100% del ancho disponible */
  margin-top:  50px; 
}
.container-text2 {
    width: 100%; /* ocupa el 100% del ancho disponible */
    max-width: 400px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
    margin-top:-65px; 
  }
  .description2 {
    text-align: center;
    margin: 5vw 0;
    line-height: 1.4; /* Reduce el espaciado entre líneas */
    color: #27E1BC;
    font-weight: bold;
    font-size: 3em; /* Tamaño del texto reducido */
    max-width: 800px; /* para que no sea tan ancho */
    margin-left: auto; 
    margin-right: auto; 
    
  
  }
  .img-container4{
   width: 100%;
    display: flex;
    justify-content: center;
  
  }
  .img-container4 img{
    width: 100%;
    max-width: 280px;
    height: auto;
  }
  @media (max-width: 1200px) {
  .title h1 {
    font-size: 1.2em;
  }
  .titulQ {
    font-size: 1.2em;
    margin-bottom: 10px; /* Reduce el espacio debajo del título */
    padding-bottom: 5px; /* Ajusta el espacio interno */
  }
  .description2 {
    font-size: 1.9em;
    padding: 10px;
    margin: 5vw auto; /* Centra el texto */

  }
  .procedimiento {
    flex-direction: column; /* Apila el texto y la imagen verticalmente */
    align-items: center; /* Centra los elementos en pantalla */
  }

  .img-container2, .img-container3 {
    order: 2; /* Mueve las imágenes al final en dispositivos móviles */
    margin: 10px auto; /* Centra las imágenes */
    width: 90%; /* Ajusta el tamaño de las imágenes para móviles */
  }

  .procedimiento-text, .procedimiento-text1 {
    order: 1; /* Mueve el texto al inicio */
    width: 100%; /* Asegura que ocupe el 100% del ancho en móviles */
    text-align: center; /* Centra el texto */
    margin-top: -80px; /* Añade espacio entre el texto y la imagen */
  }
  .container2 {
    flex-direction: column; /* Apila la imagen y el texto */
    align-items: center; /* Centra los elementos */
  }
  .container-text1, .container-text2{
    font-size: 1.3em;
  }
}
</style>