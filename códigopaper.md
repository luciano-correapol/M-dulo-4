---
title: "LA INDUSTRIA DE LAS PASTAS ALIMENTICIAS"
subtitle: "Estructura, Dinámica Competitiva, Innovación Tecnológica y Perspectivas del Sector a Nivel Global y en Argentina"
author: |
  | Aguirre Simionato, Juan Marcos
  | Scala, Enzo
  | Correa Pol, Luciano
  | Vera, Tomás
  | Cabrera, Tomás
  |
  | *Pasta Inteligente — Proyecto de Análisis Económico*
  | *Facultad de Ingeniería · Cátedra de Economía*
date: "Mendoza, Argentina · 2026"
output: 
  pdf_document:
    number_sections: true
    toc: true
    toc_depth: 3
geometry: "left=3cm, right=2.5cm, top=2.5cm, bottom=2.5cm"
fontsize: 11pt
header-includes:
  - \usepackage{caption}
  - \captionsetup[table]{name=Tabla}
  - \usepackage{booktabs}
  - \usepackage{longtable}
  - \usepackage{array}
  - \usepackage{multirow}
  - \usepackage{float}
  - \usepackage{hyperref}
  - \usepackage{xcolor}
  - \definecolor{azuloscuro}{HTML}{0f3460}
  - \hypersetup{colorlinks=true, linkcolor=azuloscuro, urlcolor=azuloscuro}
---

```{r setup, include=FALSE}
knitr::opts_chunk$set(
  echo    = FALSE,
  warning = FALSE,
  message = FALSE,
  fig.align = "center",
  fig.pos  = "H"
)

# Paquetes necesarios
# install.packages(c("knitr", "kableExtra", "ggplot2", "dplyr", "scales"))
library(knitr)
library(kableExtra)
library(ggplot2)
library(dplyr)
library(scales)
```

\vspace{0.5cm}

> *Este documento integra información de fuentes primarias y secundarias verificadas: International Pasta Organisation (IPO), Unión de Industriales Fideeros de la República Argentina (UIFRA), INDEC, INTA, Molinos Río de la Plata S.A. y publicaciones científicas arbitradas.*

\newpage

# Resumen {-}

Las pastas alimenticias constituyen uno de los alimentos más consumidos a nivel mundial, con una producción global que superó los 17 millones de toneladas métricas en 2023 y un mercado valorado en USD 26,87 mil millones. Este trabajo analiza en profundidad la industria fideera desde una perspectiva económica, tecnológica y estructural, abarcando las dimensiones global y local (Argentina/región de Cuyo). Se examinan la cadena de valor, la estructura oligopólica del mercado, la dinámica de costos de materias primas, las tendencias de innovación —con especial atención a la tecnología de pasta con memoria de forma desarrollada por Tao et al. (2021) en *Science Advances*—, los flujos de comercio exterior, las regulaciones aplicables y las perspectivas de crecimiento proyectadas hasta 2030. Los resultados muestran un sector en expansión sostenida impulsado por urbanización, demanda de conveniencia y diferenciación de producto, con importantes oportunidades para productores de escala pequeña y mediana que apuesten por innovación y sustentabilidad.

**Palabras clave:** pastas alimenticias, industria fideera, memoria de forma, trigo candeal, mercado oligopólico, innovación alimentaria, Molinos Río de la Plata, UIFRA, IPO, Cuyo.

---

# Introducción

Las pastas alimenticias son el resultado de la transformación industrial del trigo —principalmente trigo candeal (*Triticum turgidum* L. subsp. *durum*) o trigo harinero (*Triticum aestivum*)— en productos de alto consumo masivo distribuidos a escala global. Su historia se remonta siglos atrás en la cuenca mediterránea, pero su industrialización masiva se consolidó en el siglo XX de la mano de tecnologías de extrusión, laminado y secado continuo que permitieron producir grandes volúmenes a costos decrecientes (Ignacio, 2016).

En la actualidad, la industria enfrenta tensiones simultáneas: competencia por precio en el segmento de *commodities*, presión ambiental para reducir *packaging* y huella de carbono, y oportunidades de diferenciación a través de innovación de producto. En este contexto emergen desarrollos científicos como el de las pastas con memoria de forma (Tao et al., 2021), que proponen una reconfiguración radical del paradigma productivo: separar la forma final del producto de su geometría durante el almacenamiento y transporte.

El presente trabajo aborda la industria fideera desde múltiples ángulos: estructura de mercado, cadena productiva, materias primas, regulación, comercio exterior, innovación tecnológica y perspectivas económicas. Se presta atención especial al caso argentino, donde la industria tiene raíces culturales profundas vinculadas a la inmigración italiana y donde la estructura oligopólica está dominada principalmente por Molinos Río de la Plata S.A. El análisis integra datos del mercado de Cuyo como caso de aplicación regional.

## Objetivos del trabajo

Los objetivos específicos son:

* Caracterizar la estructura y dinámica de la industria fideera a nivel global y local.
* Analizar la cadena de valor y los factores de costo en la producción de pastas secas.
* Examinar la dinámica de innovación tecnológica, con foco en pastas morfantes.
* Describir el comercio exterior argentino de pastas y su evolución reciente.
* Identificar tendencias de consumo, regulación y sustentabilidad aplicables al sector.
* Proveer un marco de referencia para la evaluación de proyectos de inversión en el sector.

