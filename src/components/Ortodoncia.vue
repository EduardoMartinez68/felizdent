<template>
    <v-container>
        <v-row>
    <v-col cols="12">
        <div class="ortodoncia-container">
          <!-- Sección de la imagen principal -->
          <div class="image-section">
            <div class="image-container">
              <img class="main-image" src="@/assets/Ortodoncia/Orto.jpg" alt="Dentadura" />
              <h1 class="title">Ortodoncia y Ortopedia Maxilar </h1>
            </div>
          </div>

          <p class="description">
            Perfeccionamos tu sonrisa para hacerla brillar
          </p>
        </div>
      </v-col>

      <v-col cols="12">
      <div class="container2">
          <div class="container-text">
            <p>
            Disfrutar de una sonrisa perfecta es posible con el tratamiento de ortodoncia
            que mejor se adecúe a tu salud bucodental. La sociedad es cada vez más exigente,
            y nuestras relaciones sociales se ven condicionadas por muchos factores, entre
            ellos nuestro aspecto. Una sonrisa sana y natural es uno de los principales puntos
            que nos ayuda a mantener nuestra seguridad en el día a día y cuidar de nuestra calidad
            de vida. Pero muchas personas no cuentan con esa seguridad. Las imperfecciones presentes
            en la sonrisa pueden causarnos inseguridad, y puede afectar a nuestra autoestima o a
            nuestra relación con los demás. Del mismo modo, cualquier alteración en la mandíbula
            puede afectar nuestra propia respiración.
            </p>
          </div>
          <div class="img-container">
            <img src="@/assets/Ortodoncia/Orto1.jpg" alt="Dentista trabajando">
          </div>
        </div>
    </v-col>

     <!-- Pregunta desplegable -->
     <v-col cols="12">
          <section class="questions">
            <div class="question blue" @click="toggleQuestion(1)">
              <h3>
                ¿Qué es la ortodoncia?
                <span :class="{ expanded: activeQuestion === 1 }">+</span>
              </h3>
              <div v-if="activeQuestion === 1" class="answer">
                <hr class="divider" /> <!-- Línea divisoria -->
                <p>
                La ortodoncia es la especialidad de la odontología que se encarga de corregir
                las malposiciones o desviaciones de los dientes y deformidades de los maxilares.
                La ortodoncia solventa problemas dentales como la mordida cruzada, la mordida abierta
                o profunda y los dientes apiñados o separados, entre otros.
                </p>
              </div>
            </div>
            </section>
            </v-col>

        <!-- Sección de tratamientos -->
      <v-col cols="12">
        <div class="tratamientos-section">
          <h1>Tratamientos dentales de FelizDent</h1>
          <h2 class="title2"> Brackets Convencionales</h2>
          <div class="tratamiento-description">
            <p>
            Son los brackets metálicos tradicionales que  se ajustan  el arco metálico a cada bracket.
            Es uno de los métodos más comunes para corregir la alineación de los dientes.
            </p>
            <img src="@/assets/Ortodoncia/Orto2.jpg" alt="Brackets" />
          </div>
        </div>
      </v-col>

      <v-col cols="12">
        <div class="tratamientos-section1">
          <h2 class="title2"> Técnica de Autoligado</h2>
          <div class="tratamiento-description">
            <p>
            Es una técnica donde se emplean brackets especiales que no requieren el uso
            de ligaduras elásticas para sostener el arco. Esto permite que los dientes
            se muevan más libremente y con menos fricción.
            </p>
            <img src="@/assets/Ortodoncia/Orto3.jpg" alt="Brackets" />
          </div>
          </div>
      </v-col>

      <v-col cols="12">
        <div class="tratamientos-section1">
          <h2 class="title2"> Brackets Estéticos </h2>
          <div class="tratamiento-description">
            <p>
            Son una variante de los brackets convencionales, pero están hechos de materiales
            como la porcelana o el zafiro, que se asemejan al color natural de los dientes.
            </p>
            <img src="@/assets/Ortodoncia/Orto4.jpg" alt="Brackets" />
          </div>
          </div>
         </v-col>

         <v-col cols="12">
        <div class="tratamientos-section1">
          <h2 class="title2"> Brackets Linguales </h2>
          <div class="tratamiento-description">
            <p>
            Son brackets que se colocan en la parte interna de los dientes
            (por el lado de la lengua), lo que los hace prácticamente invisibles desde el exterior.
            </p>
            <img src="@/assets/Ortodoncia/Orto5.jpg" alt="Brackets" />
          </div>
          </div>
         </v-col>

      
      <v-col cols="12">
        <div class="DentAli-section">
          <h2 class="title3"> ¿Qué puede ocurrir si mi dentadura no está alineada?</h2>
          <div class="tratamiento-description2">
            <p>
              Una dentadura no alineada, en un principio, puede ocasionar molestias al
              masticar y hasta al hablar. Esto, a largo plazo, puede generar problemas
              en el sistema masticatorio– nuestra mandíbula – y en el sistema nervioso.
              Pero, además, pueden surgir otra serie de problemas:
            </p>
            <img src="@/assets/Ortodoncia/Orto6.jpg" alt="Dientes" />
          </div>
        </div>
      </v-col>

      <div class="tratamiento-description3">
    <ul>
      <li>Una alteración en la mandíbula puede dificultar hábitos como la respiración.</li>
      <li>La falta de desarrollo de los dientes puede causar apiñamiento dental.</li>
      <li>Alteración del crecimiento de huesos de la cara, como el prognatismo mandibular.</li>
      <li>Una malposición dental puede generar contracturas musculares, o tensión muscular en zonas como la espalda y el cuello. También puede dar lugar a vértigo o zumbidos.</li>
      <li>Pueden aparecer dolores de cabeza, migrañas, y hasta cefalea de origen dental.</li>
      <li>El estrés puede causar todavía mayor tensión muscular, y agravar los desórdenes presentes en la mandíbula.</li>
      <li>Afecta la articulación temporomandibular.</li>
    </ul>
  </div>

  <div class="beneficios-ortodoncia">
    <h2>Beneficios de la ortodoncia</h2>
    <div class="beneficios-container">
      <div class="beneficio-cuad cuad1">
        <p>
          La ortodoncia, como beneficio principal, corrige la posición de los dientes
          superiores e inferiores. Esto, en primer lugar, permite que hábitos como masticar o hablar
          se desarrollen con total normalidad. Tener una correcta funcionalidad de los dientes
          y una buena técnica de mordida, evitará problemas y malformaciones en nuestra mandíbula.
        </p>
      </div>
      <div class="beneficio-cuad cuad2">
        <p>
          La correcta posición de los dientes permite que el cepillado de los dientes sea más
          efectivo, lo que favorece la higiene bucodental. Del mismo modo, la alineación correcta
          de los dientes aporta un aspecto saludable y armonioso a nuestra sonrisa, lo que
          beneficia a nuestra estética y también a nuestra autoestima.
        </p>
      </div>
      <div class="beneficio-cuad cuad3">
        <p>
          Es por eso que la ortodoncia se ha convertido en una solución ideal no solo para niños,
          sino también para adultos y para personas mayores. La existencia de materiales y
          prácticas que disimulan el tratamiento de ortodoncia anima cada vez a más personas a
          recurrir a esta para conseguir todos estos beneficios para su sonrisa.
        </p>
      </div>
    </div>
  </div>

  <v-col cols="12">
        <div class="OrtoMax">
          <h2 class="title4"> Ortopedia Maxilar</h2>
          <div class="tratamiento-description4">
            <p>
            Se enfoca en modificar el crecimiento óseo de los maxilares y la mandíbula
            en pacientes jóvenes, generalmente antes de que hayan completado su crecimiento.
            </p>
            <img src="@/assets/Ortodoncia/Orto7.jpg" alt="Dientes" />
          </div>
        </div>
      </v-col>

      <v-col cols="12">
        <div class="OrtoMax1">
          <h2 class="title5"> ¿Cómo funciona la Ortopedia Maxilar?</h2>
          <div class="tratamiento-description5">
            <p>
            La ortopedia maxilar se basa en el uso de dispositivos ortopédicos, que son aparatos
            diseñados para modificar o guiar el crecimiento óseo. Estos dispositivos pueden ser:
            </p>
            <img src="@/assets/Ortodoncia/Orto8.jpg" alt="Dientes" />
          </div>
        </div>
      </v-col>

      <div class="tratamiento-description3">
    <ul>
      <li>Fijos o removibles, dependiendo del caso.</li>
      <li>Funcionales, diseñados para utilizar la propia fuerza muscular del paciente
        (al masticar o hablar) para guiar el crecimiento óseo de manera adecuada.</li>
      </ul>  
  </div>
  </v-row>
  </v-container>
