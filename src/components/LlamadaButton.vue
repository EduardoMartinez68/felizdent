<template>
  <!-- Botón de llamada -->
  <a class="call-button" href="tel:2221526613" aria-label="Llamar al consultorio">
    <img src="@/assets/Imagenes/imagenLlamada.jpg" alt="Llamar" class="call-icon">
    
  </a>
</template>

<script>
export default {
  name: 'CallButton'
}
</script>

<style scoped>
/* Estilos para el botón de llamada */
.call-button {
  position: fixed;
  bottom: 140px; /* Más arriba que el botón de WhatsApp para que no se superpongan */
  right: 20px;
  width: 100px;
  height: 100px;
  z-index: 1000;
  border-radius: 50%;
  background-color:  #27e1bc;
  box-shadow: 0 2px 10px rgba(0, 0, 0, 0.3);
  display: flex;
  align-items: center;
  justify-content: center;
  transition: background-color 0.3s;
}

/* Cambio de color al pasar el ratón sobre el botón */
.call-button:hover {
  background-color:#8A63F1;
}

.call-button img.call-icon {
  width: 80px;
  height: 80px;
}

</style>
