
<template>

<!-- Historia de la Clínica -->
<v-container>
      <v-row>
    <section class="hero">
      <div class="content">
        <h1>FelizDent</h1>
        <h2>Por el gusto de verte sonreír</h2>
        <p>Felizdent es una clínica dental en con más de 20 años de experiencia, ofreciendo soluciones dentales innovadoras con tratamientos innovadores y mínimamente invasivos.
        Utilizamos materiales de última generación y contamos con un equipo de odontólogos especializados en periodoncia, estética dental, ortodoncia
        y odontopediatría, comprometidos con brindarte el mejor cuidado para tu salud bucal.</p>
        <img src="@/assets/imagenesC/especialistasabril2026.jpeg" alt="Consultorio dental">
      </div>
    </section>
    </v-row>
    </v-container>

     <!-- Carrusel "Servicios" -->
     <v-row>
      <v-container>
     <div class="especialidades-container">
      <div class="carrusel">
        <div
          v-for="especialidad in especialidades"
          :key="especialidad.id"
          class="imagen-contenedor"
          @click="irADetalle(especialidad)"
        >
          <img :src="especialidad.imagen" alt="Especialidad" class="imagen">
          <div class="nombre-overlay">{{ especialidad.nombre }}</div>
        </div>
      </div>
    </div>
  </v-container>
   </v-row>
   

     <!-- Dentistas" -->
    <v-container>
    <div class="doctors-gallery">
    <h2>Conoce a nuestro equipo de dentistas</h2>

     <!-- Tarjeta 1 -->
      <v-row>

  <!-- Tarjeta 3 -->
  <v-col cols="12" md="4">
  <div class="card">
      <div class="card-inner" :class="{ flipped: isFlipped3 }">
        <!-- Cara delantera -->
        <div class="card-front">
          <img src="@/assets/Imagenes/docisa.jpg" alt="Imagen del Dentista" class="card-img3">
          <div class="card-content">
            <h3>Dra. Isabel Chávez </h3>
            <h4>Estomatología Pediátrica </h4>
            <hr class="custom-line3"> <!-- Línea horizontal -->
            <div class="text-with-images">
              <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
              <div class="text-content">
                <p class="justified-text">
                  Lic. En Estomatología por la “Benemérita Universidad Autónoma de Puebla” 2002 a 2006.
                </p>
              </div>
            </div>
            <div class="text-with-images">
              <img src="@/assets/Imagenes/dentist11.jpg" alt="Logo" class="small-img">
              <div class="text-content">
                <p class="justified-text">
                  Especialidad en Estomatología Pediátrica “Hospital para el Niño Poblano” 2009 a 2011.
                </p>
              </div>
            </div>
            <div class="button">
              <button class="btn-primary3v" @click.stop="flipCard3">Ver más</button>
            </div>
          </div>
        </div>

        <!-- Cara trasera -->
        <div class="card-back">
          <div class="card-back-content">
            <h3>Diplomados</h3>
            <div class="text-with-images3">
              <img src="@/assets/Imagenes/dentist3.jpg" alt="Logo" class="small-img">
              <div class="text-content3">
                <p class="justified-text">
                  Diplomado en Investigación Clínica "Benemérita Universidad Autónoma de Puebla" 2009- 2010 (240 hrs).

                </p>
              </div>
            </div>
            <div class="text-with-images3">
              <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
              <div class="text-content3">
                <p class="justified-text">
                  Diplomado de Ortopedia Maxilar con Aplicación Clínica En la "Benemérita Universidad Autónoma de Puebla" (campus Tehuacán)
                  2019- 2021.

                </p>
              </div>
            </div>
            <div class="text-with-images3">
              <img src="@/assets/Imagenes/dentist3.jpg" alt="Logo" class="small-img">
              <div class="text-content3">
                <p class="justified-text">
                  Diplomado de Actualización Ortopedia y Odontopediatría "Desarrollo Especializado con Nuevas Técnicas de Actualizaciòn"
                  2021-2022.

                </p>
              </div>
            </div>

            <div class="button-container">
              <button class="btn-primary3" @click.stop="flipCard3">Volver</button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </v-col>

    <!-- Tarjeta 4 -->
   <v-col cols="12" md="4">
  <div class="card">
      <div class="card-inner" :class="{ flipped: isFlipped4 }">
        <!-- Cara delantera -->
        <div class="card-front">
          <img src="@/assets/Imagenes/dentistY.jpg" alt="Imagen del Dentista" class="card-img4">
          <div class="card-content">
            <h3>Dra. Yazmin Téllez Bautista </h3>
            <h4>Estomatología y Especialista en Endodoncia</h4>
            <hr class="custom-line4"> <!-- Línea horizontal -->
            <div class="text-with-images">
              <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
              <div class="text-content">
                <p class="justified-text">
                  Lic. En Estomatología por la “Benemérita Universidad Autónoma de Puebla” 1998-2003.
                </p>
              </div>
            </div>
            <div class="text-with-images">
              <img src="@/assets/Imagenes/dentist12.jpg" alt="Logo" class="small-img">
              <div class="text-content">
                <p class="justified-text">
                  Especialidad en endodoncia por “Centro Mexicano en estomatologia”2009 a 2011”.
                </p>
              </div>
            </div>
            <div class="button">
              <button class="btn-primary4v" @click.stop="flipCard4">Ver más</button>
            </div>
          </div>
        </div>

        <!-- Cara trasera -->
        <div class="card-back">
          <div class="card-back-content">
            <h3>Diplomados</h3>
            <div class="text-with-images4">
              <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
              <div class="text-content4">
                <p class="justified-text">
                  Diplomado de medicina interna en Estomatología en “Benemérita Universidad
              Autónoma de puebla” 2012-2013.

                </p>
              </div>
            </div>
            <div class="text-with-images4">
              <img src="@/assets/Imagenes/dentist3.jpg" alt="Logo" class="small-img">
              <div class="text-content4">
                <p class="justified-text">
              Diplomado en Diagnóstico y Tratamientos básicos Periodontales en “Benemérita
              Universidad Autónoma de Puebla” abril 2015-febrero 2016.

                </p>
              </div>
            </div>
            <div class="text-with-images4">
              <img src="@/assets/Imagenes/dentist13.jpg" alt="Logo" class="small-img">
              <div class="text-content4">
                <p class="justified-text">
               Diplomado en Odontología Estetica y Restauradora en "Colegio Dental del Estado de Mexico, A.C" 2022. 
                </p>
              </div>
            </div>
            <div class="text-with-images4">
              <img src="@/assets/Imagenes/dentist15.jpg" alt="Logo" class="small-img">
              <div class="text-content4">
                <p class="justified-text">
                   Diplomado en Cirugía Plástica Periodental en "Colegio de Actualización Profesional Tepeaca"2024.

                </p>
              
            </div>
          </div>

            <div class="button-container">
              <button class="btn-primary4" @click.stop="flipCard4">Volver</button>
            </div>
          </div>
        </div>
      </div>
    </div>
   </v-col>

    <!-- Tarjeta 5 -->
    <v-col cols="12" md="4">
  <div class="card">
      <div class="card-inner" :class="{ flipped: isFlipped5 }">
        <!-- Cara delantera -->
        <div class="card-front">
          <img src="@/assets/Imagenes/dentistBr.jpg" alt="Imagen del Dentista" class="card-img5">
          <div class="card-content">
            <h3>Dra. Bricia Pascuala López López</h3>
            <h4>Estomatología</h4>
            <hr class="custom-line5"> <!-- Línea horizontal -->
            <div class="text-with-images">
              <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
              <div class="text-content">
                <p class="justified-text">
                  Lic. en Estomatología por la “Benemérita Universidad Autónoma de Puebla” 2008 a 2013.
                </p>
              </div>
            </div>

            <div class="button">
              <button class="btn-primary5v" @click.stop="flipCard5">Ver más</button>
            </div>
          </div>
        </div>

        <!-- Cara trasera -->
        <div class="card-back">
          <div class="card-back-content">
            <h3>Diplomados</h3>
            <div class="text-with-images5">
              <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
              <div class="text-content5">
                <p class="justified-text">
                  Diplomado de medicina interna en Estomatología avalada por
                   "Benemérita Universidad Autónoma de Puebla” 2019-2020. 

                </p>
              </div>
            </div>
            <div class="text-with-images5">
              <img src="@/assets/Imagenes/dentist15.jpg" alt="Logo" class="small-img">
              <div class="text-content5">
                <p class="justified-text">
                  Diplomado de Biocosmética Dental por el “Colegio de Actualización
                   de Tepeaca” octubre 2021-septiembre a 2022.
                </p>
              </div>
            </div>
            <div class="text-with-images5">
              <img src="@/assets/Imagenes/dentist15.jpg" alt="Logo" class="small-img">
              <div class="text-content5">
                <p class="justified-text">
                  Diplomado en Prostodoncia Total por “Colegio de Actualización
                   de Tepeaca” noviembre 2022 a junio 2022. 

                </p>
              
            </div>
          </div>

            <div class="button-container">
              <button class="btn-primary5" @click.stop="flipCard5">Volver</button>
            </div>
          </div>
        </div>
      </div>
    </div>
    </v-col>

    <!-- Tarjeta 6 -->
   