# Contexto Histórico y Cultural

## Orígenes y expansión global

La pasta seca como producto industrial de consumo masivo tiene sus raíces en el sur de Italia, particularmente en las regiones de Campania y Sicilia, donde las condiciones climáticas favorecían el cultivo de trigo candeal y el secado natural al aire libre. La difusión global fue impulsada por las oleadas migratorias europeas de los siglos XIX y XX, que transportaron no solo el producto sino también las técnicas de elaboración y los hábitos de consumo.

Italia mantiene su posición como líder mundial tanto en producción como en consumo per cápita: en 2023 produjo 3,9 millones de toneladas y sus ciudadanos consumen 23,3 kg por persona al año, seguida por Túnez (17 kg), Venezuela (13,6 kg) y Grecia (12,2 kg) (IPO, 2024). Según datos de IPO para el World Pasta Day 2024, la producción global en 2023 alcanzó casi 17 millones de toneladas, distribuidas en 52 países con consumo mínimo de 1 kg per cápita al año —frente a 30 países que superaban ese umbral hace una década.

## La pasta en Argentina: herencia y consumo

Argentina representa el caso más notable de apropiación cultural de la pasta fuera de Italia. La inmigración italiana masiva entre 1880 y 1950 —que llevó a que en 1914 el 13% de la población total fuera italiana o de origen italiano— consolidó a la pasta como un alimento estructural de la dieta argentina (Ignacio, 2016).

El consumo per cápita argentino fue de 7,39 kg/hab en 2020 según la UIFRA (2020), con tendencias al alza en años posteriores hasta alcanzar estimaciones de 14 kg/hab en algunos relevamientos de 2023 que incluyen pasta fresca y otras variedades (Informes de Expertos, 2026). La discrepancia entre estas cifras obedece a diferencias metodológicas en la definición del universo medido.

Culturalmente, la tradición de comer fideos los días 29 de cada mes —usualmente con monedas debajo del plato para atraer prosperidad— ilustra la profundidad de la integración de la pasta en la identidad gastronómica argentina, más allá de su función nutricional.

# El Mercado Global de Pastas

## Tamaño, valor y proyecciones

El mercado global de pastas alimenticias fue valuado en USD 26,87 mil millones en 2023 y se proyecta alcanzar USD 35,08 mil millones en 2030, con una tasa de crecimiento anual compuesta (CAGR) del 3,88% para el período 2024-2030 (ResearchAndMarkets.com, 2024; IPO, 2024). Este crecimiento está impulsado principalmente por:

* **Urbanización acelerada:** especialmente en Asia y África, donde la pasta se posiciona como alimento conveniente y de bajo costo para poblaciones urbanas con restricciones de tiempo.
* **Demanda de salud y bienestar:** que impulsa la pasta integral, sin gluten, con proteína vegetal añadida y con legumbres.
* **Innovación de producto:** que expande el mercado hacia segmentos premium y hacia consumidores que buscan experiencias gastronómicas diferenciadas.
* **Sustentabilidad:** donde la pasta seca tiene una huella ambiental notablemente menor que las proteínas animales, favoreciendo su posicionamiento en dietas flexitarianas y veganas.

```{r tabla-consumo}
tabla1 <- data.frame(
  "País / Región"               = c("Italia", "Túnez", "Venezuela", "Grecia",
                                    "Perú", "Chile", "Alemania", "EE.UU.",
                                    "Francia", "Argentina (est.)"),
  "Consumo (kg/hab/año)"        = c(23.3, 17.0, 13.6, 12.2, 9.9, 9.6, 9.3, 8.8, 8.6, 7.4),
  "Posición"                    = c("1°","2°","3°","4°","5°","6°","7°","8°","9°","~11°"),
  "Tendencia"                   = c("Estable","Creciente","Variable","Estable",
                                    "Creciente","Creciente","Estable","Creciente",
                                    "Estable","Creciente"),
  check.names = FALSE
)

kable(tabla1,
      caption = "Consumo per cápita de pasta por país (2023–2024). Fuente: IPO (2024); UIFRA (2020).",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position", "scale_down"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white")
```

```{r grafico-consumo, fig.cap="Consumo per cápita de pasta por país (kg/hab/año, 2023). Fuente: IPO (2024).", fig.height=4, fig.width=7}
tabla1 |>
  arrange(desc(`Consumo (kg/hab/año)`)) |>
  mutate(`País / Región` = factor(`País / Región`,
                                   levels = rev(`País / Región`))) |>
  ggplot(aes(x = `País / Región`, y = `Consumo (kg/hab/año)`,
             fill = `Consumo (kg/hab/año)`)) +
  geom_col(width = 0.7) +
  geom_text(aes(label = `Consumo (kg/hab/año)`),
            hjust = -0.15, size = 3, color = "#333333") +
  scale_fill_gradient(low = "#a8c4e0", high = "#0f3460") +
  coord_flip() +
  scale_y_continuous(limits = c(0, 27), expand = c(0, 0)) +
  labs(x = NULL, y = "kg por habitante por año") +
  theme_minimal(base_size = 10) +
  theme(legend.position = "none",
        panel.grid.major.y = element_blank(),
        panel.grid.minor   = element_blank(),
        axis.text.y        = element_text(color = "#333333"))
```

