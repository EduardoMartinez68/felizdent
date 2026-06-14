<template>
  <div class="container">
    <h1>Dentistas</h1>
  </div>
    
  <v-container>
    <v-row>


      <!-- Tarjeta 3 -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped3 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/Imagenes/docisa.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dra. Isabel Chávez</h3>
                <h4>Estomatología Pediátrica</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. En Estomatología por la "Benemérita Universidad Autónoma de Puebla" 2002 a 2006.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist11.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Especialidad en Estomatología Pediátrica "Hospital para el Niño Poblano" 2009 a 2011.
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard3">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Diplomados</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist3.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado en Investigación Clínica "Benemérita Universidad Autónoma de Puebla" 2009- 2010 (240 hrs).
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado de Ortopedia Maxilar con Aplicación Clínica En la "Benemérita Universidad Autónoma de Puebla" (campus Tehuacán) 2019- 2021.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist3.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado de Actualización Ortopedia y Odontopediatría "Desarrollo Especializado con Nuevas Técnicas de Actualización" 2021-2022.
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard3">Volver</button>
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
              <img src="@/assets/Imagenes/dentistY.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dra. Yazmin Téllez Bautista</h3>
                <h4>Estomatología y Especialista en Endodoncia</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. En Estomatología por la "Benemérita Universidad Autónoma de Puebla" 1998-2003.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist12.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Especialidad en endodoncia por "Centro Mexicano en estomatología" 2009 a 2011.
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard4">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Diplomados</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado de medicina interna en Estomatología en "Benemérita Universidad Autónoma de puebla" 2012-2013.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist3.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado en Diagnóstico y Tratamientos básicos Periodontales en "Benemérita Universidad Autónoma de Puebla" abril 2015-febrero 2016.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist13.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado en Odontología Estetica y Restauradora en "Colegio Dental del Estado de Mexico, A.C" 2022.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist15.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado en Cirugía Plástica Periodental en "Colegio de Actualización Profesional Tepeaca" 2024.
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard4">Volver</button>
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
              <img src="@/assets/Imagenes/dentistBr.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dra. Bricia Pascuala López López</h3>
                <h4>Estomatología</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. en Estomatología por la "Benemérita Universidad Autónoma de Puebla" 2008 a 2013.
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard5">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Diplomados</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado de medicina interna en Estomatología avalada por "Benemérita Universidad Autónoma de Puebla" 2019-2020.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist15.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado de Biocosmética Dental por el "Colegio de Actualización de Tepeaca" octubre 2021-septiembre a 2022.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist15.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Diplomado en Prostodoncia Total por "Colegio de Actualización de Tepeaca" noviembre 2022 a junio 2022.
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard5">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>

      <!-- Tarjeta 8 -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped8 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/Imagenes/dentistEli.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dr. Elio Federico Monterrosas Fuentes</h3>
                <h4>Estomatología y Especialista en Ortopedia</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. En Estomatología por la "Benemérita Universidad Autónoma de Puebla" 1998 a 2003.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist21.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Especialidad en Ortopedia por la "Universidad Nacional Autónoma de México (UNAM)" 2009 a 2011.
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard8">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Nivel académico</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. En Estomatología por la "Benemérita Universidad Autónoma de Puebla" 1998 a 2003.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist21.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Especialidad en Ortopedia por la "Universidad Nacional Autónoma de México (UNAM)" 2009 a 2011.
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard8">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>

      <!-- Tarjeta 9 -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped9 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/Imagenes/docang.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dr. José Ángel Pérez Benítez</h3>
                <h4>Estomatología y Especialista en Ortodoncia y Endodoncia</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist19.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. En Estomatología por la "Universidad México Americana del Golfo, Puebla" 2011 a 2015.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist12.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Especialidad en endodoncia por "Centro Mexicano en estomatología" 2016 a 2018.
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard9">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Nivel académico</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist19.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. En Estomatología por la "Universidad México Americana del Golfo, Puebla" 2011 a 2015.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist12.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Especialidad en endodoncia por "Centro Mexicano en estomatología" 2016 a 2018.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist22.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Especialidad en Ortodoncia por "Centro Universitario Interamericano del Pacífico (CEUNI), Plantel Golfo Centro, Heroica Puebla de Zaragoza, PUE" 2019 a 2021.
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard9">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>

      <!-- Tarjeta 10 -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped10 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/imagenesespecialistas/dramgsanchezperez.jpeg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dra. María Guadalupe Sánchez Pérez</h3>
                <h4>Estomatología</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist8.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Universidad del Valle de Puebla 
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard10">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Experiencia</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist23.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Servicio Social en "Clínica Particular Dental Dorada" Auxiliar dental en diversas áreas odontológicas, incluyendo limpieza y desinfección de instrumental y equipamiento utilizado, de 2022 a 2023.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist23.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Trabajo en" Dental Dorada" como auxiliar en: Endodoncia, Ortodoncia, Rehabilitación, Cirugía bucal Y conocimientos en área de recepción, 2023 a 2024.
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard10">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>

      <!-- Tarjeta 12 -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped12 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/Imagenes/dentistMG.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dra. María Guadalupe Pérez Ponce</h3>
                <h4>Odontóloga General</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist8.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. En Odontología "Centro de Estudios Superiores de Tepeaca" 2018 a 2023.
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard12">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Experiencia</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist26.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      OPPSS realizado en "Centro de Estudios Superiores de Tepeaca."
                    </p>
                  </div>
                </div>
                <div class="text-content">
                  <p class="justified-text">
                    • "Uso de aparatología rayos x".
                  </p>
                </div>
                <div class="text-content">
                  <p class="justified-text">
                    • "Profilaxis, educación de higiene oral."
                  </p>
                </div>
                <div class="text-content">
                  <p class="justified-text">
                    • "Restauración de estéticas".
                  </p>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard12">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>

      <!-- Tarjeta 13 - Aylin -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped13 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/Imagenes/docayl.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dra. Aylin Zayagos Fernández</h3>
                <h4>Lic. en Estomatología</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      "BENEMÉRITA UNIVERSIDAD AUTÓNOMA DE PUEBLA" Facultad de Estomatología 2018 2024.
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard13">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Experiencia</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Servicio social culminado en el periodo ene 2024- feb 2025 realizado en el área de práctica profesional (jornadas en diferentes comunidades).
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard13">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>

      <!-- Tarjeta 14 - Salma -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped14 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/Imagenes/docsalm.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dra. Salma Yenifer Rodriguez Camarillo</h3>
                <h4>Lic. en Estomatología</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. en Estomatología por la "Benemérita Universidad Autónoma de Puebla" 2018 a 2023.
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard14">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Experiencia</h3>
                <div class="text-with-images">
                  <div class="text-content">
                    <p class="justified-text">
                      S.S Clinica de Estomatologia del CRS Experiencia en cirugias periodontales: Alargamiento de corona 2023 2024
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard14">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>

      <!-- Tarjeta 15 - Sandra -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped15 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/Imagenes/docsandra.jpg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dra. Sandra Velázquez</h3>
                <h4>Lic. en Estomatología con especialidad en estomatologia pediatrica</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. en Estomatología.
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <img src="@/assets/ImagenesP/logohnp.jpeg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Especialidad en Estomatología Pediátrica, Hospital para el Niño Poblano 2023/2025
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard15">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Experiencia</h3>
                <div class="text-with-images">
                  <div class="text-content">
                    <p class="justified-text">
                      Consultorio | Asistente dental Febrero 2019 3 meses +Asistir en consulta Toma de radiografías periapicales lavado y esterilizado de instrumental
                    </p>
                  </div>
                </div>
                <div class="text-with-images">
                  <div class="text-content">
                    <p class="justified-text">
                      Consultorio | Asistente dental Mayo 2019 - 1 mes Asistir en consulta Lavado y esterilizado de instrumental Toma de impresiones y vaciado de modelos
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard15">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>

      <!-- Tarjeta 16 - Daniel -->
      <v-col cols="12" md="4">
        <div class="card">
          <div class="card-inner" :class="{ flipped: isFlipped16 }">
            <!-- Cara delantera -->
            <div class="card-front">
              <img src="@/assets/Imagenesespecialistas/drdaniel.jpeg" alt="Imagen del Dentista" class="card-img">
              <div class="card-content">
                <h3>Dr. Daniel Jiménez de Rosas</h3>
                <h4>Dentista General</h4>
                <hr class="custom-line">
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Lic. Benemérita universidad autónoma de Puebla 2007-2012.
                    </p>
                    <p class="justified-text">
                      Servicio social San Salvador El Seco 2013-2014
                    </p>
                  </div>
                </div>
                <div class="button">
                  <button class="btn-primary-v" @click.stop="flipCard16">Ver más</button>
                </div>
              </div>
            </div>

            <!-- Cara trasera -->
            <div class="card-back">
              <div class="card-back-content">
                <h3>Experiencia</h3>
                <div class="text-with-images">
                  <img src="@/assets/Imagenes/dentist2.jpg" alt="Logo" class="small-img">
                  <div class="text-content">
                    <p class="justified-text">
                      Clínica dental con experiencia en tratamientos generales y consulta integral.
                    </p>
                  </div>
                </div>
                <div class="button-container">
                  <button class="btn-primary" @click.stop="flipCard16">Volver</button>
                </div>
              </div>
            </div>
          </div>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  name: 'DentistCard',
  data() {
    return {

      isFlipped2: false,
      isFlipped3: false,
      isFlipped4: false,
      isFlipped5: false,
      isFlipped6: false,
      isFlipped7: false,
      isFlipped8: false,
      isFlipped9: false,
      isFlipped10: false,
      isFlipped11: false,
      isFlipped12: false,
      isFlipped13: false,
      isFlipped14: false,
      isFlipped15: false,
      isFlipped16: false,
    };
  },
  methods: {

    flipCard2(event) {
      this.isFlipped2 = !this.isFlipped2;
      event.stopPropagation();
    },
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
    flipCard7(event) {
      this.isFlipped7 = !this.isFlipped7;
      event.stopPropagation();
    },
    flipCard8(event) {
      this.isFlipped8 = !this.isFlipped8;
      event.stopPropagation();
    },
    flipCard9(event) {
      this.isFlipped9 = !this.isFlipped9;
      event.stopPropagation();
    },
    flipCard10(event) {
      this.isFlipped10 = !this.isFlipped10;
      event.stopPropagation();
    },
    flipCard11(event) {
      this.isFlipped11 = !this.isFlipped11;
      event.stopPropagation();
    },
    flipCard12(event) {
      this.isFlipped12 = !this.isFlipped12;
      event.stopPropagation();
    },
    flipCard13(event) {
      this.isFlipped13 = !this.isFlipped13;
      event.stopPropagation();
    },
    flipCard14(event) {
      this.isFlipped14 = !this.isFlipped14;
      event.stopPropagation();
    },
    flipCard15(event) {
      this.isFlipped15 = !this.isFlipped15;
      event.stopPropagation();
    },
    flipCard16(event) {
      this.isFlipped16 = !this.isFlipped16;
      event.stopPropagation();
    },
  }
}
</script>

