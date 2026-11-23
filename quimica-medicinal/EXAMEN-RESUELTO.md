---
---

# Examen resuelto — Temas 1 y 2

Cada pregunta aparece con **las dos versiones del examen** (Tema 1 y Tema 2), la foto original y debajo la respuesta correcta.

Los datos y las estructuras son casi siempre los mismos entre versiones; **lo que cambia son las consignas**. Por eso conviene estudiar las dos: en el recuperatorio puede tocarte cualquiera, o una combinación.

| Pregunta | Tema 1 | Tema 2 |
|---|---|---|
| 1 — QSAR | 📷 foto | 📷 foto |
| 2 — Adrenérgicos | 📄 transcripta | 📷 foto |
| 5 — Anti-H2 | 📄 transcripta | 📷 foto |
| 6 — Tricíclicos | 📄 transcripta | 📷 foto |
| 7 — Serotoninérgicos | 📷 foto | 📷 foto |
| 8 — Metabolismo y logP | 📷 foto | 📷 foto |

> Tres preguntas del Tema 1 aparecen con la **consigna transcripta** en lugar de la foto, porque esas imágenes no pudieron guardarse en el servidor. El contenido y las respuestas están completos igual.

---

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

# PREGUNTA 2 — Adrenérgicos

## TEMA 1

> 📄 *Consigna transcripta (la foto no pudo guardarse en el servidor).*

**a. Dados los siguientes fármacos complete el cuadro** (columnas: *Estructura química / Familia química / Utilidad terapéutica*):

- **A** — anillo aromático unido por **oxígeno** a −CH₂−CH(OH)−CH₂−NH−isopropilo, con un **éster metílico** (−CH₂CH₂−COOCH₃) en *para*
- **B** — fenol (HO−) con cadena −CH₂−CH(CH₃)−NH₂
- **C** — dos anillos aromáticos sobre un mismo nitrógeno, puente de **2 carbonos** y dimetilamino terminal. *(La utilidad terapéutica venía impresa: "Tratamiento del asma".)*

**b.** Indique sobre la estructura de **A** la/s zona/s que determina/n selectividad por el subtipo de receptor.
**c.** Indique sobre la estructura de **A** la presencia de carbonos quirales y la configuración necesaria para que el fármaco sea activo.
**d.** Dibuje los productos metabólicos de una reacción de fase 1 sobre el compuesto **C**, indicando la reacción y si se altera el perfil de actividad.

### Respuestas correctas

**a) Cuadro**

| | Compuesto | Familia química | Utilidad terapéutica |
|---|---|---|---|
| **A** | **Esmolol** | **Ariloxipropanolamina** | **Arritmias** e hipertensión perioperatoria. β-bloqueante **cardioselectivo (β1)** de acción **ultracorta** |
| **B** | **Hidroxianfetamina** | **Ariletilamina** | **Descongestivo nasal** / midriático |
| **C** | Antihistamínico H1 | **Etilendiamina** | *(venía dada)* |

📌 **Sobre el esmolol:** el éster es la clave. Las **esterasas** lo hidrolizan rápidamente a un **metabolito inactivo**, y de ahí su acción ultracorta — por eso se usa por vía intravenosa en situaciones perioperatorias.

⚠️ **Error a no repetir:** en A escribiste "ariloxipropanolamina" (correcto) y después agregaste "éter de alquilamino"; en B escribiste "ariletilamina" (correcto) y agregaste "propilamina". **La segunda respuesta anula la primera.** Si ya pusiste la buena, no agregues otra.

⚠️ La columna de **utilidad terapéutica** quedó en blanco en A y B. Son dos casillas que se contestaban en tres palabras.

**b) Zonas de A que dan selectividad**

> 1. **El sustituyente sobre el nitrógeno**: el **isopropilo** orienta hacia receptores β.
> 2. **El sustituyente aceptor de puente de hidrógeno en *para*** del anillo (acá el éster) → **cardioselectividad β1**. Si ese mismo grupo estuviera en *meta*, se perdería la selectividad.

**c) Carbonos quirales y configuración**

> **Un solo carbono quiral**: el que lleva el **OH** de la cadena propanolamínica.
>
> Para las **ariloxipropanolaminas** el enantiómero activo es el **S**.
>
> ⚠️ Pero ojo con la explicación: **no se unen distinto al receptor que las ariletanolaminas (que son R)**. Es la misma disposición espacial; al insertar el oxígeno cambian las **prioridades CIP** y por eso cambia la letra.

