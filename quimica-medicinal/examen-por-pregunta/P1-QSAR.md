# PREGUNTA 1 — QSAR

## TEMA 1

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen-tema1_P1-a.jpg)

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen-tema1_P1-b.jpg)

### Respuestas correctas

**a) Seleccione el mejor modelo y justifique en términos comparativos.**

> **El Modelo I.**
>
> El **Modelo II** se descarta por R² = 0,5310, por debajo del umbral de 0,70.
>
> El **Modelo III** se rechaza pese a tener el R² más alto (0,8490): el coeficiente de **π** no supera el test de Student (**p = 0,2208 > 0,05**) y su intervalo de confianza del 95 % **(−0,1564 ; 0,6352) contiene el cero**, por lo que es estadísticamente indistinguible de cero. Como un regresor no cumple el criterio, **se rechaza el modelo completo**. El salto de R² de 0,8363 a 0,8490 es inflación por agregar una variable, no información real.
>
> El **Modelo I** cumple todo: n = 22 ≥ 4v; R² = 0,8363; F de Fisher p = 2,65×10⁻⁹; Student p < 0,05 en ambos coeficientes; ningún IC contiene el cero. Y por **parsimonia**, explica los datos igual de bien con una sola variable.

**b) ¿Qué características debe tener el sustituyente X para maximizar la afinidad?**

> Modelo I: **log RBA = 2,0846 − 0,4843 · MR**
>
> El coeficiente de **MR** es **negativo**, de modo que la afinidad se maximiza **minimizando MR**: sustituyentes **pequeños, poco voluminosos y poco polarizables** en la posición 16α.
>
> Los datos lo confirman: −H (MR 0,10) da log RBA 2,00, mientras que los sustituyentes voluminosos con NBD (MR 5,80–6,07) caen a log RBA negativos.

**c) Indique al menos dos descriptores del mismo tipo de propiedad fisicoquímica que el del modelo seleccionado, señalando si son teóricos o experimentales.**

> MR es un descriptor **ESTÉRICO**. Otros del mismo tipo:
>
> | Descriptor | Tipo |
> |---|---|
> | **Es de Taft** | **Experimental** (cinética de hidrólisis ácida de ésteres) |
> | **Sterimol** (L, B1–B5) | **Teórico** (computacional, radios de van der Waals) |
> | Volumen molecular | Teórico |
> | MSA / TPSA | Teórico |
>
> ⚠️ Conviene agregar: **MR es estérico pero arrastra un componente electrónico** (interviene el índice de refracción, ligado a la polarizabilidad). Por eso **no puede combinarse con otro descriptor estérico** en el mismo modelo: no serían ortogonales.

## TEMA 2

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen_P1-a.jpg)

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen_P1-b.jpg)

### Respuestas correctas

**a)** Idéntica a la del Tema 1: **Modelo I**, por el p-valor de Student de π y su intervalo de confianza.

**b) Si usaron un esquema de Craig, ¿en qué etapa del proceso lo habrán hecho?**

> En la etapa de **diseño de la serie de análogos, ANTES de sintetizarlos y medir su actividad**.
>
> El diagrama de Craig distribuye sustituyentes en un plano cartesiano con **σp** (electrónico) y **π** (lipofílico), que son **descriptores ortogonales**. Tiene **dos etapas de uso**:
>
> 1. **Diseño de la serie original:** sin saber todavía de qué depende la actividad, se elige un sustituyente de **cada uno de los cuatro cuadrantes**, para barrer el máximo espacio de propiedades con el mínimo número de compuestos.
> 2. **Reenfoque:** una vez obtenido un modelo válido, los **signos de los coeficientes** indican el cuadrante donde se maximiza la actividad y se vuelve a muestrear ahí.
>
> ⚠️ El diagrama de Craig **no** sirve para testear correlación: que los ejes sean ortogonales es el **requisito previo** para poder armarlo.

**c) ¿Qué propiedad fisicoquímica permite maximizar la afinidad?**

> El **volumen / impedimento estérico** del sustituyente, descripto por **MR**. Como su coeficiente es negativo, la afinidad se maximiza con sustituyentes de **baja refractividad molar**, es decir pequeños y poco polarizables.

### 🔑 Checklist de evaluación de modelos (sirve para las dos versiones)

| # | Criterio | Umbral |
|---|---|---|
| 1 | n ≥ 4 × nº de variables | soporte empírico |
| 2 | R² | ≥ 0,70 |
| 3 | Test **F de Fisher** (modelo global) | p < 0,05 |
| 4 | Test **t de Student**, **cada** coeficiente | p < 0,05 |
| 5 | **IC 95 %**: ninguno contiene el cero | — |
| 6 | Ortogonalidad (si hay ≥2 descriptores) | R² < 0,3 |
| 7 | R² ajustado (si hay ≥2) | ≥ 0,65 |
| 8 | **Parsimonia**: a igual desempeño, el más simple | — |

> **Si un solo regresor falla el test de Student, se rechaza el modelo completo.**

---