<style scoped>
/* Estilo del contenedor principal */
.container {
  padding: 20px;
  text-align: center;
}

/* Estilo para el título */
.container h1 {
  font-weight: bold;
  font-size: 36px;
  margin-top: 100px;
  margin-bottom: 40px;
  text-align: center;
}

.card {
  width: 100%;
  max-width: 100%;
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 0 4px 12px rgba(0, 0, 0, 0.08);
  overflow: hidden;
  margin: 8px 0;
  background-color: #fff;
  height: 950px;
  perspective: 1000px;
  text-rendering: optimizeLegibility;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  font-size: 1rem;
  display: flex;
  flex-direction: column;
}

@media (max-width: 768px) {
  .card {
    max-width: 280px;
    height: auto;
  }
}

@media (max-width: 480px) {
  .card {
    max-width: 100%;
    height: auto;
  }
}

.card-inner {
  width: 100%;
  height: 100%;
  position: relative;
  transition: transform 0.6s;
  transform-style: preserve-3d;
}

.card-inner.flipped {
  transform: rotateY(180deg);
}

.card-front, 
.card-back {
  width: 100%;
  height: 100%;
  position: absolute;
  backface-visibility: hidden;
}

.card-front {
  background-color: #fff;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: flex-start;
}

.card-back {
  background-color: #f0f0f0;
  transform: rotateY(180deg);
  padding: 16px;
  display: flex;
  flex-direction: column;
  justify-content: flex-start;
  text-align: left;
}

