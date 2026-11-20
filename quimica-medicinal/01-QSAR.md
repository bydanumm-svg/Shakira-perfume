# TEMA 1 — QSAR / Hansch (Pregunta 1)

**Tu nota: 2,5 / 10** — el peor puntaje del examen. También es el tema más mecánico: son 8 criterios que se aplican siempre igual.

---

## 1. Qué te tomaron

22 análogos de estradiol sustituidos en 16α. Para cada uno: log RBA (afinidad relativa por el receptor de estrógenos), MR (refractividad molar) y π (lipofilicidad del sustituyente). Con esos datos, tres modelos de regresión lineal:

| Modelo | Descriptores | R² | s | p (F-Fisher) |
|---|---|---|---|---|
| **I** | MR | 0,8363 | 0,4311 | 2,65×10⁻⁹ |
| **II** | π | 0,5310 | 0,7296 | 1,20×10⁻⁴ |
| **III** | MR + π | 0,8490 | 0,4247 | 1,59×10⁻⁸ |

Coeficientes del Modelo III:

| | Coef. | p (Student) | IC 95% |
|---|---|---|---|
| Intercepto | 2,0832 | 2,98×10⁻¹² | (1,8024 – 2,3639) |
| MR | −0,5850 | 4,53×10⁻⁶ | (−0,7785 – −0,3914) |
| **π** | **0,2394** | **0,2208** | **(−0,1564 – 0,6352)** ⚠️ |

**a)** Seleccione el mejor modelo y justifique en términos comparativos.
**b)** Si usaron un esquema de Craig, ¿en qué etapa del proceso lo habrán hecho?
**c)** ¿Qué propiedad fisicoquímica permite maximizar la afinidad?

---

## 2. Qué pusiste y por qué está mal

### a) Elegiste el Modelo III ❌

Tu argumento: *"el R² del modelo III es mayor y eso ayuda a tener más linealidad y menor dispersión de datos."*

**El problema:** usaste el R² como criterio decisivo. El R² **nunca baja** cuando agregás una variable, sirva o no sirva. Por eso un R² más alto no prueba que el modelo sea mejor.

Mirá los dos números que ignoraste, en la fila de π del Modelo III:
- **p = 0,2208**, muy por encima de α = 0,05 → el coeficiente **no** es significativo.
- **IC 95% = (−0,1564 ; 0,6352)** → **contiene el cero**.

Que el intervalo contenga el cero significa que ese coeficiente es estadísticamente **indistinguible de cero**. Y si vale cero, el término π directamente no existe en el modelo.

> 🔑 **Regla textual de la cátedra:** *"Si yo tengo un modelo en el cual hay una variable independiente que cumple la condición y otra variable independiente que no cumple la condición... rechazo el modelo completo."*

No se "elimina π y se sigue". **Se rechaza el Modelo III entero.**

Por eso el corrector te escribió al margen algo sobre el intervalo de confianza del Modelo III: era el dato que resolvía la pregunta.

### b) Craig — bien encaminada, incompleta ⚠️

Dijiste que se usa al principio, para elegir compuestos disímiles de los cuatro cuadrantes. **Eso está bien** y por eso te dieron parte del puntaje. Lo que faltó: Craig tiene **dos** etapas de uso.

### c) En blanco ❌

Se contestaba leyendo el signo del coeficiente del modelo correcto. Dos renglones.

---

## 3. Cómo había que encararlo

### El checklist (este es el corazón del tema)

Aplicalo **en este orden**, siempre:

| # | Criterio | Umbral |
|---|---|---|
| 1 | n ≥ 4 × (nº de variables independientes) | soporte empírico |
| 2 | R² | ≥ 0,70 |
| 3 | Test **F de Fisher** (modelo global) | p < 0,05 |
| 4 | Test **t de Student**, **cada** coeficiente | p < 0,05 |
| 5 | **IC 95%**, ninguno contiene el cero | — |
| 6 | Ortogonalidad entre descriptores *(si hay ≥2)* | R² entre ellos < 0,3 |
| 7 | R² ajustado *(si hay ≥2)* | ≥ 0,65 |
| 8 | **Parsimonia**: a igual desempeño, el más simple | — |

**Diferencia Fisher vs. Student** (esto lo preguntan):
- **Fisher**: una sola prueba, evalúa el modelo completo. H₀ = *todos* los coeficientes son indistinguibles de cero simultáneamente. Falla solo si fallan todos.
- **Student**: una prueba por cada coeficiente. H₀ = *ese* coeficiente vale cero.

Por eso el Modelo III **pasa Fisher pero falla Student en π**: MR solo ya alcanza para que el conjunto no sea todo cero.

### Respuesta a)