## Estructura de la producción global

La producción de pasta seca es una industria capital-intensiva con altas economías de escala. Según IPO (2024), en 25 años la producción global creció casi el 85%, pasando de 9,1 a 17 millones de toneladas. Hoy 40 países producen más de 20.000 toneladas anuales. La concentración industrial es alta: pocas empresas multinacionales (Barilla, De Cecco, La Molisana en el segmento italiano; grupos industriales locales en cada mercado) controlan la mayor parte del volumen producido.

La tendencia global apunta hacia la diferenciación de producto: crece la demanda por pastas con atributos funcionales (proteína de legumbres, pasta enriquecida, pasta para deportistas) y con características que responden a restricciones dietarias (sin TACC, baja en índice glucémico).

# La Industria Fideera Argentina

## Estructura industrial y concentración

La industria de pastas secas en Argentina ha experimentado un intenso proceso de consolidación desde los años 1990. El número de establecimientos productores pasó de 110 en el año 2000 a aproximadamente 70 en 2013, mientras que la producción total creció casi un 40% en el mismo período. Este fenómeno configura un **oligopolio con diferenciación de producto** donde pocas firmas controlan la mayor parte del *market share*.

La principal característica estructural del mercado es que, detrás de 12 o 14 marcas presentes en la góndola, operan en realidad apenas 2 o 3 empresas (UIFRA, citado en ialimentaria.com.ar, 2018). Las principales barreras de entrada son:

* **Economías de escala:** las líneas modernas son rentables solo por encima de ciertos volúmenes mínimos.
* **Acceso a canales de distribución:** los supermercados de grandes cadenas requieren volumen, capital de trabajo y capacidad logística.
* **Reconocimiento de marca:** el consumidor argentino muestra alta lealtad a marcas con décadas de presencia.
* **Inversión en maquinaria:** una línea completa puede requerir varios millones de dólares.

El estudio de Ignacio (2016) confirma que los 6 establecimientos líderes concentran el 72% del *market share* total de pastas secas en Argentina, nivel consistente con la teoría de oligopolio: pocas empresas, interdependencia estratégica y competencia principalmente vía diferenciación de producto.

## Molinos Río de la Plata: el líder dominante

Molinos Río de la Plata S.A. es la compañía líder del mercado argentino de alimentos, fundada en 1897. Opera con un portafolio multi-marca que le permite cubrir diferentes segmentos simultáneamente:

```{r tabla-molinos}
tabla2 <- data.frame(
  "Marca"      = c("Lucchetti", "Matarazzo", "Don Vicente", "Favorita", "Del Verde"),
  "Segmento"   = c("Medio-alto", "Estándar", "Diferenciado", "Económico", "Económico"),
  "Posición"   = c("Premium nacional", "Medio", "Medio-alto", "Bajo", "Bajo"),
  "Cuota (Nielsen, 2011)" = c("13,7%", "13,5%", "4,0%", "N/D", "N/D"),
  check.names  = FALSE
)

kable(tabla2,
      caption = "Marcas de pasta de Molinos Río de la Plata y cuotas de mercado. Fuente: Nielsen Argentina (2011).",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white")
```

En términos financieros, Molinos cerró 2023 con una facturación de \$432.856 millones y una ganancia neta de \$46.225 millones. En 2024, los ingresos cayeron un 6,4% (de \$942.672 a \$882.117 millones), reflejando el impacto de la contracción del consumo masivo en Argentina (Ambito, 2025). La empresa cuenta con 2.600 empleados y 14 plantas de producción, y exporta a más de 20 países.

## Otros actores relevantes

* **Marolio:** opera en el segmento económico con estrategia exportadora activa hacia Brasil, Chile, Bolivia, Colombia y Ecuador.
* **Don Felipe (Grupo Arcor):** competidor en el segmento medio-alto.
* **PyMEs regionales:** pequeñas y medianas empresas que abastecen mercados locales con ventaja de proximidad.
* **Barilla / La Molisana (importados):** presentes en el segmento premium, con precios que triplican o cuadruplican las marcas nacionales.

## Empleo e impacto económico

La industria fideera argentina genera más de 2.200 puestos de trabajo directos, regulados principalmente por el **Convenio Colectivo de Trabajo N° 119/90** (CCT 119/90), que establece categorías, escalas salariales y condiciones de trabajo para los trabajadores nucleados en el Sindicato Argentino de Trabajadores de la Industria Fideera (SATIF). En los ciclos paritarios 2022-2023 y 2023-2024 se acordaron incrementos salariales del 64% y 87% respectivamente, impactando directamente en los costos fijos de las empresas del sector.

# Cadena de Valor y Proceso Productivo

## Eslabones de la cadena