</v-row>
<div class="button-container1">
    <button class="boton-conoce-mas" @click="conoceMas">Conoce más</button>
  </div>
</div>
</v-container>


<!-- Filosofía -->
<v-container>
 <v-row>
<div class="filosofia-container">
  <h2>Conoce nuestra filosofía</h2>
  <p>Descubre qué nos motiva y guía en Felizdent. Nuestra misión,</p>
    <div class="texto2"> visión y valores reflejan nuestro compromiso con tu salud dental y bienestar.</div>
    

  <div class="misvis-section">
    <div class="misvis-item">
      <img src="@/assets/ImagenesP/mision.jpg" alt="Paciente sonriendo">
      <div class="misvis-text1">
        <h3> VISIÓN</h3>
        <p>Para el 2030 ser una clínica dental líder en la región,
 reconocida por brindar servicios dentales integrales,
 personalizados de excelencia y con el compromiso
 social de la comunidad. </p>
      </div>
    </div>

    <div class="misvis-item">
      <div class="misvis-text">
        <h3> MISIÓN</h3>
        <p>Transformar vidas a través de sonrisas
 saludables y esteticas; mejorando su autoestima, concientizando la importacia de la salud bucal, apoyados de un equipo de
 especialistas altamente calificados, aplicando
 innovación tecnológica, trato humano, para
 ofrecer soluciones integrales, personalizadas y
 con la confianza de estar en las mejores manos. </p>
      </div>
      <img src="@/assets/ImagenesP/vision.jpg" alt="Dentista trabajando">
    </div>
  </div>
  <div class="content1">
        <img src="@/assets/ImagenesP/dentI.jpg" alt="Consultorio dental">
  </div>
