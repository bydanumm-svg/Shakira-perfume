# RESUMEN — QSAR (Partes I y II)

> Armado con las diapositivas, tus anotaciones al margen y la clase grabada.
> Las citas en recuadro son textuales del profesor o de tus propias notas.

---

## 1. Qué es QSAR y para qué sirve

**QSAR** = *Quantitative Structure-Activity Relationship*. Correlaciona, de forma **cuantitativa**, datos de estructura química con datos de actividad biológica, para una **serie de compuestos análogos**.

Los dos objetivos: **explicar** y **predecir**.

La cadena lógica que hay que saber recitar:

```
Actividad = f (estructura)
Actividad = f (propiedades fisicoquímicas)
Actividad = f (descriptores moleculares)
```

- La actividad depende de la estructura (si no, nada tendría sentido).
- La estructura determina las propiedades fisicoquímicas.
- Las propiedades hay que **traducirlas a números** → descriptores.

**SAR vs. QSAR**

| | SAR | QSAR |
|---|---|---|
| Vía | Cualitativa | Cuantitativa |
| Tipo | Orientativo | Predictivo |
| Ejemplo | "Al pasar de F a Cl a Br aumenta la actividad" | "La actividad es proporcional al volumen del sustituyente, con coeficiente 0,48" |

⚠️ **Advertencia central de la materia** — correlación ≠ causalidad:

> *"Nosotros vamos a tratar de buscar correlaciones entre propiedades fisicoquímicas y valores de actividad. ¿Existe necesariamente una conexión causal entre dos variables que correlacionan? No, no necesariamente."*

Y la frase de George Box que repitió dos veces:
> *"Todos los modelos están equivocados; la pregunta práctica es cuán equivocados tienen que estar para no ser útiles."*

**Supuesto implícito fundamental:** desde el momento en que metés un set de compuestos en un mismo modelo QSAR, ya estás afirmando que **todos actúan por el mismo mecanismo** y respetan la misma relación estructura-actividad. Si algunos siguen otra regla, el modelo sale mal.

---

## 2. Descriptores moleculares

**Definición (textual, la piden así):**
> Parámetro que caracteriza un aspecto estructural o fisicoquímico específico de una molécula. Una propiedad cualitativa o cuantitativa de una molécula o de una parte de esta.

Tus notas lo resumen bien: *"ponerle números a una propiedad"*. Ejemplo: propiedad = acidez; descriptor del sistema = pH; descriptor **molecular** = pKa.

### Dos clasificaciones cruzadas

**Por origen:**

| | Definición | Ejemplos |
|---|---|---|
| **Experimentales** | Obtenidos por un procedimiento experimental | pKa, logP, μD, σ de Hammett, Es de Taft, MR |
| **Teóricos** | Obtenidos por cálculo computacional | HOMO, LUMO, cargas parciales, Sterimol, TPSA, índices de Fukui |

> *"¿Ustedes a qué le confiarían más, a algo empírico o a algo calculado? La empiria es la que manda, el experimento es el que manda."*

Razón: lo empírico es contrastable directamente. Dos programas calculan HOMO/LUMO para la misma molécula y dan valores distintos.

**Por alcance:**

- **Globales** → describen la molécula entera: logP, pKa, μD, volumen molecular, PM.
- **Locales** → describen una región o sustituyente: π, σ de Hammett, Es de Taft, MR del sustituyente.

### Las tres clases de propiedades

Todo el QSAR clásico se apoya en tres:

| Clase | Qué describe | Descriptores |
|---|---|---|
| **Electrónica** | Distribución electrónica | σ de Hammett, σ* de Taft, pKa, μD, HOMO/LUMO |
| **Estérica** | Forma y volumen | Es de Taft, Sterimol (B1, B5, L), MR, Vm, MSA/PSA |
| **Lipofilicidad** | Afinidad por entorno graso vs. acuoso | logP, π |

---

## 3. Descriptores electrónicos

### 3.1 Constantes σ de Hammett (1935)

