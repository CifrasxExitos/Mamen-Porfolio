---
layout: single
title: "📊 Proyectos y TFM"
permalink: /projects/
---

<div class="projects-tfm-section">
  <!-- Columna 1: Trabajos de Fin de Máster -->
  <div class="column tfm-column">
    <h2>Trabajos de Fin de Máster (TFM)</h2>
    <!-- Tarjeta TFM 1 -->
    <div class="card">
      <img src="URL_IMAGEN_TFM1" alt="Imagen del TFM 1">
      <h3>Título del TFM 1</h3>
      <p>Breve descripción del TFM 1, destacando objetivos y resultados clave.</p>
      <a href="https://github.com/usuario/TFM1" class="btn btn--primary" target="_blank">Ver en GitHub</a>
    </div>
    <!-- Tarjeta TFM 2 (opcional) -->
    <div class="card">
      <img src="URL_IMAGEN_TFM2" alt="Imagen del TFM 2">
      <h3>Título del TFM 2</h3>
      <p>Breve descripción del TFM 2, destacando objetivos y resultados clave.</p>
      <a href="https://github.com/usuario/TFM2" class="btn btn--primary" target="_blank">Ver en GitHub</a>
    </div>
    <!-- ...añadir más tarjetas de TFM si es necesario -->
  </div>

  <!-- Columna 2: Proyectos Destacados -->
  <div class="column projects-column">
    <h2>Proyectos Destacados</h2>
    <!-- Tarjeta Proyecto 1 -->
    <div class="card">
      <img src="URL_IMAGEN_PROY1" alt="Imagen del Proyecto 1">
      <h3>Nombre del Proyecto 1</h3>
      <p>Breve descripción del Proyecto 1, mencionando las tecnologías usadas y su propósito.</p>
      <a href="https://github.com/usuario/Proyecto1" class="btn btn--primary" target="_blank">Ver en GitHub</a>
    </div>
    <!-- Tarjeta Proyecto 2 -->
    <div class="card">
      <img src="URL_IMAGEN_PROY2" alt="Imagen del Proyecto 2">
      <h3>Nombre del Proyecto 2</h3>
      <p>Breve descripción del Proyecto 2, mencionando las tecnologías usadas y su propósito.</p>
      <a href="https://github.com/usuario/Proyecto2" class="btn btn--primary" target="_blank">Ver en GitHub</a>
    </div>
    <!-- ...añadir más tarjetas de proyectos según sea necesario -->
  </div>
</div>

/* Contenedor de la sección con dos columnas (TFM y Proyectos) */
.projects-tfm-section {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 2rem;               /* espacio entre columnas y filas */
  align-items: start;      /* alineación superior de las tarjetas en cada columna */
}

/* Columna individual (puedes agregar estilos adicionales si hace falta) */
.projects-tfm-section .column {
  /* Ejemplo: agregar un pequeño padding interno 
     padding: 0.5rem;
     */
}

/* Tarjeta de proyecto/TFM */
.projects-tfm-section .card {
  background: #fff;
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 0 2px 6px rgba(0,0,0,0.1);
  overflow: hidden;  /* para que bordes redondeados afecten a la imagen */
  padding: 1rem;
  margin-bottom: 1.5rem;  /* separación inferior entre tarjetas */
  transition: transform 0.2s ease-in-out, box-shadow 0.2s ease-in-out;
}

/* Efecto hover en la tarjeta: ligeramente elevada con sombra más intensa */
.projects-tfm-section .card:hover {
  transform: translateY(-4px);
  box-shadow: 0 4px 12px rgba(0,0,0,0.2);
}

/* Imagen dentro de la tarjeta */
.projects-tfm-section .card img {
  width: 100%;
  height: auto;
  display: block;
  margin-bottom: 0.5rem;
  /* Opcional: border-bottom o efecto hover en imagen, según se desee */
}

/* Títulos dentro de las tarjetas */
.projects-tfm-section .card h3 {
  margin: 0.5rem 0 0.5rem 0;
  font-size: 1.2rem;
  color: #333;
}

/* Botón de GitHub dentro de la tarjeta */
.projects-tfm-section .card a.btn {
  display: inline-block;
  margin-top: 0.5rem;
  /* Los estilos de color/fondo del botón provienen de la clase .btn--primary del tema */
}

/* Título de cada columna (sección) */
.projects-tfm-section h2 {
  text-align: center;
  font-size: 1.5rem;
  margin-bottom: 1rem;
}

/* Media query para dispositivos móviles: una columna en lugar de dos */
@media (max-width: 768px) {
  .projects-tfm-section {
    grid-template-columns: 1fr;   /* una sola columna */
  }
}