**d) Reacción de fase 1 sobre C**

> **Reacción: N-desalquilación oxidativa** (CYP450) sobre el dimetilamino terminal.
>
> **Productos:** el compuesto con amina **secundaria** (−NH−CH₃) + **formaldehído** (HCOH).
>
> **¿Se altera el perfil de actividad? SÍ.** La REA de los antihistamínicos H1 exige **sustituyentes pequeños sobre el nitrógeno**, pero también que la amina conserve su basicidad para la interacción iónica. Al desmetilarse cambia el patrón de sustitución del nitrógeno y **disminuye la potencia antihistamínica**.

> ℹ️ *La estructura de C no se lee con total nitidez en la foto. El esqueleto corresponde a las **etilendiaminas** (dos arilos sobre un N, puente de 2 carbonos, amina terciaria), pero conviene que verifiques esa casilla contra tu copia del examen.*

## TEMA 2

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen_P2.jpg)

### Respuestas correctas

**a) Cuadro**

| | Compuesto | Familia química | Utilidad terapéutica |
|---|---|---|---|
| **A** | **Soterenol** | **Ariletanolamina** | **Asma** y EPOC (broncodilatador) |
| **B** | **Pindolol** | **Ariloxipropanolamina** | **Hipertensión**, arritmias, angina |
| **C** | — | **Ariletilamina** | **Descongestivo nasal** |

⚠️ **No es "ariletilamina" para A ni "ariloxipropilamina" para B.** El sufijo indica el grupo funcional:

- **Ariletil**amina → sin OH bencílico (adrenérgico **indirecto**)
- **Ariletanol**amina → **con** OH bencílico (agonista directo)
- **Ariloxipropanol**amina → oxígeno puente **y** OH (antagonista)

⚠️ Y no mezclar columnas: *"agonista β2 selectivo"* es el **mecanismo**, no la utilidad terapéutica.

**b) Zona/s de A que determinan la selectividad por el subtipo de receptor**

> **Dos zonas:**
>
> 1. **El sustituyente sobre el nitrógeno.** H o CH₃ → α1; **isopropilo → β**; terc-butilo → β2. En A hay un isopropilo.
> 2. **El grupo voluminoso y polar en posición 3 del anillo** — en A, la **metanosulfonamida**, que reemplaza a uno de los OH del catecol. Es la que confiere selectividad **β2** conservando la capacidad de formar puentes de hidrógeno.
>
> Ventaja extra: al no ser ya un catecol auténtico, deja de ser sustrato de **COMT** → mayor duración de acción.

**c) Carbonos quirales y configuración activa**

> **Un solo carbono quiral**: el **bencílico** que lleva el OH. La configuración activa es **R**, igual que en la noradrenalina natural.
>
> Solo en R quedan orientados simultáneamente los tres puntos de unión: enlace **iónico** del amino con Asp-113, **puente de hidrógeno** del OH, e interacciones del **anillo**. En el enantiómero S se pierde el puente de hidrógeno.

| Familia | Enantiómero activo |
|---|---|
| Ariletanolaminas | **R** |
| Ariloxipropanolaminas | **S** |

> Y si preguntan si eso significa que se unen distinto: **NO**. Es la misma disposición espacial; al insertar el oxígeno cambia la **prioridad CIP**.

**d) Productos de una reacción de fase 1 sobre A**

> **Reacción: N-desalquilación oxidativa** (CYP450).
>
> **Productos:** el compuesto con amina **primaria** (−NH₂) + **acetona** (CH₃−CO−CH₃).
>
> **¿Se altera el perfil de actividad? SÍ.** El isopropilo era uno de los dos elementos que daban selectividad β. Al perderlo, la amina primaria orienta hacia **α1**: el metabolito pierde la selectividad β2 y la utilidad como broncodilatador.

🔑 En la N-desalquilación el fragmento que se va sale como **carbonilo**: isopropilo → **acetona**; metilo → **formaldehído**; etilo → acetaldehído.

---

# PREGUNTA 5 — Antagonistas H2

## TEMA 1

> 📄 *Consigna transcripta (la foto no pudo guardarse en el servidor).*

**Enunciado:** *En la ruta del desarrollo de la cimetidina (Tagamet®), el equipo liderado por James Black llegó al compuesto "burimamida" (SKF 91923). Si bien este compuesto se comportaba como antagonista del receptor H₂, su potencia era insuficiente. Por este motivo se diseñó una serie de análogos entre los cuales estaban los compuestos "tioburimamida" y "oxoburimamida". Luego, la optimización de la tioburimamida permitió llegar al compuesto denominado "metiamida" (SKF 92058), un importante precursor de la cimetidina (SKF 92334).*

