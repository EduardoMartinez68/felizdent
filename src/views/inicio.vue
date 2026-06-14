<template>
  <!-- Sección Filosofía -->
  <v-container>
    <v-row>
      <section class="hero inicio-container">
        <div class="content">
        <h1>FelizDent</h1>
        <h2>Por el gusto de verte sonreír</h2>
        <p>Felizdent es una clínica dental en con más de 20 años de experiencia, ofreciendo soluciones dentales innovadoras con tratamientos innovadores y mínimamente invasivos.
        Utilizamos materiales de última generación y contamos con un equipo de odontólogos especializados en periodoncia, estética dental, ortodoncia
        y odontopediatría, comprometidos con brindarte el mejor cuidado para tu salud bucal.</p>
        <img src="@/assets/ImagenesC/especialistasabril2026.jpeg" alt="Consultorio dental">
      </div>
        
       
        <h1 class="titulo-filosofia">Conoce nuestra filosofía</h1>
        <p>
          Descubre qué nos motiva y guía en Felizdent. Nuestra misión, visión y valores reflejan
          nuestro compromiso con tu salud dental y bienestar.
        </p>

        <!-- Sección Misión y Visión -->
        <div class="misvis-container">
          <!-- VISIÓN -->
          <div class="misvis-card">
            <img src="@/assets/ImagenesP/mision.jpg" alt="Paciente sonriendo" class="misvis-img" />
            <div class="misvis-text">
              <h3>VISIÓN</h3>
              <p>
               Para el 2030 ser una clínica dental líder en la región, reconocida por brindar servicios dentales integrales, personalizados de excelencia y con el compromiso social de la comunidad.
              </p>
            </div>
          </div>

          <!-- MISIÓN -->
          <div class="misvis-card reverse">
            <img src="@/assets/ImagenesP/vision.jpg" alt="Dentista trabajando" class="misvis-img" />
            <div class="misvis-text">
              <h3>MISIÓN</h3>
              <p>
              Transformar vidas a través de sonrisas saludables y esteticas; mejorando su autoestima, concientizando la importacia de la salud bucal, apoyados de un equipo de especialistas altamente calificados, aplicando innovación tecnológica, trato humano, para ofrecer soluciones integrales, personalizadas y con la confianza de estar en las mejores manos.
              </p>
            </div>
          </div>
        </div>

        <!-- Imagen final -->
        <div class="final-img-container">
          <img src="@/assets/ImagenesP/dentI.jpg" alt="Consultorio dental">
        </div>
      </section>
    </v-row>
  </v-container>

  <!-- Sección de Valores -->
  <v-container>
    <v-row>
      <div class="valores-container">
        <h2>Valores</h2>
        <ul class="valores-list">
          <li v-for="valor in valores" :key="valor.nombre">
            <strong :style="{ color: valor.color }">{{ valor.nombre }}:</strong>
            {{ valor.descripcion }}
          </li>
        </ul>
      </div>
    </v-row>
  </v-container>
</template>

<script setup>
const valores = [
  { nombre: 'Ética', color: '#8A63F1', descripcion: 'Ser firme y honesto con los pacientes sobre su tratamiento que se le va a realizar.' },
  { nombre: 'Honestidad', color: '#8A63F1', descripcion: 'Tenemos el compromiso con nuestros pacientes de brindar información transparente.' },
  { nombre: 'Trabajo en equipo', color: '#8A63F1', descripcion: 'Colaboradores con comunicacion abierta, combinando diferentes perspectivas,habilidades,experiencias y conocimientos.' },
  { nombre: 'Tolerancia', color: '#8A63F1', descripcion: 'Capacidad de aceptar y respetar las diferencias de culto, religión e idioma de nuestros pacientes y en el equipo de trabajo.' },
  { nombre: 'Responsabilidad social', color: '#8A63F1', descripcion: 'Nos involucramos activamente en campañas, actividades y proyectos que beneficien a la comunidad y promuevan la salud bucal' },
  
 
];
</script>

<style scoped>
/* Importa fuentes Montserrat y Open Sans */
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@600;700&family=Open+Sans:wght@400;600&display=swap');

.hero {
  text-align: center;
  padding: 3rem 1rem;
}
h1 {
  font-family: 'Poppins Rounded', sans-serif; /* fuente para títulos */
}

p {
  font-family: 'Montserrat', sans-serif; /* fuente para párrafos */
}


/* Títulos principales */
.titulo-principal {
  font-family: 'Poppins Rounded', sans-serif;
  font-size: 3rem;
  color:8 ;
  margin-bottom: 0.5rem;
}

.subtitulo {
  font-family: 'Montserrat', sans-serif;
  font-size: 1.5rem;
  color: white;
}

.titulo-filosofia {
  font-family: 'Montserrat', sans-serif;
  font-size: 2.5rem;
  margin-top: 2rem;
  color:white ;
}

.descripcion-filosofia {
  font-family: 'Montserrat', sans-serif;
  font-size: 1.2rem;
  color:white ;
  margin: 1rem auto 3rem;
  max-width: 800px;
}

/* Sección Misión y Visión */
.misvis-container {
  display: flex;
  flex-direction: column;
  gap: 3rem;
  align-items: center;
}

.misvis-card {
  display: flex;
  align-items: center;
  justify-content: space-between;
  gap: 2rem;
  flex-wrap: wrap;
  max-width: 1100px;
  width: 100%;
}

.misvis-card.reverse {
  flex-direction: row-reverse;
}

.misvis-img {
  width: 45%;
  border-radius: 20px;
  object-fit: cover;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
}

.misvis-text {
  width: 45%;
  text-align: left;
  font-family: 'Montserrat', sans-serif;
}

.misvis-text h3 {
  font-family: 'Montserrat', sans-serif;
  color: #8A63F1;
  font-size: 1.8rem;
  margin-bottom: 1rem;
}

.misvis-text p {
  font-size: 1.1rem;
  line-height: 1.6;
  color: #555;
}

/* Imagen final */
.final-img-container {
  margin-top: 3rem;
  display: flex;
  justify-content: center;
}

.final-img {
  border-radius: 25px;
  max-width: 700px;
  height: 400px;
  box-shadow: 0 5px 20px rgba(0, 0, 0, 0.25);
}

/* Valores */
.valores-container {
  text-align: center;
  margin-top: 3rem;
}

.valores-list {
  list-style: none;
  padding: 0;
  margin-top: 1rem;
  font-size: 1.1rem;
  font-family: 'montserrat', sans-serif;
}

.valores-list li {
  margin: 0.6rem 0;
}
</style>