</template>

<script>
 export default {
    data() {
      return {
        activeQuestion: null,
      };
    },
    methods: {
      toggleQuestion(questionNumber) {
        this.activeQuestion = this.activeQuestion === questionNumber ? null : questionNumber;
      },
    },
  };
</script>

<style scoped>
.ortodoncia-container {
    padding: 20px;
    font-family: 'Arial', sans-serif;
    margin-top: 110px;
  }
  .image-section {
    display: flex;
    flex-direction: column;
    align-items: center;
  }
  .image-container {
   position: relative; /* Para poner el título sobre la imagen */
   width: 100%; /* La imagen ocupa el 100% del ancho */
   max-width: 100vw; /* tamaño en unidades relativas */
  }
  .main-image {
    width: 100%; /* la imagen ocupa el 100% */
    height: auto; /* Mantiene la proporción de la imagen */
  }
  .title {
    position: absolute; /* Para el título */
    top: 50%; /* Centrar verticalmente */
    left: 50%; /* Centrar horizontalmente */
    transform: translate(-50%, -50%); /* Ajusta el centro del texto */
    background-color:#8A63F1; 
    color: white; 
    padding: 10px 20px; /* Espacio*/
    border-radius: 15px; 
    text-align: center;
    font-size: 2.1em; /* Tamaño del texto */
    font-weight: bold;
  }
  .description {
    text-align: center;
    margin: 20px 0;
    line-height: 1.6;
    color: #27E1BC;
    font-weight: bold;
    font-size: 1.5rem; 
    margin-top: 50px;
  }
  .container2 {
    display: flex; /* alinea los elementos en fila */
    justify-content: space-between; /* espacio entre el texto y la imagen */
    align-items: flex-start;
    padding: 20px;
    flex-wrap: wrap;
    margin-top: 70px;
  }
  .container-text {
    width: 100%; /* Asegura que ocupe el 100% en pantallas pequeñas */
    max-width: 450px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
    margin-bottom: 20px; /* Agrega margen inferior */
  }
  .img-container {
  width: 40%; /* Ajusta el ancho de la imagen */
  max-width: 400px;
  margin-right: 20px; /* Espacio a la derecha de la imagen */
  display: flex;
  align-items: flex-start; /* Asegura que la imagen también esté alineada con el texto */
}
  .img-container img {
  width: 100%;
  height: auto;
  margin-top: 0;
  object-fit: contain; 
  }
  .questions {
    margin-top: 50px;
    width: 100%;
  }
  .questions .question {
    padding: 30px;
    border-radius: 5px;
    border: 1px solid #ddd;
    cursor: pointer;
  }
  .questions .question.blue {
    background-color: #27e1bc;
  }
  .questions .question h3 {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-size: 18px;
    color: #000000;
    font-size: 1.5em;
    font-weight: bold;
  }
  .questions .question h3 span {
    transition: transform 0.3s ease;
  }
  .questions .question h3 span.expanded {
    transform: rotate(45deg);
    font-weight: bold;
  }
  .answer {
    margin-top: 10px;
    padding: 10px;
    border-radius: 5px;
    display: block;
    transition: all 0.3s ease;
    width: 100%;
  }
  .divider {
    border: 0;
    height: 1.5px;
    background: #000000;
    margin-bottom: 10px;
  }
  .tratamientos-section {
    text-align: center;
    margin-top: 135px;
    
  }
  .tratamientos-section h1{
    font-weight: bold;
  }
  .title2 {
    background-color:#8A63F1; 
    color: rgb(0, 0, 0); 
    font-size: 1.5rem; 
    border-radius: 20px; 
    padding: 10px 20px; 
    display: inline-block; 
    margin-top: 90px; 
    font-weight: bold;
  }
  .tratamiento-description {
    margin-top:  3vw; 
    font-size: 1.5rem; 
  }
  .tratamiento-description img {
    width: 100%;
    max-width: 500px;
    height: auto;
    margin-top: 40px;
  }
  .tratamientos-section1 {
    text-align: center;
    margin-top: 20px;
  }
  .DentAli-section {
    text-align: center;
    margin-top: 20px;
  }
  .title3 {
    color: rgb(0, 0, 0); 
    font-size: 1.5rem; 
    border-radius: 20px; 
    padding: 10px 20px; 
    display: inline-block; 
    margin-top: 80px; 
    font-style: italic; /* Aplica cursiva al texto */
    font-weight: bold;
  }
  .tratamiento-description2 {
    margin-top: 1.5vw; /* Reducir margen superior */
    font-size: 1.5rem;
    line-height: 1.5; 
    max-width: 450px; /*ancho del texto */
    margin-left: auto; /* Centrar el texto */
    margin-right: auto; /* Centrar el texto */
    text-align: center;
    padding: 0 10px; /* Añadir un pequeño padding lateral */
    font-style: italic; /* Aplica cursiva al texto */
  }
  .tratamiento-description2 img {
    width: 100%;
    max-width: 500px;
    height: auto;
    margin-top: 40px;
  }
  .tratamiento-description3 {
    margin-top: 50px;
    font-size: 1.5rem;
    font-style: italic;
    max-width: 600px;
    margin-left: auto;
    margin-right: auto;
    text-align: justify;
    padding: 0 10px;
}
ul {
    list-style-type: disc; /* Puntos, para la lista*/
    margin-left: 20px;
}
.beneficios-ortodoncia {
  text-align: center;
  margin-top: 120px;
}
.beneficios-ortodoncia h2 {
  font-size: 2rem;
  margin-bottom: 40px;
  font-weight: bold;
}
.beneficios-container {
  display: flex;
  justify-content: space-between; 
  align-items: stretch; /* todas las tarjetas tienen la misma altura */
  gap: 20px;
  flex-wrap: wrap; /* Ajuste en pantallas más pequeñas */
}
.beneficio-cuad {
  width: 30%;
  padding: 20px;
  border-radius: 10px;
  font-size: 1rem;
  line-height: 1.5;
  text-align: justify;
  min-height: 270px; /* Altura mínima para igualar las tarjetas */
  display: flex;
  text-align: center;
  flex-direction: column;
}
.cuad1 {
  background-color: #27e1bc; /* Color del primer cuadro */
  color: black;
}
.cuad2 {
  background-color: #d9d9d9; /* Color del segundo Cuadro */
  color: black;
}
.cuad3 {
  background-color:#8A63F1; /* Color del tercer Cuadro */
  color: black;
}
.OrtoMax{
    text-align: center;
    margin-top: 50px;
  }
  .title4 {
    color: #27e1bc;
    font-size: 3rem; 
    border-radius: 20px; 
    padding: 10px 20px; 
    display: inline-block; 
    margin-top: 80px; 
    font-weight: bold;
  }
  .tratamiento-description4 {
    margin-top:  3vw; 
    font-size: 1.5rem;  
  }
  .tratamiento-description4 img {
    width: 100%;
    max-width: 500px;
    height: auto;
    margin-top: 40px;
  }
  .OrtoMax1{
    text-align: center;
    margin-top: 10px;
  }
  .title5 {
    color: rgb(0, 0, 0); 
    font-size: 1.8rem; 
    border-radius: 20px; 
    padding: 10px 20px; 
    display: inline-block; 
    margin-top: 80px; 
    font-weight: bold;
  }
  .tratamiento-description5 {
    margin-top:  3vw; 
    font-size: 1.5rem; 
    font-style: italic; /* Aplica cursiva al texto */
  }
  .tratamiento-description5 p {
    text-align: justify;
  }
  .tratamiento-description5 img {
    width: 100%;
    max-width: 500px;
    height: auto;
    margin-top: 40px;
  }