</div>
</v-row>
</v-container>


 <!-- Sección de los valores -->
 <v-container>
  <v-row>
 <div class="valores-container">
    <h2>Valores</h2>
    <ul class="valores-list">
      <li v-for="valor in valores" :key="valor.nombre">
        <strong :style="{ color: valor.color }">{{ valor.nombre }}:</strong> {{ valor.descripcion }}
      </li>
    </ul>
  </div>

  <!-- Imagen del logo -->
  <div class="logo-container">
    <img src="@/assets/ImagenesP/logonu.jpg" alt="Felizdent Logo" class="logo-felizdent">
  </div>
  </v-row>
  </v-container>

<!--Seción de los Vídeos Testimoniales -->
<v-container> 
  <div class="testimonials-section">
    <div class="Blue-container">
    <h2>Conoce testimonios de nuestros pacientes</h2>
  </div>

    <!-- Contenedor verde para la interfaz -->
    <div class="green-container">

      <!-- Primera fila -->
      <div class="row">
        <div class="video-box">
          <iframe
            :src="videos[0].url"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
        <div class="blue-box">
          <p> RESINAS</p>
        </div>
      </div>

      <!-- Segunda fila-->
      <div class="row">
        <div class="blue-box">
          <p>CORONAS ESTETICAS</p>
        </div>
        <div class="video-box">
          <iframe
            :src="videos[1].url"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </div>
      
      <!-- Botón "Conoce más" -->
      <div class="button-container1">
        <button class="boton-conoce-mas" @click="conoceMas">Conoce más</button>
      </div>
    </div>
  </div>
