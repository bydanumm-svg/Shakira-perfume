# TEMA 5 — Antagonistas H2 (Pregunta 5)

Es la pregunta más "memorizable" del examen: una vez que sabés la historia del desarrollo, se contesta sola.

---

## 1. Qué te tomaron

Te dieron la secuencia **metiamida (SKF 92058) → cimetidina (SKF 92334) → ranitidina (Zantac®)**, con las tres regiones terminales marcadas con **líneas punteadas**:

| Compuesto | Región punteada |
|---|---|
| Metiamida | **Tiourea** (–NH–C(=S)–NH–CH₃) |
| Cimetidina | **Cianoguanidina** (–NH–C(=N–CN)–NH–CH₃) |
| Ranitidina | **Nitroetendiamina** (–NH–C(=CH–NO₂)–NH–CH₃) |

**a)** ¿Qué tipo de relación farmacomodulativa vincula a los tres compuestos considerando esas regiones? Justifique con **argumentos fisicoquímicos**.

**b)** Según la REA de la familia, ¿qué consecuencia sobre la actividad se espera al reemplazar el grupo **cianoguanidino** por uno de tipo **N-metilurea** (–NH–CO–NHCH₃)? Explique a qué se debería ese efecto sobre la potencia anti-H2.

---

## 2. Qué pusiste y por qué está mal

### a) Quedó en blanco ❌

Era la mitad del puntaje y se contestaba con dos palabras más una lista de criterios.

### b) Encaminada pero con el argumento equivocado ⚠️ (marcado "NC")

Escribiste:

> *"El oxígeno de la metilurea es dador de e⁻. Esto no es favorable ya que aumentaría la toxicidad y se busca que el pKa de la metilhistamina se asemeje al de la histamina."*

**Tres problemas:**

1. **Mezclaste dos etapas distintas del desarrollo.** El argumento del **pKa** corresponde a la optimización del **anillo imidazólico** (burimamida → tioburimamida → metiamida). El argumento de la **toxicidad** corresponde al reemplazo de la **tiourea**. Pero esta pregunta es sobre el **extremo polar** y la REA final de la cimetidina, que es otra cosa.
2. **La toxicidad no es el punto.** La pregunta pregunta explícitamente por la **potencia**, no por la toxicidad. De hecho el análogo urea tiene **baja** toxicidad.
3. **Faltó decir qué pasa.** No dijiste explícitamente que la potencia **disminuye**.

Acertaste en intuir que el cambio es desfavorable, pero el mecanismo es otro: **solvatación y lipofilia**.

---

## 3. Cómo había que encararlo

### Respuesta a)

> Los tres compuestos están vinculados por una relación de **BIOISOSTERISMO NO CLÁSICO** (isosterismo de grupos funcionales): el grupo **tiourea** de la metiamida fue reemplazado por **cianoguanidina** en la cimetidina y por **nitroetendiamina** en la ranitidina.
>
> **Justificación fisicoquímica** — los tres grupos comparten:
>
> | Propiedad | Por qué importa |
> |---|---|
> | **Planaridad** | Los tres son grupos planos, lo que permite la misma orientación en el sitio de unión |
> | **Tamaño similar** | Ocupan aproximadamente el mismo volumen |
> | **Capacidad de formar dos puentes de hidrógeno simultáneos** | Es el requisito para la interacción con el receptor H2 |
> | **Carácter NO básico (pKa muy bajo)** | No se protonan a pH fisiológico, por lo que interactúan por puentes de hidrógeno y no por interacciones electrostáticas |
> | **Momento dipolar adecuado** (magnitud y orientación) | Es el descriptor que correlaciona con la actividad en el modelo QSAR final |
>
> Lo determinante es el último punto: **las interacciones electrostáticas favorecen el agonismo, mientras que los puentes de hidrógeno favorecen el antagonismo**. Por eso los tres grupos deben ser no básicos y capaces de dar puentes de hidrógeno, y por eso se requirió incorporar grupos fuertemente atractores de electrones (–CN, –NO₂) que bajan el pKa de la guanidina de 13 a ~0,4–0,9.

📌 Si piden datos: tiourea pKa = −1,2; N-nitroguanidina = 0,9; N-cianoguanidina = 0,4; guanidina sin sustituir = 13.

### Respuesta b)