*Se muestran las cuatro estructuras: **burimamida** (cadena de 4 carbonos), **tioburimamida** (con −S− intercalado), **oxoburimamida** (con −O− intercalado) y **metiamida** (tioburimamida + CH₃ en posición 4 del imidazol).*

**a)** Indique qué tipo de relación farmacomodulativa vincula a la burimamida con la oxaburimamida y la tioburimamida.
**b)** Proponga una explicación a la relación de potencias **burimamida < tioburimamida < metiamida**, en tanto inhibidores de la secreción ácida gástrica.
**c)** Supongamos que reemplazamos el grupo **CH₃** unido al anillo imidazólico de la metiamida por un grupo **NO₂**. ¿Qué consecuencia esperaría respecto a la actividad del nuevo análogo respecto a su precursor inmediato?

### Respuestas correctas

**a)**

> **Bioisosterismo CLÁSICO.** Se reemplaza un **−CH₂−** de la cadena por **−S−** (tioburimamida) o por **−O−** (oxaburimamida). Son **isósteros divalentes**, intercambiables según la ley de desplazamiento de hidruros de Grimm. El mismo criterio vincula la tioburimamida con la oxaburimamida entre sí (−S− por −O−).

**b)**

> La potencia crece porque en cada paso el **pKa del anillo imidazólico se acerca al de la histamina (5,8)**, es decir, disminuye la fracción ionizada a pH fisiológico:
>
> | Compuesto | pKa | Por qué |
> |---|---|---|
> | **Burimamida** | 7,25 | Su cadena lateral es **dadora de electrones**, lo que aumenta la basicidad del imidazol. 40 % ionizado |
> | **Tioburimamida** | **6,25** | El **azufre** insertado es **atractor por efecto inductivo** → baja el pKa |
> | **Metiamida** | 6,80 | El **CH₃ en posición 4** es **dador**, está **cerca de Nτ y lejos de Nπ** → aumenta selectivamente la basicidad de **Nτ** y favorece el tautómero que imita a la histamina |
>
> 🔑 En la metiamida el pKa sube un poco respecto de la tioburimamida, pero **el efecto positivo del exceso de tautómero Nτ supera al efecto negativo del aumento de ionización**: la potencia es 10× la de la burimamida.

**c)**

> **La actividad DISMINUIRÍA** respecto de la metiamida.
>
> El **NO₂** es un grupo fuertemente **ATRACTOR** de electrones, exactamente lo opuesto al CH₃, que es dador. Se perdería el **aumento selectivo de basicidad de Nτ** que lograba el metilo, y el equilibrio tautomérico se desplazaría hacia el tautómero **Nπ-H**, que **no** es el que reconoce el receptor H2. Al dejar de imitar la forma tautomérica preferida de la histamina, cae la afinidad.

## TEMA 2

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen_P5.jpg)

### Respuestas correctas

**a) ¿Qué relación farmacomodulativa vincula metiamida → cimetidina → ranitidina, considerando las regiones punteadas? Justifique con argumentos fisicoquímicos.**

> **BIOISOSTERISMO NO CLÁSICO** (isosterismo de grupos funcionales): el grupo **tiourea** de la metiamida fue reemplazado por **cianoguanidina** (cimetidina) y por **nitroetendiamina** (ranitidina).
>
> **Argumentos fisicoquímicos** — los tres grupos comparten:
>
> | Propiedad | Por qué importa |
> |---|---|
> | **Planaridad** | Permite la misma orientación en el sitio de unión |
> | **Tamaño similar** | Ocupan aproximadamente el mismo volumen |
> | **Capacidad de formar dos puentes de hidrógeno simultáneos** | Es el requisito de la interacción con H2 |
> | **Carácter NO básico (pKa muy bajo)** | No se protonan a pH fisiológico |
> | **Momento dipolar adecuado** (magnitud **y orientación**) | Es el descriptor del modelo QSAR final |
>
> 🔑 Lo determinante: **las interacciones electrostáticas favorecen el agonismo; los puentes de hidrógeno favorecen el antagonismo.** Por eso los grupos deben ser no básicos, y por eso hubo que incorporar atractores fuertes (−CN, −NO₂) que bajan el pKa de la guanidina de 13 a ~0,4–0,9.