</v-container>

   <!--Seción de los comentarios-->
  
  

  <!-- Ubicación de  "San Lorenzo" -->
      <v-container>
      <v-row>
      <v-col>
         <div class="direccion-boton-contenedor">
          <img src="@/assets/ImagenesP/ubicacion.jpg" alt="Icono de dirección" class="icono-direccion" />
          <p class="direccion">{{ address }}</p>

          <!-- Botón "Ver más sucursales" con imagen -->
          <img src="@/assets/ImagenesP/ub.jpg" alt="Icono de ver más" class="icono-boton" />
          <button class="boton-ver-mas-sucursales" @click="vermasucursales">Ver más sucursales</button>
        </div>
       
      <!-- Contenedor principal: Imagen y mapa -->
      <div class="image-and-map">
        <!-- Imagen del consultorio -->
        <div class="image-container">
          <img src="@/assets/ImagenesC/consulSan.jpg" alt="Imagen de la clínica" class="clinica-img">
        </div>
  
        <!-- Mapa de Google Maps del consultorio -->
        <div class="map-container">
          <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d17961.06298242009!2d-97.86873282089783!3d18.84940874728674!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x85cf88b8922ed7d7%3A0xc2f1398865f4100f!2sFelizdent%20Clinica%20Dental!5e0!3m2!1ses!2smx!4v1725846544334!5m2!1ses!2smx"
            class="map-frame" allowfullscreen="" loading="lazy" referrerpolicy="no-referrer-when-downgrade">
          </iframe>
        </div>
      </div>
    </v-col>
    </v-row>
    </v-container>
<v-container class="mt-10">
  <iframe
      src="https://app.denty.cloud/profile_online/company_widget/10/"
      style="
        width:100%;
        height:800px;
        border:none;
        display:block;
        position:relative;
        z-index:99999;
      ">
  </iframe>
</v-container>
</template>