> **La potencia como antagonista H2 DISMINUYE.**
>
> **Causa: solvatación.** El grupo N-metilurea es considerablemente **más polar e hidrofílico** que el cianoguanidino, por lo que tiene un **logP menor**.
>
> Según la REA establecida para esta familia:
>
> $$\log(\text{actividad}) = 2{,}0 \log P + 7{,}4$$
>
> es decir, **la actividad aumenta al aumentar el logP** del grupo terminal.
>
> El razonamiento fisicoquímico es el siguiente: **a mayor polaridad e hidrofilia de un grupo funcional, más fácil es su solvatación en agua y más difícil su desolvatación**. Para que el extremo polar cumpla su función necesita establecer **dos puentes de hidrógeno simultáneos** con el receptor, y para eso primero debe **desolvatarse**. Si el grupo está fuertemente solvatado, el costo energético de quitarle las moléculas de agua es alto y queda **menos disponible para el acoplamiento ligando-receptor**.
>
> Por lo tanto, al reemplazar la cianoguanidina (menos hidrofílica) por una N-metilurea (más hidrofílica), la desolvatación se dificulta y **cae la potencia anti-H2**.

📌 **Dato que lo confirma:** en el gráfico de log(actividad) vs. logP del teórico, los derivados de **urea** están en el extremo inferior izquierdo (menor logP, menor actividad), mientras que las **cianoguanidinas N-metiladas** están arriba a la derecha.

📌 **El mismo razonamiento** explica por qué, cuando en la tioburimamida se probó reemplazar el **azufre por oxígeno**, la potencia bajó: el oxígeno se solvata más.

---

## 4. Cómo te lo pueden volver a tomar

1. **"¿Por qué se reemplazó la tiourea de la metiamida?"**
   → Porque el grupo **tiourea** es el responsable de la **toxicidad renal y hematológica** (agranulocitosis). Se probaron urea y guanidina: ambas de baja toxicidad, pero menor potencia; la guanidina además resultó **antagonista puro**.

2. **"¿Por qué hubo que agregar –CN o –NO₂ a la guanidina?"**
   → Porque la guanidina tiene **pKa ≈ 13** y se protona a pH fisiológico. Protonada, vuelve a dar interacciones **electrostáticas**, que favorecen el **agonismo**. Un grupo **atractor de electrones** baja el pKa y la mantiene neutra → puentes de hidrógeno → **antagonismo**.

3. **"¿Por qué se insertó un azufre en la cadena de la burimamida?"**
   → El S es **atractor de electrones** por efecto inductivo. Baja el pKa del imidazol de 7,25 a 6,25, acercándolo al de la histamina (5,8), reduciendo la fracción ionizada a pH fisiológico.

4. **"¿Por qué un metilo en posición 4?"**
   → Es un grupo **dador de electrones** ubicado **cerca de Nτ y lejos de Nπ**. Aumenta selectivamente la basicidad de **Nτ**, favoreciendo el tautómero que imita a la histamina. Además restringe la rotación de la cadena lateral (es lo mismo que daba selectividad H2 a la 4-metilhistamina).

5. **"¿Qué estrategia se usó para determinar el confórmero activo de la cimetidina?"**
   → Síntesis de un **análogo rígido** (formación de anillo para fijar la conformación). El análogo conservó la potencia.

6. **"Dibuje un antagonista H2 y uno H1 y señale las diferencias."**
   → H2: anillo imidazol (o furano/tiazol) + cadena larga con S + extremo polar plano no básico. H1: dos grupos voluminosos + puente de 2 carbonos + amina terciaria con sustituyentes pequeños.

7. **Modelo QSAR final.** `log A = 9,12 cos θ + 0,6 log P − 2,71`. Lo relevante: la actividad depende de la **orientación** del momento dipolar (θ), no de su magnitud.

---

## 5. Las tres frases para tener listas

1. *"Las interacciones electrostáticas favorecen la acción agonista; los puentes de hidrógeno favorecen la acción antagonista sobre los receptores H2."*
2. *"A mayor polaridad e hidrofilia, más fácil la solvatación y más difícil la desolvatación; el grupo debe desolvatarse para establecer los dos puentes de hidrógeno simultáneos con el receptor."*
3. *"Un grupo atractor de electrones baja el pKa y evita la protonación a pH fisiológico."*

Y la cita de James Black, que resume todo el desarrollo:

> *"Sabíamos que el receptor unía histamina, así que era cuestión de **conservar la afinidad y perder la eficacia**."*