/* Ajustes para pantallas pequeñas */
@media (max-width: 768px) {
  .title {
    font-size: 1.5em;
    padding: 8px 15px;
  }
  .description {
    font-size: 1.5rem; 
    margin-top: 20px;
  }
  .tratamiento-description img {
    width: 100%;
    height: auto;
  }
  .tratamiento-description,
  .tratamiento-description2,
  .tratamiento-description3 {
    flex-direction: column;
  }
   .tratamientos-section{
    margin-top: 80px;
   }
   .title2{
    margin-top: 50px;
   }
   .tratamientos-section1 {
    padding: 15px;
  }
  .container2 {
      flex-direction: column; /* Cambia a columna en pantallas pequeñas */
      align-items: center; /* Centra los elementos */
      padding: 15px;
      margin-top: 20px;
    }
    .img-container {
        width: 100%; /* Asegura que ocupe el 100% en pantallas pequeñas */
        max-width: 300px; /* Ajusta el tamaño máximo para pantallas pequeñas */
        margin: 0 auto; /* Centra la imagen en dispositivos móviles */
    }

  .beneficios-container {
    flex-direction: column;
    gap: 10px;
  }

  .beneficio-cuad {
    width: 100%;
    text-align: justify;
    font-size: 1.2rem;
  }
  .answer p {
    font-size: 14px; /* Ajusta el tamaño del texto en la respuesta */
    text-align: justify;
  }
  .container-text{
    max-width: 100%;
    margin-top: -20px;
    font-size: 1.2rem; 
  }
}