📌 pKa de los grupos: tiourea −1,2 · N-nitroguanidina 0,9 · **N-cianoguanidina 0,4** · guanidina sin sustituir 13.

**b) ¿Qué consecuencia sobre la actividad se espera al reemplazar el cianoguanidino por una N-metilurea? ¿A qué se debería?**

> **La potencia como antagonista H2 DISMINUYE.**
>
> **Causa: solvatación.** El grupo N-metilurea es bastante más **polar e hidrofílico** que el cianoguanidino, de modo que tiene **menor logP**. Según la REA establecida para esta familia:
>
> $$\log(\text{actividad}) = 2{,}0 \log P + 7{,}4$$
>
> es decir, **la actividad aumenta con el logP**. El razonamiento: *a mayor polaridad e hidrofilia, más fácil la solvatación en agua y más difícil la desolvatación*. Para cumplir su función el extremo polar debe establecer **dos puentes de hidrógeno simultáneos** con el receptor, y para eso primero tiene que **desolvatarse**. Si está muy solvatado, el costo energético es alto y queda **menos disponible para el acoplamiento**.
>
> 📌 El mismo razonamiento explica por qué el análogo con **oxígeno** (oxaburimamida) fue menos potente que el de azufre.

⚠️ **Error a no repetir:** acá no va el argumento del pKa ni el de la toxicidad. El pKa corresponde a la optimización del **anillo imidazólico**, y la toxicidad al reemplazo de la **tiourea**. Esta pregunta es sobre el **extremo polar** y se contesta con **solvatación y logP**.

---

# PREGUNTA 6 — Tricíclicos y topología

## TEMA 1

> 📄 *Consigna transcripta (la foto no pudo guardarse en el servidor).*

**1) Dada la transformación del compuesto A a la estructura B:**

- **A** — **fenotiazina** (anillo central de 6 miembros con S y N) con **F** en el anillo y cadena de **3 carbonos** terminada en dimetilamino
- **B** — sistema tricíclico con un anillo de **piridina** y uno de **tiofeno**, anillo central de **7 miembros**, **F**, y cadena de 3 carbonos terminada en **piperazina**

**a)** Complete la tabla: *Mecanismo de acción farmacológica / Topología (ángulos α, β y γ) / Aplicación clínica*, para A y B.
**b)** Familia química a la que corresponde el compuesto **A**.
**c)** Dibuje un **isómero de cadena** del compuesto A que resulta en un compuesto con otra aplicación clínica. ¿Cuál es esta?
**d)** Señale al menos **tres estrategias de farmacomodulación** que conceptualicen la obtención de B a partir de A.

**2) Dibuje un profármaco BIOPRECURSOR de la dopamina.**

### Respuestas correctas

**a) Cuadro**

| | A | B |
|---|---|---|
| **Mecanismo de acción** | Antagonista de receptores **D2** | **Inhibidor de la recaptación** de NA y 5-HT |
| **Topología (α, β, γ)** | **55°, 0°, 0°** | **50°, 30°, 20°** |
| **Aplicación clínica** | **Esquizofrenia**, psicosis aguda | **Depresión** |

⚠️ **"Neuroléptico" y "antidepresivo" NO son aplicaciones clínicas**, son las acciones. La aplicación clínica es la **enfermedad**.

**b) Familia de A:** **FENOTIAZINA** (no "dibenzofenotiazina").

**c) Isómero de cadena de A con otra aplicación clínica**

> 🔑 **Isómero de cadena ≠ homólogo.** Un isómero de cadena **conserva la fórmula molecular** y solo cambia la ramificación. Acortar la cadena de 3 C a 2 C es **homología**, y cambia la fórmula.
>
> Para una fenotiazina con cadena **lineal** −CH₂−CH₂−CH₂−N(CH₃)₂, el isómero de cadena es la **cadena ramificada** −CH₂−CH(CH₃)−N(CH₃)₂, es decir el esqueleto de la **prometazina**.
>
> **Aplicación clínica resultante: antialérgico** (antihistamínico H1).

**d) Tres estrategias de farmacomodulación A → B**

> 1. **Ampliación de anillo**: el anillo central pasa de **6 a 7 miembros**.
> 2. **Reemplazo por anillos equivalentes / bioisosterismo de anillos**: un benceno por **piridina** y el otro por **tiofeno**.
> 3. **Formación de anillo (ciclación)** sobre la amina: la dimetilamina se convierte en **piperazina**.

