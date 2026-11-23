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