Descriptor **electrónico local** que mide el carácter **atractor o dador de electrones** de un sustituyente.

**Reacción modelo:** ionización de ácidos benzoicos.

$$\log \frac{K_X}{K_0} = \rho \cdot \sigma_X \qquad \text{si } \rho = 1: \quad \sigma_X = pK_a(0) - pK_a(X)$$

**La regla del signo (esto se toma siempre):**

| Signo | Significado |
|---|---|
| **σ > 0** | Sustituyente **atractor** de electrones |
| **σ < 0** | Sustituyente **dador** de electrones |
| **σ = 0** | Solo el hidrógeno (es la referencia de la escala) |

> *"Si es más atractor de electrones que el hidrógeno, su signo es positivo. Si es más dador de electrones que el hidrógeno, su signo es negativo."*

La magnitud dice **cuán** atractor o dador.

**Por qué existen σm y σp pero NO σorto:**

En orto, el sustituyente y el grupo carboxilo están uno al lado del otro. Se superponen dos efectos: el que "camina" por el anillo y el efecto directo entre los dos grupos. No se pueden desacoplar y se pierde el comportamiento lineal. Por eso Hammett no tabuló valores de σ orto.

> *"Tengo distorsiones respecto del comportamiento lineal. Entonces por eso Hammett no estableció valores de sigma orto."*

⚠️ σm y σp del mismo sustituyente son **distintos** por defecto. Pueden incluso **cambiar de signo**: el O-fenilo tiene σm = +0,25 (atractor) y σp = −0,03 (dador).

🔑 **Restricción clave:** σ de Hammett **solo se aplica a sistemas aromáticos**. Tus notas: *"SOLO SE APLICA EN AROMATICOS!! SI O SI."*

**σ vs. ρ — no confundir:**

| | Qué es | De qué depende |
|---|---|---|
| **σ** (sigma) | Constante **del sustituyente** | Del sustituyente y su posición |
| **ρ** (rho) | Constante **de la reacción** | Sensibilidad de esa reacción a efectos electrónicos |

El caso que explicó con detalle:

| Serie | ρ |
|---|---|
| Ácidos benzoicos | 1,00 (referencia) |
| Ácidos fenilacéticos (+1 metileno) | 0,49 |
| Ácidos fenilpropiónicos (+2 metilenos) | 0,21 |
| Ácidos cinámicos (doble enlace) | 0,47 |

Cada metileno intercalado aleja y **desconecta electrónicamente** el carboxilo del anillo → cae ρ. Al introducir el doble enlace, el efecto **se recupera parcialmente** porque puede deslocalizarse por el sistema π.

📌 **Relaciones entre esas cuatro estructuras** (lo tomaron en examen): A–B, B–C y A–C son **homología**; A–D es **vinilogía**. C–D y B–D **no** son vinilogía: introducir una insaturación sin agregar carbonos no es vinilogía.

**Desviaciones:** σ⁺ y σ⁻ para casos con fuerte estabilización por resonancia (σ⁻ en ionización de fenoles, σ⁺ en solvólisis de cloruro de cumilo).

### 3.2 Descomposición de Swain y Lupton (1968)

σ puede descomponerse en dos contribuciones:

$$\sigma_X = r_x \cdot \mathcal{R} + f_x \cdot \mathcal{F}$$

- **𝓡 (resonancia)** — camina por el sistema π conjugado.
- **𝓕 (campo)** — tiene dos componentes: polarización a través de enlaces σ (inductivo clásico) + efecto electrostático a través del espacio.

🔑 **𝓡 y 𝓕 están tabulados por sustituyente** (un solo valor cada uno, no hay meta y para). Los que cambian con la posición y la reacción son los coeficientes chiquitos r y f.

**Para qué sirve** (el ejemplo que dio de su doctorado): si la correlación con σ completo es mediocre, probar con 𝓕 solo o 𝓡 solo. A él le subió de R² 0,75 a 0,85 usando 𝓕 — señal de que el efecto era de campo, no de resonancia.

### 3.3 Descriptor σ* de Taft