**2) Profármaco BIOPRECURSOR de la dopamina**

> ⚠️ **Bioprecursor ≠ profármaco con grupo transportador.** Dibujar los ésteres del catecol está **mal**, porque esos son grupos transportadores que se liberan por **hidrólisis**.
>
> Un **bioprecursor** necesita un proceso **REDOX** para activarse. Entonces va:
> - el **catecol LIBRE** (sin esterificar)
> - la dopamina unida por **amida** a un sistema de **dihidropiridina** (derivado del ácido trigonélico reducido)
>
> Al entrar al SNC, una **óxido-reductasa** (NADP⁺) oxida la dihidropiridina a **sal de piridinio** → carga fija → queda atrapada; después se hidroliza la amida y se libera dopamina.

## TEMA 2

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen_P6.jpg)

### Respuestas correctas

**a) Cuadro**

| | A | B |
|---|---|---|
| **Mecanismo de acción** | Antagonista de receptores **D2** | **Inhibidor no selectivo de la recaptación** de NA y 5-HT |
| **Topología (α, β, γ)** | **55°, 0°, 0°** | **50°, 30°, 20°** |
| **Aplicación clínica** | **Esquizofrenia**, psicosis aguda | **Depresión** |

**b) Familia química de A:** **TIOXANTENO** (no fenotiazina).

🔑 La diferencia está en **un solo átomo** del anillo central: si la cadena sale de un **N** por enlace simple → fenotiazina. Si hay un **doble enlace exocíclico** (grupo metilideno) hacia la cadena → **tioxanteno**.

**c) Derivado de la misma familia de A con otro mecanismo de acción principal**

> Un **tioxanteno con cadena puente de 2 carbonos** (y sin el sustituyente atractor en posición 2) → **antihistamínico H1**.
>
> Es la misma lógica que prometazina vs. clorpromazina: dentro de una misma familia tricíclica, **2 carbonos → antihistamínico; 3 carbonos → neuroléptico**.

**d) Tres estrategias de farmacomodulación A → B**

> 1. **Ampliación de anillo**: anillo central de **6 a 7 miembros**.
>    ⚠️ **No es "equivalente anular S × CH₂".** La equivalencia anular es reemplazar **un anillo por otro** (benceno → piridina).
> 2. **Reemplazo por anillos equivalentes**: un benceno por **piridina**.
> 3. **Bioisosterismo clásico**: **H → F** (isóstero monovalente).
> 4. *(alternativa)* **Formación de anillo**: N-metilpiperidina → **piperazina**.

**e) Profármaco MIXTO de la dopamina**

> **Dos grupos impiden el pasaje de la BHE:** el **catecol** (polar) y el **amino** (se protona → carga).
>
> **Doble latentización (método de Bodor):**
> 1. **Esterificar los dos OH del catecol** (pivaloilo) → enmascara la polaridad
> 2. **Amidar el amino** con un derivado de **dihidropiridina** → impide la protonación
>
> **Activación en el SNC:**
> 3. Una **óxido-reductasa** oxida la dihidropiridina a **piridinio** → carga fija → atrapamiento
> 4. Las **esterasas** recuperan el catecol
> 5. La hidrólisis de la amida libera **dopamina** + metabolito no tóxico
>
> 🔑 **Por qué es MIXTO:** combina los dos tipos de profármaco — **grupo transportador** (ésteres y amida, por hidrólisis) + **bioprecursor** (dihidropiridina, por redox). Si dibujás solo los ésteres, es un profármaco **común**, no mixto.

### 🎯 La tabla de topología (sirve para las dos versiones)

| Sistema | α | β | γ | Actividad |
|---|---|---|---|---|
| **Fenotiazina / Tioxanteno** | 55° | **0°** | **0°** | **Neuroléptico** |
| **Dibenzociclohepteno** (insaturado) | 50° | 30° | **0°** | Antidepresivo **y** neuroléptico |
| **Dibenzoazepina** | 50° | 30° | **20°** | **Antidepresivo** |

|  | **γ = 0°** | **γ ≠ 0°** |
|---|---|---|
| **Cadena 2 C** | Antihistamínicos / anticolinérgicos | — |
| **Cadena 3 C** | **Neurolépticos** | **ANTIDEPRESIVOS** |

---

# PREGUNTA 7 — Serotoninérgicos

## TEMA 1

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen-tema1_P7.jpg)

### Respuestas correctas

**1) Compuesto dado: NARATRIPTÁN** (indol + sulfonamida en 5 + piperidina N-metilada en 3)