<script>
  import imgOdontopediatria from '@/assets/ImagenesP/ode.jpg';
  import imgEndodoncia from '@/assets/ImagenesP/en.jpg';
  import imgCirugias from '@/assets/ImagenesP/Fot4.jpg';
  import imgOrtodoncia from '@/assets/Imagenesp/Ort.jpg'; 
  import imgEstetica from '@/assets/ImagenesP/fot3.jpg'; 
  import imgPeriodoncia from '@/assets/periodoncia/period.jpg'; 
  
  export default {
  name: 'PaginaPrincipal',
  data() {
    return {

        isFlipped3: false,
        isFlipped4: false,
        isFlipped5: false,
        isFlipped6: false,
  
        especialidades: [
          { id: 1, nombre: "Odontopediatría", imagen: imgOdontopediatria, url: "/detalles/Odontopediatria" },
          { id: 2, nombre: "Endodoncia", imagen: imgEndodoncia, url: "/detalles/Endodoncia" },
          { id: 3, nombre: "Cirugías", imagen: imgCirugias, url: "/detalles/Cirugías" },
          { id: 4, nombre: "Ortodoncia", imagen: imgOrtodoncia, url: "/detalles/Ortodoncia y Ortopedia Maxilar" },
          { id: 5, nombre: "Estética Dental", imagen: imgEstetica, url: "/detalles/EsteticaDental" },
          { id: 6, nombre: "Periodoncia", imagen: imgPeriodoncia, url: "/detalles/Periodoncia" }
        ],
        valores: [
         { nombre: 'Ética', color: '#8A63F1', descripcion: 'Ser firme y honesto con los pacientes sobre su tratamiento que se le va a realizar.' },
         { nombre: 'Honestidad', color: '#8A63F1', descripcion: 'Tenemos el compromiso con nuestros pacientes de brindar información transparente.' },
         { nombre: 'Trabajo en equipo', color: '#8A63F1', descripcion: 'Colaboradores con comunicacion abierta, combinando diferentes perspectivas,habilidades,experiencias y conocimientos.' },
         { nombre: 'Tolerancia', color: '#8A63F1', descripcion: 'Capacidad de aceptar y respetar las diferencias de culto, religión e idioma de nuestros pacientes y en el equipo de trabajo.' },
         { nombre: 'Responsabilidad social', color: '#8A63F1', descripcion: 'Nos involucramos activamente en campañas, actividades y proyectos que beneficien a la comunidad y promuevan la salud bucal' },
  
      ],
      videos: [
  { url: 'https://www.youtube.com/embed/z-O0b0Xy99Y?start=16', treatment: 'RESINAS' },
  { url: 'https://www.youtube.com/embed/TLzreW_1fPA', treatment: 'CORONAS ESTETICAS' },
]

    };
  },
  props: {
    address: {
      type: String,
      default: 'Av. Reforma 153, Barrio de Jesús, 75615 San Lorenzo Ometepec, Pue.'
    }
  },
  methods: {

    flipCard3(event) {
      this.isFlipped3 = !this.isFlipped3;
      event.stopPropagation();
    },
    flipCard4(event) {
      this.isFlipped4 = !this.isFlipped4;
      event.stopPropagation();
    },
    flipCard5(event) {
      this.isFlipped5 = !this.isFlipped5;
      event.stopPropagation();
    },
    flipCard6(event) {
      this.isFlipped6 = !this.isFlipped6;
      event.stopPropagation();
    },
    irADetalle(especialidad) {
      console.log("Navegando a:", especialidad.url);
      switch (especialidad.nombre) {
        case "Odontopediatría": 
          this.$router.push({ name: "Odontopediatria" });
          break;
        case "Endodoncia": 
          this.$router.push({ name: "Endodoncia" });
          break;
        case "Cirugías":
          this.$router.push({ name: "Cirugías" });
          break;
        case "Ortodoncia": 
          this.$router.push({ name: "Ortodoncia" });
          break;
        case "Estética Dental": 
          this.$router.push({ name: "EsteticaDental" });
          break;
        case "Periodoncia": 
          this.$router.push({ name: "Periodoncia" });
          break;
      }
    },
    conoceMas() {
      this.$router.push({ name: 'Dentistas' });
    },
    vermasucursales() {
      this.$router.push({ name: 'Consultorios' });
    },
  }
};
</script>

<style>

/* Variables CSS para colores y espaciado */
:root {
  --primary-color: #55baa8;
  --secondary-color: #4a9b8e;
  --accent-color:#8A63F1;
  --text-dark: #2c3e50;
  --text-light: #7f8c8d;
  --background-light: #f8fffe;
  --white: #ffffff;
  --shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  --shadow-hover: 0 8px 15px rgba(0, 0, 0, 0.2);
  --border-radius: 12px;
  --transition: all 0.3s ease;
}

/* Reset y estilos base */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

body {
  font-family: "Poppins Rounded, Nunito ,Montserrat, Open Sans";
  line-height: 1.6;
  color: var(--text-dark);
  background-color: var(--background-light);
}

/* Sección Hero */
.hero {
  background: linear-gradient(135deg, var(--primary-color) 0%, var(--secondary-color) 100%);
  margin-top: 10rem;
  color: var(--white);
  padding: 80px 0;
  text-align: center;
  overflow: hidden;
  width: 100%;
}

.hero::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 100 100"><defs><pattern id="grain" width="100" height="100" patternUnits="userSpaceOnUse"><circle cx="25" cy="25" r="1" fill="rgba(255,255,255,0.1)"/><circle cx="75" cy="75" r="1" fill="rgba(255,255,255,0.1)"/></pattern></defs><rect width="100" height="100" fill="url(%23grain)"/></svg>');
  opacity: 0.3;
}