Es **el equivalente de Hammett para sistemas NO aromáticos** (alquílicos). Se basa en la cinética de hidrólisis de ésteres alquílicos en medio ácido vs. básico.

> Tus notas: *"Cuanto más positivo es el valor de Taft, mayor es el poder atractor de electrones del sustituyente."*

Misma filosofía de signo que Hammett. Comparación útil: el metoxi tiene σp = −0,27 (dador en aromáticos) pero σ* = +1,81 (atractor en alquílicos), porque sin resonancia solo queda el efecto inductivo del oxígeno.

---

## 4. Descriptores estéricos

### 4.1 Es de Taft

Mide el **tamaño relativo** del sustituyente. Se obtiene de la velocidad de hidrólisis **ácida** de ésteres (la hidrólisis ácida es poco sensible a efectos electrónicos, ρ*ac → 0, así que lo que queda es estérico puro).

$$E_{S,X} = \log \left[\frac{k_x}{k_{CH_3}}\right]_{ac}$$

🔑 **Regla del signo:** cuanto **más negativo**, **mayor** el efecto estérico (más voluminoso).

| Sustituyente | Es |
|---|---|
| H | 0 |
| CH₃ | −1,24 |
| iPr | −1,71 |
| tBu | −2,78 |

⚠️ **Trampa de tablas:** la referencia puede ser el H o el **metilo** según la escala, y ahí se invierten los signos. Tus notas: *"No toma como referencia al hidrógeno sino al metilo."* Método seguro: mirar dos sustituyentes de tamaño conocido y deducir hacia dónde crece la escala.

### 4.2 Sterimol (Verloop y Tipker, 1976)

Descriptores **computacionales** basados en radios de van der Waals. Seis vectores, de los cuales importan tres:

- **B1** = radio mínimo
- **B5** = radio máximo
- **L** = longitud máxima

Ventaja: no requiere experimentos cinéticos.

### 4.3 Refractividad molar (MR) — ⚠️ el descriptor problemático

$$MR = \left(\frac{n^2-1}{n^2+1}\right)\frac{PM}{\delta}$$

Desarrollado para cuantificar **polarizabilidad**, se usa como descriptor **estérico** (volumen molar corregido por índice de refracción).

🔑 **El problema — esto se toma:** MR es estérico **pero arrastra un componente electrónico**, porque incluye el índice de refracción. Mezcla dos tipos de propiedad en un solo descriptor.

**Consecuencia práctica:** MR **no puede combinarse en un mismo modelo con otro descriptor estérico**, porque no serían ortogonales. Sí puede combinarse, en principio, con uno de lipofilicidad.

> Tus notas: *"Si un descriptor recoge propiedades distintas en sí mismo, no lo puedo combinar con descriptores que tengan las mismas propiedades."*

### 4.4 MSA, PSA y TPSA

Superficie molecular total (MSA) y superficie **polar** (PSA / TPSA, la versión topológica).

📌 Dato numérico que suelen pedir: **PSA > 90 Å²** → baja penetración a través de membranas biológicas.

---

## 5. Descriptores de lipofilicidad

### 5.1 logP (global)

$$P = \frac{[X]_{\text{fase orgánica (1-octanol)}}}{[X]_{\text{fase acuosa}}} \qquad \log P$$

Históricamente: ampolla de decantación con octanol/agua. Hoy: por HPLC en fase reversa (columna C8, extrapolación de log Kw a 100 % acuoso).

🔑 A **mayor logP, mayor lipofilicidad** (log es función monótona creciente de P).

**Dominio útil:** logP mayor a ~4–5 suele ser problemático: el compuesto se va al tejido graso y nunca llega a la diana.

### 5.2 π de Hansch-Fujita (local)

Contribución de un sustituyente a la lipofilicidad total:

$$\pi_X = \log P_{(A-X)} - \log P_{(A-H)}$$

| Signo | Significado |
|---|---|
| **π > 0** | Sustituyente **lipofílico** (sube el logP) |
| **π < 0** | Sustituyente **hidrofílico** (baja el logP) |
| **π = 0** | Hidrógeno (referencia) |