/* Ajustes para pantallas pequeñas */
@media (max-width: 1200px) {
  .answer p {
    font-size: 20px; /* Ajusta el tamaño del texto en la respuesta */
    text-align: justify;
  }
  .title {
    font-size: 1.5em;
    padding: 8px 15px;
  }
  .description {
    font-size: 1.2em;
    margin-top: 20px;
  }
  .tratamiento-description img {
    width: 100%;
    height: auto;
  }
  .tratamiento-description,
  .tratamiento-description2,
  .tratamiento-description3 {
    flex-direction: column;
  }
   .tratamientos-section{
    margin-top: 80px;
   }
   .title2{
    margin-top: 50px;
   }
   .tratamientos-section1 {
    padding: 15px;
  }
  .container2 {
      flex-direction: column; /* Cambia a columna en pantallas pequeñas */
      align-items: center; /* Centra los elementos */
      padding: 15px;
      margin-top: 20px;
    }
    .img-container {
        width: 100%; /* Asegura que ocupe el 100% en pantallas pequeñas */
        max-width: 300px; /* Ajusta el tamaño máximo para pantallas pequeñas */
        margin: 0 auto; /* Centra la imagen en dispositivos móviles */
    }

  .beneficios-container {
    flex-direction: column;
    gap: 10px;
    align-items: center; 
  }

  .beneficio-cuad {
    width: 80%;
  }
}
/* Ajustes específicos para pantallas más pequeñas (móviles) */
@media (max-width: 480px) {
  .title {
    font-size: 1.2em;
    padding: 5px 10px;
  }
  .description {
    font-size: 1.4em;
  }

  .tratamiento-description img {
    width: 100%;
    height: auto;
  }

  .tratamiento-description p {
    font-size: 0.9em;
  }

  .tratamientos-section h1, .title2, .title3, .title4, .title5 {
    font-size: 1.4em;
  }

  .container2, .tratamientos-section, .tratamientos-section1 {
    padding: 10px;
  }

  .title4{
    font-size: 2rem; 
  }
}
@media (max-width: 600px) {
    .title {
      font-size:1rem;/* Tamaño reducido para pantallas pequeñas */
    }
}
@media (max-width: 380px) {
    .title {
      font-size: 0.7rem;/* Tamaño reducido para pantallas pequeñas */
    }
}
@media (max-width: 250px) {
    .title {
      font-size: 0.4rem;/* Tamaño reducido para pantallas pequeñas */
    }
}
</style>