```{r tabla-cadena}
tabla3 <- data.frame(
  "Eslabón"     = c("1. Producción primaria", "2. Molienda", "3. Fabricación",
                    "4. Packaging", "5. Distribución",
                    "6. Comercialización", "7. Consumo final"),
  "Descripción" = c(
    "Cultivo de trigo (pan o candeal). Provincias de Buenos Aires, Córdoba, Santa Fe y Entre Ríos. Argentina produce ~20 Mt de trigo/año.",
    "Transformación del trigo en harina o semolina. Alta concentración industrial: Molinos Agro, Cargill, AGD, Bunge.",
    "Proceso de amasado, laminado/extrusión, corte, secado y empaque. Núcleo de la cadena.",
    "Provisión de envases: BOPP (polipropileno biorientado), cartón, plástico. Impacto ambiental significativo.",
    "Canal moderno (supermercados, hipermercados) y canal tradicional (almacenes, autoservicios). Distribución tercerizada.",
    "Supermercados líderes: Carrefour, La Anónima, Coto, Jumbo, DIA. Márgenes brutos del 30-35% sobre precio de lista.",
    "Hogares (consumo doméstico) y canal HORECA (hoteles, restaurantes, catering)."
  ),
  check.names = FALSE
)

kable(tabla3,
      caption = "Cadena de valor de la industria de pastas secas en Argentina. Elaboración propia.",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position", "scale_down"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white") |>
  column_spec(1, bold = TRUE, width = "3.5cm") |>
  column_spec(2, width = "10cm")
```

## Proceso productivo estándar

La elaboración industrial de pasta seca sigue un proceso estandarizado con variantes según el tipo de producto:

1. **Recepción y control de materia prima:** control de humedad, granulometría y calidad proteica de la semolina.
2. **Amasado:** mezcla de semolina con agua (~40% p/p) durante 15-20 minutos.
3. **Reposo:** 10-15 minutos para relajar la red de gluten.
4. **Laminado o extrusión:** para pastas largas (laminado) o formas complejas (extrusión). En pastas morfantes: estampado de ranuras en la etapa de laminado.
5. **Corte:** a las dimensiones específicas de cada forma.
6. **Secado:** paso crítico a 40-60°C durante 6-8 horas, hasta alcanzar humedad final \< 12,5% (norma ANMAT/SENASA).
7. **Control de calidad:** verificación de humedad, peso, color e integridad estructural.
8. **Envasado:** en bolsas de BOPP o cajas de cartón, en presentaciones de 500 g o 1 kg.
9. **Distribución:** paletizado y despacho a centros de distribución.

## Costos de producción y estructura de precios

```{r tabla-costos}
tabla4 <- data.frame(
  "Componente"           = c("Semolina de trigo candeal", "Mano de obra directa",
                             "Energía (electricidad, gas)", "Packaging (BOPP, cartón)",
                             "Amortización de maquinaria", "Logística y distribución",
                             "Marketing y comercialización", "Alquiler de planta",
                             "Otros (servicios, admin.)"),
  "Participación est."   = c("35-45%", "10-15%", "8-12%", "5-8%",
                              "4-6%", "3-5%", "3-5%", "2-4%", "5-8%"),
  "Naturaleza"           = c("Variable", "Fijo", "Semivariable", "Variable",
                              "Fijo", "Variable", "Semivariable", "Fijo", "Fijo/Variable"),
  check.names = FALSE
)

kable(tabla4,
      caption = "Estructura de costos de producción de pasta seca, PyME de calidad diferenciada. Elaboración propia.",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white")
```

La distribución del precio de venta al consumidor para un paquete de 500 g (\$3.000 ARS, Mendoza, 2026) es la siguiente:

```{r grafico-pvp, fig.cap="Distribución del precio de venta al consumidor (PVP = \\$3.000 ARS, pasta seca diferenciada, Mendoza 2026). Elaboración propia.", fig.height=3.5, fig.width=6}
pvp_df <- data.frame(
  concepto = c("IVA (21%)", "Margen\nsupermercado", "Costos\ncomerciales",
               "Costo\nproducción", "Ganancia\nfabricante"),
  pct      = c(21, 31.3, 5, 33.1, 9.6),
  ars      = c(630, 940, 150, 993, 287)
)

pvp_df |>
  mutate(concepto = factor(concepto, levels = rev(concepto))) |>
  ggplot(aes(x = concepto, y = pct, fill = concepto)) +
  geom_col(width = 0.65, show.legend = FALSE) +
  geom_text(aes(label = paste0(pct, "%\n($", format(ars, big.mark = "."), ")")),
            hjust = -0.08, size = 2.8) +
  scale_fill_manual(values = c("#e94560","#0f3460","#533483","#16213e","#a8c4e0")) +
  coord_flip() +
  scale_y_continuous(limits = c(0, 42), expand = c(0,0)) +
  labs(x = NULL, y = "% del PVP") +
  theme_minimal(base_size = 10) +
  theme(panel.grid.major.y = element_blank(),
        panel.grid.minor   = element_blank(),
        axis.text.y        = element_text(color = "#333333"))
```

# Materias Primas: Trigo y Semolina

## Trigo candeal: el insumo crítico

El trigo candeal (*Triticum turgidum* L. subsp. *durum*) es la materia prima fundamental para la pasta de calidad. Su molienda produce semolina, una harina gruesa de color amarillo intenso con alto contenido proteico (12-15%) y una estructura de gluten que confiere firmeza y resistencia a la sobrecocción (INTA, 2019).

El mercado de trigo candeal en Argentina es lo que el INTA (2019) denomina un "mercado cerrado": los acuerdos entre productores agrícolas y la industria molinera se realizan directamente, tomando como precio base el del trigo pan más un *plus* variable. Las principales zonas productoras se concentran en el sur de Córdoba, sur de Santa Fe y norte de Buenos Aires.

## Volatilidad de precios y riesgo de abastecimiento