Ejemplo: π(NO₂) = 1,85 − 2,13 = **−0,28** → el nitro es hidrofílico.

⚠️ Igual que σ, π tiene versión alquílica: **π\*** para sistemas no aromáticos.

### 5.3 🔑 Cómo se calcula realmente (acá está la trampa del examen)

**NO** se suman valores de π desde cero. Se **parte de un logP conocido** y se le suman/restan contribuciones:

$$\log P_{\text{nuevo}} = \log P_{\text{base}} - \pi_{\text{(grupo que sale)}} + \pi_{\text{(grupo que entra)}}$$

> *"No se considera logP como una suma de valores de π, sino que son los valores de π los que se suman sobre un logP base."*

**Ejemplo correcto (prednisolona → 6α-metilprednisolona):**
logP = 1,00 − π(H) + π(CH₃) = 1,00 − 0 + 0,50 = **1,50** ✓ (experimental: 1,50)

**🔑 LA REGLA QUE HAY QUE SABER SÍ O SÍ:**

π_H = 0 **solo cuando el hidrógeno está unido a un carbono aromático.** Si el hidrógeno está sobre un **heteroátomo** (N, O), **no se puede usar esa regla**: hay que **sacar el grupo funcional entero y poner el grupo entero** que lo reemplaza.

> Textual de la diapositiva: *"Dado que solo π(H-C) = 0, en el cálculo se debe considerar la pérdida de la función entera y adición del fragmento completo de la transformación."*

**Ejemplo (anilina → N-metilanilina):**
- ❌ MAL: logP(anilina) − π(H) + π(CH₃)
- ✅ BIEN: logP(anilina) − π(NH₂) + π(NHCH₃)

**Ejemplo (paracetamol → fenacetina):**
logP = 0,41 − π(OH) + π(OCH₂CH₃) = 0,41 − (−0,67) + (−0,02 + 0,50) = **1,56** ✓

📌 Esto es exactamente lo que fallaste en la Pregunta 8d. El corrector escribió *"restar amina"*.

### 5.4 Desvíos y correcciones

El método falla cuando hay **interacciones entre sustituyentes**:

| Caso | Por qué |
|---|---|
| Catecol (logP 0,88) vs. resorcinol (0,80) | Puente de hidrógeno **intramolecular** en orto → más lipofílico |
| 2,6-diisopropilfenol (4,11) vs. 3,5- (3,64) | Los isopropilos **protegen** estéricamente al OH del agua |
| Nitrofenoles (1,93 / 1,91 / 1,79) | Puente de H intramolecular + efecto electrónico sobre la ionización |

**Correcciones tabuladas:**

| Factor | Corrección |
|---|---|
| Doble enlace | −0,09 |
| Triple enlace | −0,50 |
| Ramificación polar | −0,22 |
| Ramificación no polar | −0,13 |

🔑 **La fiabilidad depende de la similitud** entre el compuesto base y el de interés: a mayor similitud, mayor fiabilidad.

---

## 6. Descriptores biológicos

**Afinidad vs. eficacia** (dos etapas de la acción farmacológica):

```
L + R  ⇄  LR  →  Respuesta
      afinidad    eficacia
```

- **Afinidad** → ensayos de unión con ligando radiomarcado.
- **Eficacia** → ensayos de concentración/dosis-respuesta.

| In vitro | Significado |
|---|---|
| Kd, KA, Bmax | Disociación, afinidad, nº de sitios |
| Ki | Constante de inhibición |
| IC₅₀ | Concentración inhibitoria 50 |
| EC₅₀ | Concentración efectiva 50 |
| pD₂ | −log[EC₅₀] |
| pA₂ | −log de la concentración de antagonista que obliga a duplicar la de agonista |
| Emax | Máxima respuesta de un agonista |

| Ex vivo / in vivo |
|---|
| MAD, ID₅₀, ED₅₀, DL₅₀ |