.hero .content {
  position: relative;
  z-index: 2;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.hero h1 {
  font-size: 3.5rem;
  font-weight: 700;
  margin-bottom: 10px;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
}

.hero h2 {
  font-size: 2rem;
  font-weight: 300;
  margin-bottom: 30px;
  opacity: 0.9;
}

.hero p {
  font-size: 1.2rem;
  max-width: 800px;
  margin: 0 auto 40px;
  line-height: 1.8;
  opacity: 0.95;
}

.hero img {
  max-width: 100%;
  height: auto;
  border-radius: var(--border-radius);
  box-shadow: var(--shadow-hover);
  margin-top: 20px;
}

/* Carrusel de Especialidades */
.especialidades-container {
  padding: 80px 0;
  background: #8A63F1;
}

.carrusel {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 30px;
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.imagen-contenedor {
  position: relative;
  border-radius: var(--border-radius);
  overflow: hidden;
  cursor: pointer;
  transition: var(--transition);
  box-shadow: var(--shadow);
}

.imagen-contenedor:hover {
  transform: translateY(-10px);
  box-shadow: var(--shadow-hover);
}

.imagen-contenedor .imagen {
  width: 100%;
  height: 250px;
  object-fit: cover;
  transition: var(--transition);
}

.imagen-contenedor:hover .imagen {
  transform: scale(1.1);
}

.nombre-overlay {
  position: absolute;
  bottom: 0;
  left: 0;
  right: 0;
  background: linear-gradient(transparent, rgba(0, 0, 0, 0.8));
  color: var(--white);
  padding: 30px 20px 20px;
  font-size: 1.3rem;
  font-weight: 600;
  text-align: center;
}

/* Galería de Doctores */
.doctors-gallery {
  padding: 80px 0;
  background: var(--background-light);
}

.doctors-gallery h2 {
  text-align: center;
  font-size: 2.5rem;
  color: var(--text-dark);
  margin-bottom: 60px;
  position: relative;
}

.doctors-gallery h2::after {
  content: "";
  position: absolute;
  bottom: -10px;
  left: 50%;
  transform: translateX(-50%);
  width: 80px;
  height: 4px;
  background: #8A63F1;
  border-radius: 2px;
}

/* Tarjetas de Doctores */
.card {
  perspective: 1000px;
  height: 800px;
  margin-bottom: 30px;
}

.card-inner {
  position: relative;
  width: 100%;
  height: 100%;
  text-align: center;
  transition: transform 0.8s;
  transform-style: preserve-3d;
}

.card-inner.flipped {
  transform: rotateY(180deg);
}

.card-front,
.card-back {
  position: absolute;
  width: 100%;
  height: 100%;
  backface-visibility: hidden;
  border-radius: var(--border-radius);
  box-shadow: var(--shadow);
  background: var(--white);
  overflow: hidden;
}

.card-back {
  transform: rotateY(180deg);
}

.card-img,
.card-img2,
.card-img3,
.card-img4,
.card-img5,
.card-img6 {
  height: 20rem;
}

.card-content,
.card-back-content {
  padding: 20px;
  height: calc(100% - 200px);
  display: flex;
  flex-direction: column;
  justify-content: space-between;
}

.card-content h3,
.card-back-content h3 {
  font-size: 1.4rem;
  color:  #8A63F1;
  margin-bottom: 10px;
  font-weight: 600;
}

.card-content h4 {
  font-size: 1rem;
  color: var(--primary-color);
  margin-bottom: 15px;
  font-weight: 500;
}

.custom-line,
.custom-line2,
.custom-line3,
.custom-line4,
.custom-line5,
.custom-line6 {
  border: none;
  height: 2px;
  background: var(--primary-color);
  margin: 15px 0;
  border-radius: 1px;
}

.text-with-images,
.text-with-images2,
.text-with-images3,
.text-with-images4,
.text-with-images5,
.text-with-images6 {
  display: flex;
  align-items: flex-start;
  margin-bottom: 15px;
  gap: 15px;
}

.small-img {
  width: 40px;
  height: 40px;
  border-radius: 50%;
  object-fit: cover;
  flex-shrink: 0;
}

.text-content,
.text-content2,
.text-content3,
.text-content4,
.text-content5,
.text-content6 {
  flex: 1;
}

.justified-text {
  text-align: justify;
  font-size: 0.9rem;
  line-height: 1.5;
  color: var(--text-light);
}

/* Botones */
.btn-primary1v,
.btn-primary2v,
.btn-primary3v,
.btn-primary4v,
.btn-primary5v,
.btn-primary6v,
.btn-primary1,
.btn-primary2,
.btn-primary3,
.btn-primary4,
.btn-primary5,
.btn-primary6 {
  background: var(--primary-color);
  color: var(--white);
  border: none;
  padding: 12px 24px;
  border-radius: 25px;
  cursor: pointer;
  font-weight: 600;
  transition: var(--transition);
  font-size: 0.9rem;
}

.btn-primary1v:hover,
.btn-primary2v:hover,
.btn-primary3v:hover,
.btn-primary4v:hover,
.btn-primary5v:hover,
.btn-primary6v:hover,
.btn-primary1:hover,
.btn-primary2:hover,
.btn-primary3:hover,
.btn-primary4:hover,
.btn-primary5:hover,
.btn-primary6:hover {
  background: var(--secondary-color);
  transform: translateY(-2px);
  box-shadow: var(--shadow);
}

.button-container,
.button-container1 {
  text-align: center;
  margin-top: 40px;
}

.boton-conoce-mas,
.boton-ver-mas-sucursales {
  background: var(--primary-color);
  color: var(--white);
  border: none;
  padding: 15px 30px;
  border-radius: 30px;
  cursor: pointer;
  font-weight: 600;
  font-size: 1.1rem;
  transition: var(--transition);
  text-transform: uppercase;
  letter-spacing: 1px;
}

.boton-conoce-mas:hover,
.boton-ver-mas-sucursales:hover {
  background:  #8A63F1;
  transform: translateY(-3px);
  box-shadow: var(--shadow-hover);
}

/* Sección Filosofía */
.filosofia-container {
  padding: 80px 20px;
  max-width: 1200px;
  margin: 0 auto;
  text-align: center;
}

.filosofia-container h2 {
  font-size: 2.5rem;
  color: var(--text-dark);
  margin-bottom: 20px;
}

.filosofia-container p {
  font-size: 1.2rem;
  color: var(--text-light);
  margin-bottom: 10px;
}

.texto2 {
  font-size: 1.2rem;
  color: var(--text-light);
  margin-bottom: 60px;
}

.misvis-section {
  display: grid;
  gap: 60px;
  margin-bottom: 60px;
}

.misvis-item {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 40px;
  align-items: center;
}

.misvis-item:nth-child(even) {
  direction: rtl;
}

.misvis-item:nth-child(even) > * {
  direction: ltr;
}

.misvis-item img {
  width: 100%;
  height: 300px;
  object-fit: cover;
  border-radius: var(--border-radius);
  box-shadow: var(--shadow);
}

.misvis-text,
.misvis-text1 {
  padding: 30px;
  background: var(--white);
  border-radius: var(--border-radius);
  box-shadow: var(--shadow);
}

.misvis-text h3,
.misvis-text1 h3 {
  font-size: 1.8rem;
  color: #8A63F1;
  margin-bottom: 20px;
  font-weight: 700;
}

.misvis-text p,
.misvis-text1 p {
  font-size: 1.1rem;
  line-height: 1.8;
  color: var(--text-dark);
  text-align: justify;
}

.content1 {
  text-align: center;
}

.content1 img {
  max-width: 100%;
  height: auto;
  border-radius: var(--border-radius);
  box-shadow: var(--shadow);
}

/* Sección Valores */
.valores-container {
  padding: 80px 20px;
  max-width: 1000px;
  margin: 0 auto;
}

.valores-container h2 {
  font-size: 2.5rem;
  color: var(--text-dark);
  text-align: center;
  margin-bottom: 50px;
}

.valores-list {
  list-style: none;
  display: grid;
  gap: 25px;
}

.valores-list li {
  background: var(--white);
  padding: 25px;
  border-radius: var(--border-radius);
  box-shadow: var(--shadow);
  border-left: 5px solid var(--primary-color);
  transition: var(--transition);
}

.valores-list li:hover {
  transform: translateX(10px);
  box-shadow: var(--shadow-hover);
}

.valores-list li strong {
  font-size: 1.2rem;
  display: block;
  margin-bottom: 10px;
}

.logo-container {
  text-align: center;
  padding: 40px 0;
}

.logo-felizdent {
  max-width: 300px;
  height: auto;
  border-radius: var(--border-radius);
  box-shadow: var(--shadow);
}

/* Sección Testimoniales */
.testimonials-section {
  padding: 80px 0;
  background: var(--background-light);
}

.Blue-container {
  text-align: center;
  margin-bottom: 60px;
}

.Blue-container h2 {
  font-size: 2.5rem;
  color: var(--text-dark);
  position: relative;
}

.Blue-container h2::after {
  content: "";
  position: absolute;
  bottom: -10px;
  left: 50%;
  transform: translateX(-50%);
  width: 80px;
  height: 4px;
  background: #8A63F1;
  border-radius: 2px;
}

.green-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 20px;
}

.row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
  margin-bottom: 30px;
  align-items: center;
}