El precio internacional del trigo es una de las variables con mayor impacto en los costos de la industria. Episodios recientes relevantes:

* **Campaña 2022/2023:** sequía severa redujo la cosecha a 12,6 Mt, generando presión alcista sobre precios domésticos.
* **Campaña 2023/2024:** recuperación parcial a ~15,9 Mt. El precio en Matba Rofex subió más del 20% entre marzo y mayo de 2024 (de USD 203 a USD 253,50/t).
* **Campaña 2025/2026:** cosecha estimada en 22 Mt, cercana al récord histórico de 22,4 Mt de 2021/22 (Diario de Cuyo, 2025).

A nivel global, el conflicto Rusia-Ucrania sigue siendo factor de incertidumbre, dado que ambos países representan juntos más del 25% de las exportaciones mundiales de trigo. Las estrategias de cobertura disponibles para el fabricante incluyen contratos de abastecimiento a precio fijo, operaciones de futuros en Matba Rofex y gestión de inventario estratégico.

# Innovación Tecnológica: Pasta Morfante y 4D Food Printing

## El paradigma de la pasta con memoria de forma

La investigación de Tao et al. (2021), publicada en *Science Advances* (DOI: 10.1126/sciadv.abf4098), representa un punto de inflexión en el diseño de pastas alimenticias. El equipo —integrado por 17 investigadores de Carnegie Mellon University, Syracuse University y Zhejiang University— demostró que es posible programar la forma tridimensional final de una pasta mediante el estampado de ranuras asimétricas en una cara de la lámina plana durante el proceso de laminado.

El mecanismo es puramente físico: las ranuras incrementan el tiempo de hidratación y expansión de esa zona durante la cocción. La cara sin ranuras se hidrata y expande más rápidamente, generando una curvatura diferencial controlada y reproducible. La innovación matemática central es un modelo computacional predictivo que permite diseñar el patrón de ranuras (ancho, profundidad, separación) para obtener con precisión cualquier forma tridimensional deseada, transformando el proceso de diseño experimental en un sistema computacionalmente guiado.

## Antecedente: MIT Media Lab (2017)

El trabajo del MIT Media Lab de 2017 constituye el antecedente directo: el equipo investigó la respuesta de materiales a la humedad y extendió el principio a láminas de pasta comestibles. El dato más citado es que "al empacar macarrones perfectamente, el 67% del volumen es aire" (MIT Media Lab, 2017), lo que fundamenta cuantitativamente la ventaja logística de las pastas en formato plano. La diferencia con Tao et al. (2021) es que el MIT estableció el concepto como prueba de concepto sin desarrollar el modelo matemático subyacente.

## Desarrollos posteriores (2024-2026)

La literatura científica reciente confirma la consolidación de esta línea de investigación:

* **Severini et al. (2026)** — *Journal of Food Engineering*, 402, 112700: sistema semi-automatizado para crear ranuras de profundidad variable en *snacks* de base cereal, extendiendo la tecnología más allá de la pasta.
* **Bhandari et al. (2026)** — *Journal of Food Engineering*, 404, 112778: morfosis controlada de bicapas de proteína vegetal bajo condiciones de procesamiento térmico.
* **Derossi et al. (2024)** — *Journal of Food Engineering*: caracterización de los cambios de forma dinámicos durante la cocción con técnicas de imagen de alta resolución.

## Ventajas industriales y ambientales

```{r tabla-ventajas}
tabla6 <- data.frame(
  "Dimensión"      = c("Logística", "Packaging", "Almacenamiento",
                       "Ambiental", "Energía de cocción", "Regulatoria"),
  "Ventaja"        = c("Reducción del volumen de aire en envase",
                       "Menor superficie de envase por unidad",
                       "Mayor densidad de producto por pallet",
                       "Menor huella de carbono en transporte",
                       "Mayor área superficial efectiva",
                       "Sin aditivos ni cambios de formulación"),
  "Cuantificación" = c("50-65% menos volumen vs. formas 3D",
                       "~40% menos material de envase",
                       "Hasta 2× unidades por pallet",
                       "Proporcional a reducción de volumen",
                       "No cuantificado en literatura industrial",
                       "Equivalente a pasta seca estándar (ANMAT)"),
  check.names = FALSE
)

kable(tabla6,
      caption = "Ventajas industriales de la pasta con memoria de forma. Fuente: Tao et al. (2021); MIT Media Lab (2017); elaboración propia.",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position", "scale_down"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white")
```

# Comercio Exterior

## Exportaciones argentinas

Las exportaciones crecieron sostenidamente, pasando de 23.817 t y USD 13,9 M (2019) a 35.620 t y USD 23,3 M (2023), un incremento del 49,6% en volumen. Los principales destinos son Brasil, Chile, Bolivia, Colombia, Ecuador y Estados Unidos. Según el presidente de UIFRA, Juan Manuel Airoldes, "el mercado externo recién se abrió hace 14 años" (La Nación, 2024), con el primer impulso exportador en 2011 a raíz de un problema de capacidad en la industria chilena.