> **a) Grupos ionizables a pH 7,40:** la **amina terciaria** del anillo de piperidina (se protona a pH fisiológico). La sulfonamida secundaria y el NH del indol no se ionizan a ese pH.
>
> **b) Blanco farmacológico:** receptores **5-HT₁B/1D** (agonista).
>
> **c) Aplicación clínica:** **MIGRAÑA** (antimigrañoso). ⚠️ No es antidepresivo.
>
> **d) Se desarrolló a partir de la farmacomodulación de la SEROTONINA**, por diseño racional:
>
> ```
> 5-HT → 5-carboxamidotriptamina (no selectivo)
>      → N-metilcarboxamidometilo (selectivo, no oral)
>      → N-metilsulfamoilmetilo (selectivo, oxidación rápida)
>      → SUMATRIPTÁN / NARATRIPTÁN
> ```
>
> 🔑 El **OH** de la serotonina da afinidad por 5-HT₃, así que hay que **sacarlo** para ganar selectividad. Las posiciones **1, 2 y β no deben sustituirse**.

**2) Tabla**

| | **A** (paroxetina) | **B** (nomifensina) |
|---|---|---|
| **Mecanismo de acción** | **ISRS** — inhibidor selectivo de la recaptación de **serotonina** (bloquea **SERT**) | Inhibidor de la recaptación de **noradrenalina** y dopamina (bloquea **NET**) |
| **Nº de estereoisómeros** | 2 centros quirales → **4** | 1 centro quiral → **2** |
| **Familia química** | **Ariloxialquilamina** | **Arilalquilamina** |

**b) Farmacóforo**

> - **Paroxetina:** el grupo **ariloxi** (O unido al benzodioxol) + la cadena + la **amina** del anillo de piperidina. El anillo fluorofenilo aporta pero no es el núcleo.
> - **Nomifensina:** el sistema **arilalquilamina**: anillo aromático + cadena carbonada + **amina**.

## TEMA 2

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen_P7.jpg)

### Respuestas correctas

**1) Compuesto dado: GRANISETRÓN** (indazol N-metilado + carboxamida + azabiciclo)

> **a) Grupos ionizables a pH 7,40:** la **amina terciaria** del sistema azabicíclico (tropano).
>
> **b) Blanco farmacológico:** receptor **5-HT₃** (antagonista). Es el único receptor de serotonina asociado a un **canal iónico**; los demás son GPCR.
>
> **c) Aplicación clínica:** **náuseas y vómitos inducidos por quimioterápicos** (antiemético).
>
> **d) Se desarrolló a partir de la farmacomodulación de las ORTOPRAMIDAS** (benzamidas con metoxilo en *orto*), en particular de la **METOCLOPRAMIDA**, que es antiemética por antagonismo **D2 y 5-HT₃**. También contribuyó la **cocaína**, que tiene débil actividad antagonista 5-HT₃ (vía bemesetron / MDL72222).

**2) Tabla**

| | **A** (nisoxetina) | **B** (sertralina) |
|---|---|---|
| **Mecanismo de acción** | **ISRNA** — inhibidor selectivo de la recaptación de **noradrenalina** (bloquea **NET**) | **ISRS** — inhibidor selectivo de la recaptación de **serotonina** (bloquea **SERT**) |
| **Nº de estereoisómeros** | 1 centro quiral → **2** | 2 centros quirales → **4** |
| **Familia química** | **Ariloxialquilamina** | **Arilalquilamina** (tetralina) |

⚠️ **A no es un antagonista serotoninérgico**: actúa sobre el **transportador**, no sobre el receptor. Y la familia no es "éter de aminoalquilo" (esa es de antihistamínicos H1).

### 🎯 LA REGLA que define el mecanismo

| Sustituyente en el grupo fenoxi | Selectividad |
|---|---|
| **Atractor de electrones en *PARA*** (−CF₃) | **SEROTONINA (ISRS)** |
| **Dador de electrones en *ORTO*** (−OCH₃, −CH₃) | **NORADRENALINA (ISRNA)** |

El par didáctico: **fluoxetina** (−CF₃ en para → ISRS) vs. **nisoxetina** (−OCH₃ en orto → ISRNA). Estructuras casi idénticas, mecanismos opuestos.

📌 Los **duales** (venlafaxina, duloxetina) **no cumplen ninguna** de las dos reglas.

