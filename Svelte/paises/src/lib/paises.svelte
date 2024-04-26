<script>
  export let pais;
  let p;

  const paises = {
    colombia: [
      "Colombia",
      "Bogota",
      "51,52 Millones",
      "Peso Colombiano",
      "1,142 Millones km°",
      "colombia.png",
      "Colombia, antigua colonia española, logró su independencia en el siglo XIX. Enfrentó guerras civiles y conflictos internos, y en el siglo XX se vio afectada por el narcotráfico y la violencia asociada. Actualmente, busca la paz tras décadas de conflicto armado interno, aunque enfrenta desafíos como la desigualdad social y la corrupción.",
    ],
    venezuela: [
      "Venezuela",
      "Caracas",
      "28,2 Millones",
      "Bolivar",
      "916,445 km°",
      "venezuela.png",
      "La historia de Venezuela incluye la colonización española, la lucha por la independencia liderada por Simón Bolívar, períodos de dictadura y democracia, y el auge petrolero del siglo XX. En los últimos años, el país ha enfrentado una profunda crisis económica y política bajo el gobierno del chavismo, con graves problemas de hiperinflación y escasez de alimentos y medicinas.",
    ],
    ecuador: [
      "Ecuador",
      "Quito",
      "17,8 Millones",
      "Dolar Estadounidense",
      "256,370 km°",
      "ecuador.png",
      "Ecuador: desde culturas indígenas hasta independencia en el siglo XIX. Desafíos: inestabilidad política, conflictos limítrofes y crisis económicas. Reto actual: superar problemas para un futuro estable y próspero.",
    ],
    peru: [
      "Peru",
      "Lima",
      "33,72 Millones",
      "Sol Peruano",
      "1.285.215 km°",
      "peru.png",
      "Culturas precolombinas, llegada de los españoles en el siglo XVI, colonización, lucha por la independencia liderada por José de San Martín y Simón Bolívar en el siglo XIX, períodos de inestabilidad política, conflictos internos y externos. Retos actuales incluyen el desarrollo económico y la inclusión social.",
    ],
    brasil: [
      "Brasil",
      "Brasilia",
      "214,3 Millones",
      "Real Brasileño",
      "8,51 km°",
      "brazil.png",
      "Culturas indígenas, colonización portuguesa en el siglo XVI, Imperio brasileño, abolición de la esclavitud en 1888, República en 1889, períodos de dictadura y democracia, economía diversificada, desafíos actuales incluyen la desigualdad social y la conservación ambiental.",
    ],
    argentina: [
      "Argentina",
      "Buenos Aires",
      "46.2 Millones",
      "Peso Argentino",
      "671,370 km°",
      "argentina.png",
      "En 1826, en plena lucha entre unitarios y federales, un Congreso General Constituyente reunido en Buenos Aires sancionó una Constitución de vida efímera en la que oficializaba el nombre de Nación Argentina, que no logró imponerse por estar vinculado a la supremacía porteña",
    ],
  };

  p = paises[pais];
</script>

<div class="card mb-3" style="max-width: 540px;">
  <div class="row g-0">
    <div class="col-md-4">
      <img
        src="./src/assets/{p[5]}"
        class="img-fluid rounded-start"
        alt="Bandera_Sudamericana"
      />
    </div>
    <div class="col-md-8">
      <div class="card-body">
        <div><h5 class="fw-bolder">{p[0]}</h5></div>
        <div>
          <small>Capital: </small><code class="font-monospace">{p[1]}</code>
        </div>
        <div>
          <small>Poblacion: </small><code class="font-monospace">{p[2]}</code>
        </div>
        <div>
          <small>Moneda: </small><code class="font-monospace">{p[3]}</code>
        </div>
        <div>
          <small>Extencion: </small><code class="font-monospace">{p[4]}</code>
        </div>
        <p class="card-text">{p[6]}</p>
      </div>
    </div>
  </div>
</div>