.video-box {
  background: var(--white);
  border-radius: var(--border-radius);
  overflow: hidden;
  box-shadow: var(--shadow);
  aspect-ratio: 16 / 9;
}

.video-box iframe {
  width: 100%;
  height: 100%;
  border: none;
}

.blue-box {
  background: var(--primary-color);
  color: var(--white);
  padding: 40px;
  border-radius: var(--border-radius);
  text-align: center;
  box-shadow: var(--shadow);
}

.blue-box p {
  font-size: 1.3rem;
  font-weight: 600;
  margin: 0;
}

/* Sección Comentarios */
.comentarios-section {
  padding: 80px 0;
  background: var(--white);
}

/* Sección Ubicación */
.direccion-boton-contenedor {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 15px;
  margin-bottom: 40px;
  padding: 20px;
  background: var(--white);
  border-radius: #8A63F1;
  box-shadow: var(--shadow);
  flex-wrap: wrap;
}

.icono-direccion,
.icono-boton {
  width: 30px;
  height: 30px;
  object-fit: contain;
}

.direccion {
  font-size: 1.1rem;
  color: var(--text-dark);
  margin: 0;
  text-align: center;
  flex: 1;
  min-width: 200px;
}

.image-and-map {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 30px;
  margin-top: 40px;
}