### 🔑 Transformación de la variable dependiente

Nunca se usa el IC₅₀ crudo. Se usa **pIC₅₀ = −log[IC₅₀]**, y **antes de aplicar el logaritmo hay que pasar a unidades MOLARES**.

Si el dato está en nanomolar: dividir por 1×10⁹ y recién ahí aplicar −log. Es la misma lógica que el pH.

⚠️ **Valores no concretos no sirven.** Si un dato dice "MIC > 25", no puede entrar en una regresión lineal: hay que descartarlo. Solo valores concretos.

---

## 7. El modelo QSAR

### Forma general

$$\text{Actividad} = \beta_A A + \beta_B B + \ldots + \beta_N N + \beta_0$$

Donde A, B, …, N son descriptores y las β son los **parámetros de ajuste**.

🔑 **Lo que se ajusta son las β, no las variables.** Las X y la Y son datos conocidos; lo desconocido es el modelo.

**Por qué es "lineal" aunque haya un término al cuadrado:** la regresión lineal toma π² como **una variable en bloque**. No mira el exponente. Por eso siguen siendo regresiones lineales.

**Supuesto:** se considera que los valores de X y de Y **no tienen error**. Se usan valores concretos.

### El golem (la metáfora que usa para el dominio de aplicación)

Un modelo es como un golem: *"robot armado para cumplir una misión, potente pero sin conciencia de límites, peligroso para su uso en automático, no demasiado útil a menos que se sepa controlar."*

Si le pasás un logP de 20, te va a devolver un número. Por eso hay que definir el **dominio de aplicación**: el espacio químico donde el modelo es válido, acotado por los datos con los que se construyó. Usarlo fuera de ese rango es **extrapolar**.

### 🔑 Regla de oro previa a todo

> *"Moraleja: representen en un gráfico cartesiano los datos."*

Siempre se le puede ajustar una recta a cualquier nube de puntos. Si los datos describen una parábola invertida (típico del logP: sube, llega a un óptimo, decae), ajustar una recta no tiene sentido. **Mirar los datos antes de modelar.**

### Homogeneidad de los datos

No se pueden mezclar en una misma columna:
- Valores de actividad de **fuentes distintas** (distintos laboratorios, distintos protocolos).
- Descriptores **experimentales con calculados**.

> *"O son todos calculados o son todos empíricos."*

Sí se pueden combinar **descriptores de distinto tipo** en un modelo (uno electrónico + uno lipofílico), siempre que sean ortogonales.

---

## 8. Diseño de análogos

### 8.1 Diagrama de Craig (1971)

Plano cartesiano donde se distribuyen sustituyentes, con **σp** en un eje y **π** en el otro.

🔑 **Requisito previo:** los ejes deben ser descriptores **ortogonales** (σ es electrónico, π es lipofílico → independientes). Por eso **no** se podría armar con σ y MR.

> ⚠️ *"Que yo vea que en un examen me tracen una línea, un R² ahí en diagrama de Craig… no, porque yo ya tengo que partir del supuesto de que si lo pongo en diagrama de Craig es porque las variables no están correlacionadas."*
>
> El diagrama de Craig **NO** sirve para testear correlación. La ortogonalidad es el requisito, no el resultado.

**Los cuatro cuadrantes:**

| Cuadrante | σp | π |
|---|---|---|
| I | + | − |
| II | + | + |
| III | − | − |
| IV | − | + |

**Las dos etapas de uso (siempre preguntan las dos):**

1. **Diseño de la serie original** — sin saber aún de qué depende la actividad, se elige un sustituyente de **cada cuadrante**. Así se explora el **máximo espacio de propiedades con el mínimo número de compuestos**.
2. **Reenfoque** — una vez obtenido un modelo válido, los **signos de los coeficientes** indican el cuadrante donde se maximiza la actividad, y se vuelve a muestrear concentrándose ahí.

Ejemplo: si el modelo da `Actividad = 0,5·π + 0,7·σp + 1,0`, ambos coeficientes positivos → el óptimo está en el cuadrante con π > 0 **y** σp > 0.