```{r grafico-exportaciones, fig.cap="Evolución de las exportaciones argentinas de pasta seca (2019-2023). Fuente: UIFRA (citado en La Nación, 2024).", fig.height=3, fig.width=5.5}
exp_df <- data.frame(
  anio     = c(2019, 2023),
  toneladas = c(23817, 35620),
  usd_mill  = c(13.9, 23.3)
)

ggplot(exp_df, aes(x = factor(anio), y = toneladas, group = 1)) +
  geom_line(color = "#0f3460", linewidth = 1.2) +
  geom_point(size = 5, color = "#e94560") +
  geom_text(aes(label = paste0(format(toneladas, big.mark = "."), " t\nUSD ", usd_mill, " M")),
            vjust = -1.1, size = 3, color = "#333333") +
  scale_y_continuous(limits = c(15000, 42000),
                     labels = label_comma(big.mark = ".")) +
  labs(x = "Año", y = "Toneladas exportadas") +
  theme_minimal(base_size = 10) +
  theme(panel.grid.minor = element_blank())
```

## El debate sobre retenciones

En enero de 2024, el proyecto de Ley Ómnibus propuso aumentar las retenciones a las exportaciones de pastas secas del 4,5% al 15%. La UIFRA se opuso enérgicamente, argumentando que la medida no reconoce la diferencia entre exportar el grano crudo y exportar un producto con valor agregado (La Nación, 2024). La industria fideera, al transformar trigo en pasta, añade entre un 30% y un 70% de valor al producto primario, generando empleo industrial y divisas de mayor calidad.

## Importaciones: el segmento premium

Las importaciones de pasta se concentran en el segmento premium (Barilla, De Cecco, La Molisana), con precios al consumidor de entre \$3.500 y \$4.200 por 500 g en 2026, frente a los \$1.500-\$2.800 de las marcas nacionales. Según datos del IPO (2025), las exportaciones italianas de pasta crecieron a 2,4 millones de toneladas en 2024 (+9,1% interanual), con Argentina entre los países con crecimiento superior al 50% en importaciones de pasta italiana.

# Marco Regulatorio

## Normativa alimentaria

La producción y comercialización de pastas en Argentina está regulada principalmente por el **Código Alimentario Argentino (CAA)**, administrado conjuntamente por ANMAT y SENASA. Los requisitos técnicos fundamentales incluyen:

* Humedad máxima del producto terminado: 12,5%.
* Contenido proteico mínimo para pasta de semolina 100%: establecido por el CAA.
* Rotulado nutricional obligatorio (Resolución Conjunta SPyRS y SAGPA 149/2005 y 683/2005).
* Registro RNPA (Registro Nacional de Productos Alimenticios) obligatorio.
* Habilitación de planta productora ante ANMAT para comercio interprovincial.
* Cumplimiento de Buenas Prácticas de Manufactura (BPM) según GMC/RES 80/96.
* Para exportaciones: certificación SENASA con protocolo específico por país de destino.

## Marco laboral e impositivo

```{r tabla-impuestos}
tabla8 <- data.frame(
  "Impuesto / Arancel"    = c("IVA (pastas secas)", "Ingresos Brutos (Mendoza)",
                               "Impuesto a las Ganancias", "Retenciones a exportación",
                               "Arancel de importación (maquinaria)"),
  "Tasa"                  = c("21%", "~3,5%", "35% (corporativo)",
                               "4,5% (2024)", "0-14% (Mercosur)"),
  "Observaciones"         = c(
    "Tasa general de alimentos elaborados (no la reducida del 10,5%).",
    "Varía por actividad y jurisdicción.",
    "Sobre utilidad neta. PyMEs pueden encuadrar en monotributo.",
    "La Ley Ómnibus (2024) propuso 15%; no aprobado en esos términos.",
    "Arancel externo común Mercosur según posición arancelaria."
  ),
  check.names = FALSE
)

kable(tabla8,
      caption = "Marco impositivo y arancelario relevante para la industria fideera, Argentina 2024-2026. Elaboración propia.",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position", "scale_down"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white") |>
  column_spec(3, width = "6cm")
```

# El Mercado de Cuyo

## Características demográficas y de consumo

La región de Cuyo —Mendoza, San Juan y San Luis— tiene una población total de aproximadamente 3,5 millones de habitantes (INDEC, Censo 2022):

```{r tabla-cuyo}
tabla9 <- data.frame(
  "Indicador"  = c("Población Mendoza", "Población San Juan", "Población San Luis",
                   "Total Cuyo", "Consumo per cápita (pasta seca)",
                   "Consumo total Cuyo/mes (paquetes 500 g)",
                   "Segmento calidad media-alta (~25%)"),
  "Valor"      = c("~2.086.000 hab.", "~818.234 hab.", "~600.000 hab.",
                   "~3.500.000 hab.", "~7,4 kg/hab/año (UIFRA, 2020)",
                   "~4.316.000 paquetes/mes",
                   "~1.079.000 paquetes/mes"),
  check.names = FALSE
)

kable(tabla9,
      caption = "Mercado de pastas secas en Cuyo. Fuente: INDEC Censo 2022; UIFRA 2020; elaboración propia.",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white")
```

## Segmentación del mercado cuyano