.image-container,
.map-container {
  border-radius: var(--border-radius);
  overflow: hidden;
  box-shadow: var(--shadow);
}

.clinica-img {
  width: 100%;
  height: 400px;
  object-fit: cover;
}

.map-frame {
  width: 100%;
  height: 400px;
  border: none;
}

/* Responsive Design */
@media (max-width: 768px) {
  .hero h1 {
    font-size: 2.5rem;
  }

  .hero h2 {
    font-size: 1.5rem;
  }

  .hero p {
    font-size: 1rem;
  }

  .carrusel {
    grid-template-columns: 1fr;
    gap: 20px;
  }

  .card {
    height: auto;
    min-height: 500px;
  }

  .misvis-item {
    grid-template-columns: 1fr;
    gap: 20px;
  }

  .misvis-item:nth-child(even) {
    direction: ltr;
  }

  .row {
    grid-template-columns: 1fr;
    gap: 20px;
  }

  .image-and-map {
    grid-template-columns: 1fr;
    gap: 20px;
  }

  .direccion-boton-contenedor {
    flex-direction: column;
    text-align: center;
  }

  .direccion {
    min-width: auto;
  }
}

@media (max-width: 480px) {
  .hero {
    padding: 40px 0;
  }

  .hero h1 {
    font-size: 2rem;
  }

  .hero h2 {
    font-size: 1.2rem;
  }

  .doctors-gallery h2,
  .filosofia-container h2,
  .valores-container h2,
  .Blue-container h2 {
    font-size: 2rem;
  }

  .card-content,
  .card-back-content {
    padding: 15px;
  }

  .misvis-text,
  .misvis-text1 {
    padding: 20px;
  }

  .valores-list li {
    padding: 20px;
  }
}

/* Animaciones */
@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(30px);
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

.card,
.valores-list li,
.misvis-item {
  animation: fadeInUp 0.6s ease-out;
}

/* Efectos de hover adicionales */
.imagen-contenedor::before {
  content: "";
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  bottom: 0;
  background: linear-gradient(45deg, var(--primary-color), #8A63F1);
  opacity: 0;
  transition: var(--transition);
  z-index: 1;
}

.imagen-contenedor:hover::before {
  opacity: 0.2;
}

.nombre-overlay {
  z-index: 2;
}

</style>