### 8.2 Esquema de Topliss (1972)

Árbol de decisión **secuencial**. Se parte del compuesto con R = H, se reemplaza por Cl en para y se mide:

- Actividad **baja** (L, *less*) → rama de la izquierda
- Actividad **igual** (E, *equal*) → rama del medio
- Actividad **sube** (M, *more*) → rama de la derecha

Y así sucesivamente. Siempre se compara contra el **inmediato anterior**.

**Craig vs. Topliss:**

| | Craig | Topliss |
|---|---|---|
| Estrategia | Sintetiza **toda la serie junta** | Sintetiza **de a uno**, según el resultado anterior |
| Tipo | Visión panorámica del espacio | Camino guiado |
| Uso | El más utilizado | Más económico en síntesis |

---

## 9. Evaluación y selección de modelos ⭐

**Este es el bloque que más se toma.**

### Criterios de aceptación

**Para TODAS las regresiones:**

| Criterio | Umbral |
|---|---|
| **n ≥ 4v** (v = nº de regresores) | soporte empírico |
| **R² ≥ 0,70** | |
| **Prueba t de Student**: p-valor(βᵢ) < 0,05 | para **cada** coeficiente |

**Adicionales para regresiones MÚLTIPLES:**

| Criterio | Umbral |
|---|---|
| **Ortogonalidad**: R²(A vs B) | < 0,3 *(la diapositiva dice 0,50, él lo corrigió a 0,3 en clase)* |
| **Prueba F de Fisher**: p-valor < 0,05 | |
| **R² ajustado ≥ 0,65** | |

$$R^2_{adj} = 1 - \left[\frac{(1-R^2)(n-1)}{n-v-1}\right]$$

### El R² y su trampa

**Qué significa:** la fracción de la varianza de la variable dependiente que es explicada por la independiente. Coloquialmente: qué parte del comportamiento de Y explica X.

🔑 **El R² nunca disminuye al agregar variables.** Sirvan o no. Por eso existe el R² ajustado, que penaliza según el número de variables (y **siempre da menor** que el R²; puede incluso dar negativo).

> *"Hay que creerle al R² cuando te está diciendo que es malo, no cuando es bueno."*

### Student vs. Fisher — la diferencia se toma

| | **t de Student** | **F de Fisher** |
|---|---|---|
| Cuántas pruebas | Una **por cada** coeficiente | **Una sola**, del modelo completo |
| H₀ | βᵢ = 0 | β₁ = β₂ = … = βₙ = 0 (**todos** a la vez) |
| H₁ | βᵢ ≠ 0 | no-H₀ |
| Falla cuando | Ese coeficiente es indistinguible de cero | **Todos** lo son |

En ambos casos: **se rechaza H₀ cuando p-valor < α = 0,05**.

📌 Por eso un modelo puede **pasar Fisher y fallar Student**: basta que una sola variable sirva para que el conjunto no sea "todo cero".

### Intervalos de confianza

Criterio equivalente y más visual: **si el IC 95 % de un coeficiente contiene el cero**, ese coeficiente es estadísticamente **indistinguible de cero**.

> *"No es que se acerque a cero, sino que estadísticamente sea distinguible o indistinguible de cero."*

### 🔑 La regla que define el examen

> *"Si yo tengo un modelo en el cual hay una variable independiente que cumple la condición y otra variable independiente que no cumple la condición… **rechazo el modelo completo**."*

No se elimina la variable mala y se sigue. **Se descarta el modelo entero** y se pasa al siguiente.

### Principio de parsimonia (Navaja de Occam)

Si dos modelos explican **igual de bien** los datos, quedarse con el **más simple**.

⚠️ Importante: *si* el más complejo explica claramente mejor, no se descarta por ser complejo. La parsimonia aplica solo a igualdad de desempeño.

### Orden práctico de evaluación