```{r tabla-segmentacion}
tabla10 <- data.frame(
  "Segmento"              = c("Económico", "Estándar", "Diferenciado / Calidad", "Premium / Importado"),
  "Precio 500g (ARS)"     = c("$800-$1.500", "$1.500-$2.500", "$2.500-$4.200", "$3.500-$8.500"),
  "% del mercado"         = c("~55%", "~10%", "~25%", "~10%"),
  "Marcas dominantes"     = c("Favorita, Marolio, marcas propias",
                               "Terrabusi, genéricos",
                               "Don Vicente, Matarazzo, Lucchetti, Don Felipe",
                               "Barilla, De Cecco, La Molisana"),
  check.names = FALSE
)

kable(tabla10,
      caption = "Segmentación del mercado de pastas secas en Cuyo, 2026. Elaboración propia.",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position", "scale_down"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white")
```

## Ventajas para un productor local (Maipú, Mendoza)

Una planta productora ubicada en el Parque Industrial de Maipú ofrece ventajas competitivas específicas:

* **Proximidad a puntos de venta:** tiempos de distribución al Gran Mendoza de 1-2 horas, frente a las 12-18 horas desde Buenos Aires para competidores nacionales.
* **Franja logística competitiva:** acceso a la Ruta 7 (corredor bioceánico) para distribución regional a San Juan, San Luis, La Pampa y potencialmente Chile.
* **Mercado menos saturado:** menor concentración de marcas nacionales que en el GBA, facilitando la entrada de productos diferenciados.
* **Costos logísticos reducidos:** la mayor densidad de carga de la pasta morfante amplifica aún más esta ventaja geográfica.

# Tendencias y Perspectivas 2025-2030

## Tendencias globales

* **Salud y bienestar:** crecimiento de pasta integral, con legumbres, sin gluten y alta en proteínas.
* **Sustentabilidad:** presión de *retailers* y consumidores para reducir *packaging* plástico y huella de carbono.
* **Conveniencia:** formatos más prácticos —pasta de cocción rápida (2-3 min), kits de comida con pasta—.
* **Premiumización:** crecimiento del segmento artesanal incluso en mercados de alto consumo.
* **Digitalización:** el e-commerce de alimentos impulsa presentaciones compactas y de mayor vida útil, donde las pastas morfantes tienen ventaja.

## Proyecciones de mercado

```{r tabla-proyecciones}
tabla11 <- data.frame(
  "Indicador"                      = c("Mercado global (USD miles de millones)",
                                       "Producción global (millones de t)",
                                       "Exportaciones ARG (toneladas)",
                                       "Segmento premium ARG (% total)",
                                       "Consumo per cápita ARG (kg/hab)"),
  "2023 (real)"                    = c("26,87", "~17", "35.620", "~7%", "~7,4-14"),
  "2026 (est.)"                    = c("28-30", "~18", "40.000-45.000", "~10%", "~8-15"),
  "2030 (proyección)"              = c("35,08 (IPO)", "~20+", "50.000+", "~12-15%", "~9-16"),
  check.names = FALSE
)

kable(tabla11,
      caption = "Proyecciones del mercado de pastas. Fuente: IPO (2024); UIFRA (2020); ResearchAndMarkets (2024); elaboración propia.",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position", "scale_down"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white")
```

# Viabilidad Económica: El Caso de la Pasta Inteligente en Cuyo

## Propuesta de valor y posicionamiento

El proyecto considera el lanzamiento de una línea de pasta seca con memoria de forma bajo el concepto "Pasta Inteligente" en el mercado de Cuyo, producida en una planta en el Parque Industrial de Maipú, Mendoza. El producto aplica directamente la tecnología de Tao et al. (2021), adaptada a escala industrial mediante la incorporación de un rodillo grabado por CNC en la línea de laminado estándar.

El posicionamiento propuesto ocupa el espacio entre el segmento nacional de calidad (Don Vicente: ~\$2.800) y el segmento importado (Barilla: ~\$4.200), con un precio de lanzamiento de **\$3.100 ARS por paquete de 500 g**.

## Parámetros productivos y financieros

```{r tabla-proyecto}
tabla12 <- data.frame(
  "Parámetro"  = c("Capacidad instalada",
                   "Producción inicial (60% capacidad)",
                   "Precio de góndola (PVP)",
                   "Ingreso neto de fábrica por paquete",
                   "Costo de producción por paquete",
                   "Margen de ganancia por paquete",
                   "Costos fijos mensuales",
                   "Costos variables totales (60.000 uds./mes)",
                   "Punto de equilibrio",
                   "Utilidad neta anual est. (antes de impuestos)",
                   "Personal total"),
  "Valor"      = c("1 Mt/día × 240 días = 480.000 paq./año",
                   "60.000 paq./mes = 720.000 paq./año (2 turnos)",
                   "$3.100 ARS/paquete (500 g)",
                   "~$1.280 ARS (41% del PVP)",
                   "~$993 ARS",
                   "~$287 ARS",
                   "~$17,9 M ARS/mes",
                   "~$39,1 M ARS/mes",
                   "~18,8% de capacidad instalada (~4.500 paq./día)",
                   "~$629 M ARS",
                   "10 personas (7 operarios + 3 admin./comercial)"),
  check.names = FALSE
)

kable(tabla12,
      caption = "Parámetros productivos y financieros del proyecto Pasta Inteligente, Maipú, Mendoza, 2026. Elaboración propia.",
      booktabs = TRUE, linesep = "") |>
  kable_styling(latex_options = c("striped", "hold_position"),
                font_size = 9) |>
  row_spec(0, bold = TRUE, background = "#0f3460", color = "white") |>
  column_spec(1, width = "7cm") |>
  column_spec(2, width = "7cm")
```

