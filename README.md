## Analisis de crédito al sector privado y exportaciones en Piura

# Pregunta guía 

¿En qué medida el crédito directo del sistema financiero al sector privado en Piura impacta en el nivel de exportaciones del departamento?

# Descripción General

Exploramos la relación entre el crédito directo al sector privado en Piura y las exportaciones, incorporando el Índice Costero El Niño (ICEN) como proxy de choques climáticos. Usamos datos mensuales 2005–2022 para construir un panel limpio y alineado, visualizar distribuciones, comparar dinámicas Piura vs. Perú y evaluar co-movimientos (correlaciones) y regularidades empíricas.

# Fuentes de datos (mensual)

Fuente principal: API del Banco Central de Reserva del Perú (BCRP)

Servicio oficial que entrega series macroeconómicas en formato JSON; garantiza trazabilidad, periodicidad mensual y metadatos consistentes.

Series 

- Crédito total nacional: Stock agregado de crédito al sector privado en todo el país; sirve como referencia para comparar el ciclo crediticio de Piura con la dinámica nacional.

- Crédito directo al sector privado a nivel de Piura (moneda nacional, moneda extranjera): Stock de préstamos del sistema financiero a empresas y hogares en Piura, desagregado en moneda nacional (MN) y moneda extranjera (ME); indica profundidad financiera regional y composición cambiaria.

- Exportaciones de Piura (FOB, US$): Valor mensual de ventas externas originadas en Piura a precios FOB en dólares; capta el desempeño exportador regional.

- Exportaciones nacionales (FOB, US$): Valor total de exportaciones del Perú; permite contextualizar a Piura dentro del patrón exportador agregado y su exposición a ciclos globales.

- Tipo de cambio promedio (S/ por US$): Cotización mensual promedio del sol frente al dólar; se usa para convertir exportaciones de US$ a S/ y para análisis de precios relativos. 

Fuente Índice Costero del Niño (ICEN): API del Instituto Geofísico del Perú (IGP)

Índice mensual del calentamiento/enfriamiento costero (Niño/Niña). Valores positivos sugieren Niño; negativos, Niña. Se utiliza como proxy de choques climáticos sobre la producción/exportación.

# Procedimiento

- Obtención de datos (BCRP)
- Limpieza macro y estandarización temporal
- Carga, limpieza y filtrado del ICEN
- Homologación de fechas y unión de variables macroeconómicas e Índice Costero del Niño
- Gráficos
  - Distribución Normal
  - Mapas  de calor
  - Boxplot
  - Series de tiempo
    
# Conclusión

- El crédito total en Piura y el nacional comparten una misma tendencia ascendente entre 2005 y 2022, reflejando la expansión del sistema financiero peruano. La diferencia central está en la escala: mientras Piura se mide en miles de millones, el crédito nacional se mide en cientos de miles de millones. Esto evidencia que Piura sigue de cerca la dinámica nacional, aunque con un peso proporcionalmente pequeño en el total del país.
  
- Las exportaciones de Piura muestran una distribución concentrada en valores bajos (300–700 millones) pero con picos esporádicos que llegan hasta los 2000 millones, reflejo de su alta dependencia en productos agroexportadores y pesqueros sensibles a factores externos. En contraste, las exportaciones nacionales son más estables, con valores mayormente entre 8000 y 12000 millones y menos afectados por choques puntuales, gracias a una canasta más diversificada. Esto marca la diferencia entre una región volátil y un país más resiliente.
  
- El Índice Costero El Niño (ICEN) presenta valores que oscilan alrededor de cero, reflejando condiciones normales la mayor parte del tiempo, pero con desviaciones notables en eventos extremos. Los picos positivos (El Niño) y negativos (La Niña) afectan directamente a las exportaciones, especialmente en Piura. El caso más claro fue 2017, cuando un fuerte Niño costero coincidió con una caída marcada en las exportaciones regionales, mostrando cómo la variabilidad climática impacta en sectores dependientes de condiciones ambientales.
  
- El crédito en Piura y el nacional están casi perfectamente correlacionados, mostrando que el dinamismo financiero regional replica al nacional. Las exportaciones de Piura y del país también se mueven juntas, aunque con más independencia. El ICEN, en cambio, tiene correlaciones negativas débiles, lo que indica que su impacto sobre exportaciones es visible pero limitado y sobre el crédito casi nulo. Esto diferencia los factores macrofinancieros (más estables) de los climáticos (más volátiles y específicos).