1. ¿n ≥ 4v? → si no, descarto.
2. ¿R² ≥ 0,70? → si no, descarto.
3. ¿Fisher p < 0,05?
4. ¿**Student p < 0,05 en todos** los coeficientes? → si falla uno, **rechazo el modelo entero**.
5. ¿Algún IC contiene el cero? → confirma lo anterior.
6. ¿Ortogonalidad < 0,3? ¿R² ajustado ≥ 0,65?
7. Entre los que sobreviven: **parsimonia**.

### Interpretación del modelo

El **signo** del coeficiente dice el sentido; la **magnitud**, la importancia.

- Coeficiente **positivo** → la actividad crece al aumentar ese descriptor.
- Coeficiente **negativo** → la actividad crece al **disminuirlo**.
- Coeficiente **cercano a cero** → ese descriptor no aporta.

Y hay que traducir el descriptor a **propiedad**: π o logP → lipofilicidad; σ → efecto electrónico; MR o Es → volumen / impedimento estérico.

---

## 10. Validación

**Objetivo:** establecer la relevancia y confiabilidad del modelo, según especificaciones fijadas **antes** del modelado.

| | **Interna** | **Externa** |
|---|---|---|
| Qué evalúa | **Robustez** | **Predictividad** |
| Cómo | Se parte el set original en *training set* (construcción) y *test set* (evaluación). Se ajusta con uno y se desafía con el otro. Se repite varias veces (**remuestreo**). | Se traen compuestos **nuevos**, nunca vistos por el modelo, de actividad conocida, y se compara predicho vs. experimental. |
| Si falla | El modelo no es robusto: dependía de unos pocos datos | **Sobreajuste** (*over-fitting*): el modelo solo reproduce los datos que ya tenía |

⚠️ Los compuestos de validación externa deben caer **dentro del dominio de aplicación**. Si no, es extrapolar.

---

## 11. Hansch-Fujita vs. Free-Wilson

| | **Hansch-Fujita** | **Free-Wilson (1964)** |
|---|---|---|
| Base | Descriptores fisicoquímicos | Variables **indicadoras** (0 o 1) por sustituyente y posición |
| Forma | Act = βA·A + … + β₀ | log(Act) = Σ Xjk·ajk + μ (μ = actividad media de la serie) |
| **Ventajas** | Predice compuestos nuevos; fácil de aplicar; da información mecanística | No requiere conocer propiedades fisicoquímicas; necesita **pocos** compuestos |
| **Desventajas** | A veces faltan descriptores tabulados; requiere **muchos** compuestos | Muchas variables; **no** explica el porqué fisicoquímico; **no** predice para sustituyentes o posiciones no estudiadas |

Otros métodos mencionados: QSAR 3D (GRID, CoMFA, HQSAR).

---

## 12. Machete final

**Signos — la tabla que resuelve media pregunta:**

| Descriptor | Positivo | Negativo |
|---|---|---|
| σ de Hammett | atractor de e⁻ | dador de e⁻ |
| σ* de Taft | atractor de e⁻ | dador de e⁻ |
| π | lipofílico | hidrofílico |
| **Es de Taft** | — | **más negativo = más voluminoso** |

**Umbrales:**
- n ≥ 4v · R² ≥ 0,70 · R²adj ≥ 0,65 · p < 0,05 (Student y Fisher) · ortogonalidad R² < 0,3 · PSA > 90 Å² = mala permeabilidad

**Restricciones de uso:**
- σ de Hammett → **solo aromáticos** (si no, σ* de Taft)
- MR → estérico **con** componente electrónico, no va con otro estérico
- π_H = 0 → **solo** sobre carbono aromático
- Craig → requiere ejes **ortogonales**

**Cinco frases para el examen:**
1. *"El R² nunca disminuye al agregar variables, por eso no es criterio suficiente."*
2. *"El IC 95 % contiene el cero, luego el coeficiente es indistinguible de cero."*
3. *"Un regresor que no supera el test de Student invalida el modelo completo."*
4. *"Correlación no implica causalidad."*
5. *"A igual desempeño, por parsimonia me quedo con el modelo más simple."*
