<template>
  <section class="testimonios-section">
    <h2 class="titulo">Conoce nuestros testimonios de  pacientes</h2>

    <div class="fila" v-for="(item, idx) in items" :key="item.id">
      <div
        class="bloque video-bloque"
        :class="{ orden2: isOdd(idx) }"
      >
        <div class="video-wrap">
          <iframe
            :src="item.embedUrl"
            title="Testimonio"
            frameborder="0"
            allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
            allowfullscreen
          ></iframe>
        </div>
      </div>

      <div
        class="bloque tarjeta-bloque"
        :class="{ orden2: !isOdd(idx) }"
      >
        <div class="tarjeta">
          <div class="tarjeta-titulo">{{ item.title }}</div>
        </div>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "TestimoniosVideos",
  data() {
    return {
      items: [
        {
          id: 1,
          title: "Testimonio de resinas",
          embedUrl: "https://www.youtube.com/embed/z-O0b0Xy99Y?start=29",
        },
        {
          id: 2,
          title: "Testimonio de coronas Estéticas",
          embedUrl: "https://www.youtube.com/embed/TLzreW_1fPA",
        },
        {
          id: 3,
          title: "Testimonio Ortodoncia",
          embedUrl: "https://www.youtube.com/embed/L5wEmiVXXUU",
        },
        {
          id: 4,
          title: " Testimonio coronas Dentales",
          embedUrl: "https://www.youtube.com/embed/E4YlZXQGIRU",
        },
         {
          id: 5,
          title: "Testimonio puente fijo 3 unidades",
          embedUrl: "https://www.youtube.com/embed/i8vcT5DTn6M",
        },
      ],
    };
  },
  methods: {
    isOdd(i) {
      return i % 2 === 0;
    },
  },
};
</script>

<style scoped>
.testimonios-section {
  padding: 50px 20px;
  background: #f6fdfb;
}

.titulo {
  
  font-size: 36px !important;
  text-align: center;
  margin: 90px 0 30px !important;
  color: #123 !important;
  z-index: 10;
  position: relative;


}

.fila {
  display: flex;
  align-items: center;
  gap: 30px;
  margin: 30px 0;
  flex-wrap: wrap;
}

.bloque {
  width: 48%;
  min-height: 220px;
  box-sizing: border-box;
}

.orden2 {
  order: 2;
}

.video-wrap {
  width: 100%;
  padding-bottom: 56.25%;
  position: relative;
  border-radius: 12px;
  overflow: hidden;
  background: #000;
}

.video-wrap iframe {
  position: absolute;
  inset: 0;
  width: 100%;
  height: 100%;
  border: 0;
}

/* Colores base */
.tarjeta {
  border-radius: 12px;
  height: 100%;
  min-height: 220px;
  display: flex;
  align-items: center;
  justify-content: center;
  padding: 20px;
  box-shadow: 0 6px 18px rgba(0,0,0,0.06);
  color: white;
  font-weight: bold;
}

/* 1er tarjeta */
.fila:nth-child(1) .tarjeta {
  background: #57c6b7; 
}

/* 2da tarjeta */
.fila:nth-child(2) .tarjeta {
  background: #57c6b7; 
}

/* 3ra tarjeta */
.fila:nth-child(3) .tarjeta {
  background: #8A63F1; 
}

/* 4ta tarjeta */
.fila:nth-child(4) .tarjeta {
  background:#57c6b7; 
}
.fila:nth-child(5) .tarjeta {
  background: #8A63F1; 
}
.fila:nth-child(6) .tarjeta {
  background: #57c6b7; 
}

.tarjeta-titulo {
  color: #fff;
  font-weight: 700;
  font-size: 24px;
  text-transform: uppercase;
  text-align: center;
  letter-spacing: 0.8px;
}

@media (max-width: 900px) {
  .bloque {
    width: 100%;
  }
  .orden2 {
    order: initial;
  }
  .fila {
    gap: 18px;
  }
  .titulo { margin-top: 20px; font-size: 28px; }
}
</style>