> **Elijo el Modelo I.**
>
> El **Modelo II** se descarta: R² = 0,5310, por debajo del umbral de 0,70.
>
> El **Modelo III** se rechaza pese a tener el R² más alto (0,8490). El coeficiente de π no supera el test de Student (p = 0,2208 > 0,05) y su intervalo de confianza del 95% (−0,1564 ; 0,6352) incluye el cero, por lo que es estadísticamente indistinguible de cero. Como uno de los regresores no cumple el criterio, se rechaza el modelo completo. El R² apenas sube de 0,8363 a 0,8490: esa diferencia es inflación por agregar una variable, no información real.
>
> El **Modelo I** cumple todo: n = 22 ≥ 4; R² = 0,8363 ≥ 0,70; F de Fisher p = 2,65×10⁻⁹ < 0,05; Student p = 2,65×10⁻⁹ para MR y 1,64×10⁻¹² para el intercepto, ambos < 0,05; ningún IC contiene el cero. Además, por parsimonia, explica los datos igual de bien con una sola variable.

### Respuesta b)

> En la **etapa de diseño de la serie de análogos, antes de sintetizarlos y medir su actividad**.
>
> El diagrama de Craig distribuye los sustituyentes en un plano cartesiano cuyos ejes son σp (electrónico) y π (lipofílico), **descriptores ortogonales entre sí**. Se usa en dos momentos:
>
> 1. **Diseño de la serie original:** sin saber todavía de qué depende la actividad, se elige un sustituyente de cada uno de los cuatro cuadrantes. Así se barre el máximo espacio de propiedades fisicoquímicas con el mínimo número de compuestos sintetizados.
> 2. **Reenfoque:** una vez obtenido un modelo válido, los signos de los coeficientes indican hacia qué cuadrante se maximiza la actividad, y se vuelve a muestrear concentrándose ahí.

⚠️ **Trampa frecuente:** el diagrama de Craig **no** sirve para averiguar si dos variables están correlacionadas. Al revés: que sean ortogonales es el **requisito previo** para poder armarlo. Textual del profesor: *"Que yo vea que en un examen me tracen una línea, un R² ahí en diagrama de Craig... no, porque yo ya tengo que partir del supuesto de que si lo pongo en diagrama de Craig es porque las variables no están correlacionadas."*

### Respuesta c)

> El Modelo I es: **log RBA = 2,0846 − 0,4843 · MR**
>
> El único descriptor significativo es **MR (refractividad molar)**, un descriptor **estérico** (volumen/polarizabilidad del sustituyente). Su coeficiente es **negativo**, de modo que la afinidad se maximiza **minimizando MR**: sustituyentes pequeños y poco voluminosos en la posición 16α.

Los datos lo confirman: −H (MR 0,10) da log RBA 2,00, y los sustituyentes voluminosos con NBD (MR 5,80–6,07) caen a log RBA negativos.

⚠️ **Cuidado con MR:** es estérico, pero **arrastra un componente electrónico** (entra el índice de refracción, ligado a la polarizabilidad). Por eso no puede combinarse en un mismo modelo con otro descriptor estérico: no serían ortogonales.

---

## 4. Cómo te lo pueden volver a tomar

Las variantes son casi siempre estas:

1. **Mismo formato, otros números.** Buscá primero la columna de p-valores de Student y los IC. Ahí está la respuesta, no en el R².
2. **Que todos los modelos pasen Student.** Ahí decide la **parsimonia**: el más simple. Pero ojo, parsimonia solo aplica *a igual desempeño*; si el más complejo explica claramente mejor, se queda el complejo.
3. **Pedir la ortogonalidad.** Respuesta: regresión de un descriptor contra el otro; si R² < 0,3, son ortogonales y pueden ir juntos.
4. **R² ajustado.** Siempre menor que el R². Corrige la inflación por número de variables. Es el que hay que comparar entre modelos con distinto número de variables.
5. **Validación.** Interna (remuestreo: partir el set en construcción + evaluación) vs. externa (compuestos nuevos, nunca vistos por el modelo). Si falla → **overfitting**.
6. **Dominio de aplicación.** No se puede extrapolar fuera del rango de los datos que calibraron el modelo.
7. **Coeficiente con signo positivo.** Entonces la actividad se maximiza *aumentando* ese descriptor. Y hay que nombrar la propiedad, no solo el descriptor: π/logP → lipofilicidad; σ → efecto electrónico; MR/Es → volumen o impedimento estérico.

### Frases para tener listas

- *"El R² nunca disminuye al agregar variables, por eso no es criterio suficiente de selección."*
- *"El IC 95% contiene el cero, por lo tanto el coeficiente es indistinguible de cero."*
- *"Un regresor que no supera el test de Student invalida el modelo completo."*
- *"Correlación no implica causalidad."*