## Análisis de viabilidad

* **Punto de equilibrio bajo (18,8%):** amplio margen de seguridad; la empresa cubre costos fijos con apenas 4.500 paquetes diarios.
* **Alta escalabilidad:** operando inicialmente al 60%, se puede alcanzar el 100% de capacidad (~100.000 paq./mes) incorporando un segundo turno sin nueva inversión en maquinaria.
* **Ventaja estructural en logística:** la reducción del volumen de *packaging* permite un margen operativo superior al de competidores con formas 3D convencionales.
* **Riesgo de tipo de cambio:** la maquinaria importada tiene costos en USD, mientras que los ingresos son en pesos; la devaluación afecta el CAPEX inicial pero no el flujo operativo, dado que los insumos principales son de origen nacional.

# Conclusiones

1. **Mercado global en expansión sostenida:** CAGR del 3,88% proyectada hasta 2030 y valor de mercado superior a USD 35.000 millones. La urbanización global y la demanda de conveniencia son los principales motores de crecimiento.

2. **Oligopolio con diferenciación como estructura dominante:** en Argentina, pocas empresas controlan el mercado con múltiples marcas. La barrera de entrada clave no es tecnológica sino de escala mínima eficiente y acceso a canales de distribución. La innovación de producto es el mecanismo más accesible para nuevos competidores.

3. **La tecnología de pasta morfante como oportunidad real:** Tao et al. (2021) y sus continuaciones en 2026 demuestran que la pasta con memoria de forma ha pasado de concepto de laboratorio a tecnología industrialmente implementable, con ventajas logísticas y ambientales cuantificables.

4. **Argentina: fortalezas exportadoras con riesgos macroeconómicos:** el crecimiento exportador del 49,6% entre 2019 y 2023 confirma la competitividad del sector en mercados regionales, aunque la volatilidad del tipo de cambio, la inflación y la incertidumbre regulatoria condicionan la planificación de inversiones.

5. **Cuyo como mercado viable para pasta diferenciada:** la región ofrece un mercado de aproximadamente 1 millón de paquetes mensuales en el segmento diferenciado, con ventajas logísticas para un productor local que se amplifican al usar pasta morfante.

6. **Sustentabilidad como vector estratégico:** la reducción de *packaging*, la menor huella logística y la alineación con dietas de base vegetal posicionan a la pasta morfante de forma consistente con las tendencias globales de consumo responsable.

\newpage
# Referencias {-}

* Ambito (2024, 5 de junio). *PyMEs argentinas de pastas secas buscan crecer en exportaciones*. https://www.ambito.com
* Ambito (2025, 11 de marzo). *La caída del consumo le pegó a Molinos Río de la Plata: su facturación cayó 6,4% en 2024*. https://www.ambito.com
* Bhandari, B. (2026). Controlled shape morphing of plant-based protein bilayers via surface engineering under thermal food processing conditions. *Journal of Food Engineering, 404*, 112778.
* Derossi, A., et al. (2024). Dynamic shape changes of dried pasta during cooking via designed surface grooves. *Journal of Food Engineering*. https://doi.org/10.1016/j.jfoodeng.2024.00428X
* Diario de Cuyo (2025). *Rindes de trigo argentino se acercan a máximos récords*.
* Ignacio, D. L. J. (2016). *Mercado de Pastas Secas en Argentina*. Universidad Torcuato Di Tella.
* Informes de Expertos (2026). *Mercado de Pasta en Argentina: Tamaño, Participación, Crecimiento 2026-2035*.
* INDEC (2023). *Censo Nacional de Población, Hogares y Viviendas 2022*. https://www.indec.gob.ar
* Instituto Nacional de Tecnología Agropecuaria (INTA). (2019). Producción y calidad del trigo candeal en Argentina: análisis del quinquenio 2014/2018. *Revista de Investigaciones Agropecuarias*.
* International Pasta Organisation (IPO). (2024, 24 de octubre). *World Pasta Day 2024: A billion plates of pasta in 10 years to feed the planet*. https://internationalpasta.org
* International Pasta Organisation (IPO). (2025, 20 de mayo). *Italian pasta conquers the world: Record global consumption and export growth*. https://internationalpasta.org
* La Nación (2024, 14 de junio). *Molinos Río de la Plata: un gigante de las góndolas que sufre la baja del consumo pero busca crecer vía compras*.
* La Nación (2024, 26 de enero). *Ley ómnibus: la industria de las pastas secas le reclama a Milei que se las excluya del 15% de retenciones*.
* MIT Media Lab (2017). *Researchers engineer shape-shifting noodles*. https://www.media.mit.edu
* ResearchAndMarkets.com (2024). *Global Pasta Market Analysis, Size, and Forecasts Report 2024: A \$35+ Billion Industry by 2030*. PR Newswire.
* Severini, C., et al. (2026). New insights into morphing food through a semi-automated system for creating accurate surface grooves of varying depths on cereal-based snacks. *Journal of Food Engineering, 402*, 112700.
* Tao, Y., et al. (2021). Morphing pasta and beyond. *Science Advances, 7*, eabf4098. https://doi.org/10.1126/sciadv.abf4098
* Unión de Industriales Fideeros de la República Argentina (UIFRA). (2020). *Informe Sectorial 2020: Pastas Secas*. https://uifra.org.ar
