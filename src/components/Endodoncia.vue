<template>
    <v-container>
      <v-row>
        <v-col cols="12">
        <div class="Endodoncia-container">
          <div class="image-section">
            <div class="image-container">
              <img class="main-image" src="@/assets/Endodoncia/Endo.jpg" alt="dientes" />
              <h1 class="title">Endodoncia</h1>
            </div>
          </div>

          <p class="description">
            Recuperar la salud dental y eliminar el dolor es posible gracias al tratamiento de endodoncia.
          </p>
          </div>
          </v-col>

          <v-col cols="12">
      <div class="container2">
          <div class="container-text">
            <p>
            Tener dientes dañados o con infección no solo genera molestias, sino
            que puede afectar gravemente nuestra calidad de vida. El dolor constante,
            la dificultad para masticar o hablar, y la preocupación por perder un diente pueden
            impactar en nuestra seguridad y autoestima. Una endodoncia permite salvar un diente
             natural, eliminando el dolor y la infección desde la raíz.
            </p>
          </div>
          <div class="img-container">
            <img src="@/assets/Endodoncia/Endo1.jpg" alt="Dientes">
          </div>
        </div>
    </v-col>

    <v-col cols="12">
        <div class="Endo-section">
          <h2 class="title2"> ¿Qué es la endodoncia? </h2>
          <div class="Endo-description">
            <p>
           La endodoncia se ocupa de preservar un diente que ha sido gravemente dañado
           o infectado. La pulpa dental puede inflamarse o infectarse debido a varias razones:
            </p>
            <img src="@/assets/Endodoncia/Endo2.jpg" alt="Dientes" />
          </div>
        </div>
      </v-col>

    <div class="Endo-description2">
    <ul>
        <li>Caries profundas.</li>
        <li>Traumatismos o fracturas del diente.</li>
        <li>Procedimientos dentales repetidos en el mismo diente.</li>
        <li>Grietas o fisuras.</li>
     </ul>
     </div>

    <!-- Pregunta desplegable -->
    <v-col cols="12">
    <div class="titul">
            <div class="titulQ"> ¡Tu salud dental es nuestra prioridad en Felizdent!</div>
          </div>
        <section class="questions">
            <div class="question blue" @click="toggleQuestion(1)">
              <h3>
                ¿Cuándo es necesaria una endodoncia?
                <span :class="{ expanded: activeQuestion === 1 }">+</span>
              </h3>
              <div v-if="activeQuestion === 1" class="answer">
                <hr class="divider" /> <!-- Línea divisoria -->
                <p>
                 Algunos de los síntomas que pueden indicar la necesidad de una endodoncia incluyen:
            <ul>
                <li>Dolor intenso al masticar o al presionar el diente.</li>
                <li>Sensibilidad prolongada al calor o al frío.</li>
                 <li>Decoloración del diente.</li>
                <li>Hinchazón en las encías cercanas al diente afectado.</li>
                <li>Presencia de una fístula (pequeña lesión en las encías por donde drena pus).</li>
            </ul>
                </p>
              </div>
            </div>
            </section>
        </v-col>

        <!-- Sección de tratamientos -->
      <v-col cols="12">
        <div class="tratamientos-section">
          <h1>Tratamientos dentales de FelizDent</h1>
          <h2 class="title3"> Apicoformación</h2>
          <div class="tratamiento-description">
            <p>
            Se realiza cuando la raíz de un diente no ha terminado de desarrollarse,
            lo que puede ocurrir en dientes jóvenes o inmaduros. La apicoformación
            estimula el desarrollo de la raíz y su cierre.
            </p>
            <img src="@/assets/Endodoncia/Endo3.jpg" alt="Dientes" />
          </div>
        </div>
      </v-col>

      <v-col cols="12">
        <div class="tratamientos-section2">
          <h2 class="title4"> Unirradiculares y multirradiculares</h2>
          <div class="tratamiento-description2">
            <div class="descrip2">
            <p>
            Los dientes pueden tener uno o varios conductos radiculares.
            Los tratamientos endodónticos se clasifican según la cantidad de raíces y conductos:

            <ul>
                <li>Unirradiculares: dientes con un solo conducto (como los dientes anteriores).</li>
                <li>Multirradiculares: dientes con múltiples conductos (como los molares).</li>
            </ul>
            </p>
        </div>
            <div class="img-container2">
            <img src="@/assets/Endodoncia/Endo4.jpg" alt="Dientes" />
         </div>
        </div>
        </div>
      </v-col>

      <v-col cols="12">
  <div class="tratamientos-section2">
    <h2 class="title4"> Apicectomías</h2>
    <div class="tratamiento-content">
      <div class="img-container3">
        <img src="@/assets/Endodoncia/Endo5.jpg" alt="Dientes" />
      </div>
      <div class="descrip3">
        <p>
          Es una cirugía que se realiza cuando el tratamiento de conductos convencional no ha sido suficiente para eliminar la infección. Se extirpa la punta de la raíz y el tejido circundante para eliminar la fuente de la infección.
        </p>
      </div>
    </div>
    </div>
  </v-col>
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
.Endodoncia-container {
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
    width: 100%; 
    height: auto; /* Mantiene la proporción de la imagen */
  }
  .title {
    position: absolute; /* Para el título */
    top: 50%; /* Centrar verticalmente */
    left: 50%; /* Centrar horizontalmente */
    transform: translate(-50%, -50%); /* Ajusta el centro del texto */
    background-color: #8A63F1; 
    color: white; 
    padding: 10px 20px; /* Espacio*/
    border-radius: 15px; 
    text-align: center;
    font-size: 2.6em; /* Tamaño del texto */
    font-weight: bold;
    border-radius: 17px;
  }
  .description {
    text-align: center;
    margin: 20px 0;
    line-height: 1.6;
    color: #27E1BC;
    font-weight: bold;
    font-size: 1.5em; /* Tamaño del texto */
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
    width: 100%; 
    max-width: 350px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
    margin-bottom: 20px; /* Agrega margen inferior */
  }
  .img-container {
  width: 30%; /* Ajusta el ancho de la imagen */
  max-width: 320px;
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
  .Endo-section {
    text-align: center;
    margin-top: -25px;
  }
  .title2 {
    color: #8A63F1;
    font-size: 2rem; 
    border-radius: 20px; 
    padding: 10px 20px; 
    display: inline-block; 
    margin-top: 80px; 
    font-style: italic; /* Aplica cursiva al texto */
    font-weight: bold;
  }
  .Endo-description {
    margin-top:  3vw; 
    font-size: 1.5rem; 
    font-style: italic;
  }
  .Endo-description img {
    width: 100%;
    max-width: 500px;
    height: auto;
    margin-top: 40px;
  }
  .Endo-description2 {
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
.titul{
  padding: 20px;
  margin-top: 80px;
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
.questions {
    margin-top: 20px;
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
  .title3 {
    background-color: #8A63F1; 
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
  .tratamientos-section2 {
    text-align: center;
    margin-top: -35px;
  }
  .title4 {
    background-color:#8A63F1; 
    color: rgb(0, 0, 0); 
    font-size: 1.5rem; 
    border-radius: 20px; 
    padding: 10px 20px; 
    display: inline-block; 
    margin-top: 90px; 
    font-weight: bold;
  }
  .tratamiento-description2{
    display: flex; /* alinea los elementos en fila */
    justify-content: space-between; /* espacio entre el texto y la imagen */
    align-items: flex-start;
    padding: 20px;
    flex-wrap: wrap;
    margin-top: 70px;
  }
  .descrip2 {
    width: 100%; 
    max-width: 310px;
    text-align: justify;
    box-sizing: border-box;
    margin-right: 0; /* Elimina el margen derecho */
    font-size: 1.3rem; 
    margin-bottom: 20px; /* Agrega margen inferior */
  }
  .img-container2 {
  width: 100%; /* Ajusta el ancho de la imagen */
  max-width: 220px;
  margin-right: 20px; /* Espacio a la derecha de la imagen */
  display: flex;
  align-items: flex-start; /* Asegura que la imagen también esté alineada con el texto */
}
  .img-container2 img {
  width: 100%;
  height: auto;
  margin-top: 0;
  object-fit: contain; 
  }
  .tratamiento-content {
    display: flex; /* alinea los elementos en fila */
    justify-content: space-between; /* espacio entre el texto y la imagen */
    padding: 20px;
    flex-wrap: wrap;
    margin-top: 70px;
  }
  .descrip3{
  max-width: 400px;
  margin-right: 20px; /* Espacio a la derecha de la imagen */
  display: flex;
  align-items: flex-start; /* El texto se alinea con la imagen */
}
  .descrip3 p{
  width: 100%;
  height: auto;
  margin-top: 0;
  object-fit: contain; 
  text-align: justify;
  font-size: 1.3rem; 
  }
  .img-container3 {
  width: 30%; /* Ajusta el ancho de la imagen */
  max-width: 320px;
  margin-right: 20px; /* Espacio a la derecha de la imagen */
  display: flex;
  align-items: flex-start; /* Asegura que la imagen también esté alineada con el texto */
}
  .img-container3 img {
  width: 100%;
  height: auto;
  margin-top: 0;
  object-fit: contain; 
  }

/* Media para hacer responsiva la página en moviles*/
@media (max-width: 768px) {
  .title {
    font-size: 1.8em; 
    padding: 8px 15px;
  }
  .image-container {
    width: 100%;
  }
  .container2, .Endo-description, .tratamientos-section, .tratamiento-description, .tratamiento-description2, .tratamiento-content {
    flex-direction: column; /* Cambia de fila a columna */
    align-items: center; /* todo esta centrado */
    text-align: center;
  }
  .img-container, .img-container2{
    width: 100%; 
    max-width: 100%;
    margin: 0 auto; 
  }
  .img-container3{
    width: 100%; 
    max-width: 100%;
    margin: 0 auto; 
    margin-top: -55px; 
  }
  .container-text{
    width: 100%; 
    margin-right: 0; 
    font-size: 1.3em;
    margin-top: -30px; 
  }
  .descrip2{
    width: 100%; 
    margin-right: 0; 
    margin-top: -55px; 
    font-size: 1.4em; 
  }
  .descrip3 {
    width: 100%; 
    margin-right: 0;
    margin-top: 55px; 
  }
  .Endodoncia-container, .tratamientos-section {
    padding: 10px; 
  }
  ul {
    margin-left: 20px; /* Reduce el margen de las listas */
  }
  .title2{
   font-size: 1.6rem;
  }
  .titulQ {
    font-size: 1.2em;
  }
}

/* Media para hacer responsiva la página (1200) Tablets*/
  @media (max-width: 1200px) {
  .title {
    font-size: 1.8em;
    padding: 8px 15px;
  }
  .container-text{
  width: 100%; /* El texto ocupará el 100% del ancho */
  max-width: none; /* Sin ancho */
  font-size: 1.5em; 
}
  .image-container {
    width: 100%; 
  }
  .container2, .Endo-description, .tratamientos-section, .tratamiento-description, .tratamiento-description2, .tratamiento-content {
    flex-direction: column; /* Cambia de fila a columna */
    align-items: center; /* Asegura que todo esté centrado */
    text-align: center;
  }
  .img-container{
    width: 100%;
    max-width: 100%;
    margin: 0 auto; /* Centra las imágenes */
  }
  .img-container2{
    width: 100%; 
    max-width: 75%;
    margin: 0 auto; 
  }
  .img-container3{
    width: 100%; /* La imagen ocupa el 100% del contenedor */
    max-width: 100%;
    margin: 0 auto; /* Centra las imágenes */
    margin-top: -55px; 
  }
  .descrip2{
    width: 100%; /* El texto ocupará el 100% del ancho */
    max-width: none; /* Sin ancho */
    font-size: 1.4em; 
  }
  .descrip3 {
    width: 100%; /* El texto ocupará el 100% del ancho */
    max-width: none; /* Sin ancho */
    margin-top: 55px; 
  }
  .descrip3 p{
    font-size: 1.5em; 
  }
  .Endodoncia-container, .tratamientos-section {
    padding: 10px; /* Reduce el padding en pantallas pequeñas */
  }
  .description {
    font-size: 1.4em;
  }
  ul {
    margin-left: 20px; 
  }
  .title2{
   font-size: 1.6rem;
  }
  .title3, .title4 {
    font-size: 1.3rem; 
    margin-top: 20px; /* Reduce el margen superior */
  }
  .questions .question h3 {
    font-size: 1.4em; 
  }
  .question p {
    font-size: 1.4em; 
  }
  .titulQ {
    font-size: 1.2em; 
  }
 .tratamientos-section h1{
  font-size: 1.5em; 
  margin-top:-40px; 

  }
  .answer{
    text-align: justify
  }
  .tratamiento-description p{
    text-align: justify
  }
  }
</style>