/* Imágenes de las tarjetas */
.card-img {
  width: 100%;
  height: 500px;
  object-fit: cover;
}

@media (max-width: 768px) {
  .card-img {
    height: 350px;
  }
}

@media (max-width: 480px) {
  .card-img {
    height: 250px;
  }
}

.small-img {
  width: 40px;
  height: auto;
  margin-right: 8px;
  flex-shrink: 0;
}

/* Contenedores de texto con imágenes */
.text-with-images {
  display: flex;
  align-items: flex-start;
  margin: 12px 0;
  gap: 8px;
}

/* Contenido de texto */
.text-content {
  flex: 1;
  word-wrap: break-word;
  overflow-wrap: break-word;
}

.text-content p {
  margin: 0;
  padding: 0;
  line-height: 1.4;
}

.card-content {
  padding: 16px;
  display: flex;
  flex-direction: column;
}

.card-back-content {
  font-size: 1.15em;
  padding: 0;
}

.card-back-content h3 {
  font-size: 1.16em;
  margin: 0 0 16px 0;
  padding: 0;
  text-align: left;
}

.card-content h3 {
  margin: 0 0 8px 0;
  padding: 0;
  font-size: 1.15em;
  text-align: center;
}

.card-content h4 {
  font-size: 0.95em;
  color: #666;
  margin: 0 0 12px 0;
  padding: 0;
  font-weight: normal;
  text-align: center;
}

.custom-line {
  border: none;
  height: 1px;
  background-color: #ddd;
  margin: 12px 0;
  padding: 0;
}

.justified-text {
  margin: 0;
  padding: 0;
  color: #333;
  text-align: justify;
  line-height: 1.4;
}

.button {
  display: flex;
  justify-content: center;
  padding: 8px 16px 16px 16px;
  width: 100%;
  box-sizing: border-box;
}

/* Botones "Ver más" */
.btn-primary-v {
  padding: 10px 24px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 0.9em;
  background-color: #4a9b8e;
  color: #fff;
  transition: background-color 0.3s ease;
  white-space: nowrap;
}

.btn-primary-v:hover {
  background-color: #3a8b7e;
}

/* Botones "Volver" */
.btn-primary {
  padding: 10px 24px;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  font-size: 0.9em;
  background-color: #8A63F1;
  color: #fff;
  transition: background-color 0.3s ease;
  white-space: nowrap;
}

.btn-primary:hover {
  background-color: #7a53e1;
}

.button-container {
  width: 100%;
  display: flex;
  justify-content: center;
  padding: 16px;
  box-sizing: border-box;
  margin-top: auto;
}
</style>