💡 **Truco:** aprendete **solo la nisoxetina**. Sacándole el orto-metoxi y poniéndole CF₃ en para tenés la fluoxetina. Con una estructura memorizada contestás las dos.

### ⚠️ Setrones vs. triptanes — se confunden porque los dos tienen indol

| | Después del indol |
|---|---|
| **Triptanes** | Son **triptaminas**: cadena corta terminada en **amina** |
| **Setrones** | Hay un **carbonilo** entre el indol y la amina |

---

# PREGUNTA 8 — Deducción estructural, metabolismo y logP

## TEMA 1

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen-tema1_P8.jpg)

### Respuestas correctas

**Datos:** C₁₈H₂₂**N₂** · MW 266,38 · logP 3,90 · logD₇,₄ 1,37 · pKa 10,02 · Refractividad 85,31 · **α = 58°, β = 32°, γ = 20°**

**a) Dibuje el compuesto, indique actividad y mecanismo**

> **Paso 1 — la topología.** β ≠ 0° → anillo central de **7 miembros**. **γ ≠ 0°** → anillos **no coplanares** → carbonos **sp³** en el puente → **ANTIDEPRESIVO**.
>
> **Paso 2 — la fórmula.** Hay **DOS nitrógenos** → uno está en el anillo y otro en la cadena → **DIBENZOAZEPINA**.
>
> **Paso 3 — repartir los átomos.** El tricíclico aporta C₁₄H₁₂N, la cadena de 3 C aporta C₃H₆, y queda **CH₄N = −NH−CH₃** (amina **secundaria**).
>
> **Paso 4 — el pKa** de 10,02 confirma una amina alifática secundaria.
>
> **→ El compuesto es la DESIPRAMINA.**
>
> **Actividad:** antidepresivo. **Mecanismo:** inhibidor de la recaptación de **noradrenalina** y serotonina (NET/SERT).

⚠️ **No es −NH₂.** Con amina primaria la fórmula daría C₁₇H₂₀N₂ = 252, no 266.

**b) Grupo funcional responsable del pKa:** la **amina secundaria** de la cadena lateral.

**c) Precursor, sistema enzimático y productos**

> **Precursor: IMIPRAMINA** (misma estructura con amina **terciaria**, −N(CH₃)₂; C₁₉H₂₄N₂).
>
> **Sistema enzimático: citocromo P450** — **N-desalquilación oxidativa** (fase 1).
>
> **Productos:** **desipramina** + **formaldehído (HCOH)**.

⚠️ El subproducto es **formaldehído**, no metanol.

📌 Dato que suma: el metabolito es **más activo** que su precursor, así que la imipramina funciona como **profármaco**. Pero la desmetilación no puede seguir: las aminas **secundarias** conservan la lipofilia para llegar al SNC; una primaria ya no.

**d) logP del precursor**

> El hidrógeno sustituido está sobre un **NITRÓGENO**, no sobre un carbono aromático. **No se puede usar π(H) = 0.** Hay que considerar la pérdida de la **función entera** y la adición del **fragmento completo**:
>
> $$\log P_{\text{imipramina}} = \log P_{\text{desipramina}} - \pi(-\mathrm{NHCH_3}) + \pi(-\mathrm{N(CH_3)_2})$$
>
> $$= 3{,}90 - \pi(-\mathrm{NHCH_3}) + \pi(-\mathrm{N(CH_3)_2})$$
>
> con los valores de **π alquílico (π\*)** de la tabla de descriptores.

⚠️ **Lo que NO va:** `3,90 + (2 × 0,56)`. Eso aplica la regla del carbono aromático a un hidrógeno sobre nitrógeno. El corrector lo marcó con **"RESTAR AMINA"**.

## TEMA 2

![](/home/user/Shakira-perfume/quimica-medicinal/.img-web/examen_P8.jpg)

### Respuestas correctas

**Datos:** C₁₉H₂₁**N** · MW 263,38 · logP 4,43 · logD₇,₄ 1,58 · pKa 10,47 · Refractividad 96,21 · **α = 53°, β = 31°, γ = 22°**

**a) Dibuje el compuesto, indique actividad y mecanismo**

> **Paso 1.** β ≠ 0° → anillo central de 7 miembros. **γ ≠ 0°** → **ANTIDEPRESIVO**.
>
> **Paso 2.** Hay **UN solo nitrógeno** → el anillo central cierra con **carbono** → **DIBENZOCICLOHEPTENO** (10,11-dihidro, con los dos CH₂ sp³ que generan el γ, y doble enlace exocíclico hacia la cadena).
>
> **Paso 3.** El tricíclico aporta C₁₅; quedan **3 carbonos de cadena + 1 metilo sobre el N** → amina **secundaria −NH−CH₃**.
>
> **→ El compuesto es la NORTRIPTILINA.**
>
> **Actividad:** antidepresivo. **Mecanismo:** inhibidor de la recaptación de NA y 5-HT.

⚠️ **No es "antagonista dopaminérgico"** — ese es el mecanismo de un neuroléptico. Y la cadena es de **3 carbonos**, nunca de 4 (la de 4 es de las **butirofenonas**).

**b) Grupo funcional responsable del pKa:** la **amina secundaria**.

**c) Precursor, sistema enzimático y productos**

> **Precursor: AMITRIPTILINA** (amina terciaria, −N(CH₃)₂).
> **Enzima: citocromo P450**, N-desalquilación oxidativa.
> **Productos: nortriptilina + formaldehído.**

**d) logP del precursor**

> $$\log P_{\text{amitriptilina}} = 4{,}43 - \pi(-\mathrm{NHCH_3}) + \pi(-\mathrm{N(CH_3)_2})$$

⚠️ **Lo que NO va:** `4,43 + 0,50`.

### 🎯 El método, paso a paso (sirve para cualquier variante)

```
1) Mirá β y γ
      β ≠ 0  → anillo central de 7 miembros
      γ ≠ 0  → anillos no coplanares → ANTIDEPRESIVO
      γ = 0 y cadena 3C → NEUROLÉPTICO
      γ = 0 y cadena 2C → ANTIHISTAMÍNICO

2) Contá los NITRÓGENOS de la fórmula molecular
      1 N  → el anillo central cierra con carbono → DIBENZOCICLOHEPTENO
      2 N  → hay un N en el anillo → DIBENZOAZEPINA

3) Restá los átomos del tricíclico y repartí el resto
      cadena SIEMPRE de 3 C + lo que quede sobre el nitrógeno

4) Confirmá con el pKa (~10 = amina alifática)
```

### 🔑 La regla del logP, que falló en las dos versiones

> **π(H) = 0 SOLO cuando el hidrógeno está unido a un CARBONO AROMÁTICO.**
> Si está sobre un **heteroátomo** (N, O), hay que **restar el grupo entero y sumar el grupo entero**.

| | |
|---|---|
| ❌ MAL | logP(anilina) − π(H) + π(CH₃) |
| ✅ BIEN | logP(anilina) − π(**NH₂**) + π(**NHCH₃**) |

Caso en que **sí** se usa π(H) = 0: prednisolona → 6α-metilprednisolona, donde el H está sobre un carbono:
logP = 1,00 − 0 + 0,50 = **1,50** ✓

---

# RESUMEN DE ERRORES TRANSVERSALES

Los mismos cinco errores aparecieron en las dos versiones del examen:

1. **Mezclar mecanismo de acción con aplicación clínica.** "Neuroléptico" y "antidepresivo" son **acciones**; las aplicaciones clínicas son **esquizofrenia** y **depresión**. Y "agonista β2 selectivo" es mecanismo, no utilidad terapéutica.

2. **Nombres de familias incompletos.** *Ariletil*amina por **ariletanol**amina · *ariloxipropil*amina por **ariloxipropanol**amina · *éter de aminoalquilo* por **ariloxialquilamina** · *fenotiazina* por **tioxanteno**.

3. **Escribir la respuesta correcta y después agregar otra.** Pasó en la Pregunta 2 del Tema 1: el segundo nombre anula al primero.

4. **π(H) = 0 fuera de lugar.** Solo vale sobre carbono aromático.

5. **Justificar con el dato equivocado.** En QSAR, el R² en vez del p-valor de Student. En anti-H2, el pKa y la toxicidad en vez de la solvatación.

### Y tres distinciones finas que se tomaron

| Distinción | Qué significa |
|---|---|
| **Isómero de cadena ≠ homólogo** | El isómero conserva la fórmula y cambia la ramificación; el homólogo agrega o quita un CH₂ |
| **Bioprecursor ≠ profármaco con transportador** | El bioprecursor necesita un proceso **redox**; el transportador se libera por **hidrólisis**. El **mixto** tiene los dos |
| **Ampliación de anillo ≠ equivalencia anular** | Ampliar cambia el **tamaño** del anillo (6→7); la equivalencia reemplaza **un anillo por otro** (benceno→piridina) |
