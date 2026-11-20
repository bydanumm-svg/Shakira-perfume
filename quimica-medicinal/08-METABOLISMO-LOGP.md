# TEMA 8 — Deducción estructural, metabolismo y logP (Pregunta 8)

Esta pregunta junta tres temas: **topología tricíclica**, **metabolismo de fase 1** y **cálculo de logP**. El error del logP es el mismo concepto que te costó en la Pregunta 1, así que arreglarlo sirve doble.

---

## 1. Qué te tomaron

Un compuesto con estos datos:

| Dato | Valor |
|---|---|
| Fórmula molecular | **C₁₉H₂₁N** |
| Peso molecular | **263** |
| logP | **4,43** |
| pKa | **10,47** |
| Topología | **α = 53°, β = 31°, γ = 22°** |

Se pedía: **a)** deducir y dibujar la estructura; **b)** familia química y actividad; **c)** el precursor del que proviene por **N-desalquilación** y la reacción involucrada; **d)** el **logP del precursor**.

---

## 2. Qué pusiste y por qué está mal

### a) La cadena lateral ❌ — el corrector escribió "NO, cadena de 4 carbonos"

Dibujaste una cadena de **4 carbonos** terminada en una amina **primaria** (–NH₂).

**Dos problemas:**

1. **La fórmula molecular no cierra.** Con C₁₉H₂₁N, si contás los átomos del sistema tricíclico (C₁₅ con los dos bencenos y el puente) te quedan **4 carbonos** para repartir entre la cadena **y** los sustituyentes del nitrógeno. Con una cadena de 4 C y –NH₂ te sobran carbonos y no da el hidrógeno.
2. **La REA lo prohíbe.** La cadena de los antidepresivos tricíclicos es de **3 carbonos**, nunca de 4. La de 4 carbonos es la de las **butirofenonas** (haloperidol), que son neurolépticos no tricíclicos.

🔑 La respuesta correcta es **cadena de 3 carbonos + amina SECUNDARIA (–NH–CH₃)**.

### d) El logP del precursor ❌ — el corrector escribió "NO, restar amina"

Hiciste:

> logP(precursor) = 4,43 **+ 0,50** = 4,93

Es decir, sumaste el π del metilo sobre el hidrógeno de la amina, como si estuvieras reemplazando un **H unido a un carbono aromático**.

🔑 **Y esa es exactamente la regla que no se puede aplicar acá.**

> **π(H) = 0 SOLO cuando el hidrógeno está unido a un CARBONO AROMÁTICO.**
>
> Si el hidrógeno está sobre un **heteroátomo** (N, O), hay que **restar el grupo funcional entero y sumar el grupo entero** que lo reemplaza.

Como el hidrógeno que se sustituye está sobre el **nitrógeno**, no sobre un carbono aromático, el método correcto es sacar la amina completa y poner la amina completa. De ahí el **"restar amina"** del corrector.

---

## 3. Cómo había que encararlo

### a) Deducción de la estructura ⭐

**Paso 1 — La topología dice qué sistema tricíclico es.**

| Observación | Conclusión |
|---|---|
| **β = 31° ≠ 0°** | El anillo central es de **7 miembros** |
| **γ = 22° ≠ 0°** | Los anillos **no son coplanares** → el puente tiene **carbonos sp³** → es un **ANTIDEPRESIVO** |

**Paso 2 — La fórmula molecular dice cuál de los sistemas de 7 miembros.**

C₁₉H₂₁N tiene **un solo nitrógeno**. Si fuera una **dibenzoazepina** (imipramina y familia), habría **dos** nitrógenos: el del anillo y el de la cadena. Con un solo N, el anillo central debe cerrarse con **carbono** → es un **dibenzociclohepteno**.

**Paso 3 — El resto de la fórmula da la cadena.**

El sistema dibenzocicloheptadieno aporta C₁₅. Quedan **C₄H** para la cadena lateral y el nitrógeno: **3 carbonos de cadena + 1 metilo sobre el N**, es decir una **amina secundaria**.

**Paso 4 — El pKa lo confirma.** pKa = 10,47 corresponde a una **amina alifática secundaria**, no a una primaria ni a una terciaria aromática.

> **La estructura es la NORTRIPTILINA:** sistema **dibenzociclohepteno** (10,11-dihidro, con los dos CH₂ sp³ que generan el ángulo γ), con un doble enlace exocíclico hacia una **cadena de 3 carbonos** terminada en **–NH–CH₃**.

⚠️ **Detalle fino que vale la pena entender:**

| Dibenzociclohepteno | γ | Actividad |
|---|---|---|
| Con **doble enlace** en el puente (10,11-deshidro) | **0°** | Antidepresivo **y** neuroléptico |
| **Saturado** (10,11-dihidro) — amitriptilina, nortriptilina | **≠ 0°** | **Antidepresivo puro** |

Es exactamente lo que explica la clase: el **doble enlace mantiene el anillo plano**; al **saturarlo**, aparece el ángulo γ y se pierde el carácter neuroléptico.

### b) Familia química y actividad

> **Familia química:** **dibenzociclohepteno** (antidepresivo tricíclico, ADT).
>
> **Actividad:** **antidepresivo**.
>
> **Mecanismo de acción:** inhibidor de la recaptación de noradrenalina y serotonina (bloquea los transportadores **NET** y **SERT**). La nortriptilina, al ser amina secundaria, es relativamente más selectiva por **noradrenalina**.

📌 Y de nuevo: no confundas **actividad/uso** (antidepresivo) con **mecanismo** (inhibidor de la recaptación).

### c) El precursor y la reacción ⭐

> **Precursor: AMITRIPTILINA** — la misma estructura, pero con el nitrógeno como **amina terciaria**: –N(CH₃)₂.
>
> **Reacción: N-DESALQUILACIÓN OXIDATIVA** (N-desmetilación), de **fase 1**, catalizada por el **citocromo P450**.
>
> **Productos:**
> 1. **Nortriptilina** (amina secundaria)
> 2. **Formaldehído** (HCHO)

🔑 **Regla de la N-desalquilación:** el fragmento que se va sale siempre como **compuesto carbonílico**.

| Sustituyente que se pierde | Producto |
|---|---|
| **metilo** | **formaldehído** (HCHO) |
| etilo | acetaldehído |
| isopropilo | acetona |

📌 **Dato que conviene agregar** (lo repite el teórico, y es el mismo caso de imipramina → desipramina): el metabolito **es activo**, de modo que la amitriptilina puede considerarse un **profármaco**. Pero la desmetilación **no puede seguir**: las aminas **secundarias** conservan la lipofilia adecuada para llegar al SNC; una amina **primaria** ya no la tendría.

### d) El logP del precursor ⭐⭐

> El hidrógeno que se sustituye está unido a un **nitrógeno**, no a un carbono aromático. Por lo tanto **no se puede usar π(H) = 0**: hay que considerar **la pérdida de la función entera y la adición del fragmento completo**.
>
> $$\log P_{\text{amitriptilina}} = \log P_{\text{nortriptilina}} - \pi(-\mathrm{NHCH_3}) + \pi(-\mathrm{N(CH_3)_2})$$
>
> $$= 4{,}43 - \pi(-\mathrm{NHCH_3}) + \pi(-\mathrm{N(CH_3)_2})$$
>
> con los valores de **π alquílico (π\*)** tomados de la tabla de descriptores.

⚠️ **Los valores numéricos hay que sacarlos de la tabla de la cátedra** — no los pongo acá para que no memorices un número equivocado. Lo que se evalúa es el **planteo**, y el planteo es ese.

**Resultado esperado:** la amina **terciaria** es algo más lipofílica que la secundaria, así que el logP del precursor sale **un poco mayor** que 4,43 (el valor experimental de la amitriptilina está alrededor de 4,9).

📌 Fijate que el **número** al que llegaste (4,93) no estaba lejos del real. Lo que te descontaron fue el **método**: aplicaste la regla del carbono aromático a un hidrógeno sobre nitrógeno.

### El ejemplo canónico de esta regla

Es el que está en la diapositiva de QSAR, con la anilina:

| | |
|---|---|
| ❌ MAL | logP(anilina) − π(H) + π(CH₃) |
| ✅ BIEN | logP(anilina) − π(**NH₂**) + π(**NHCH₃**) |

Y el caso en que **sí** se usa π(H) = 0: prednisolona → 6α-metilprednisolona, donde el H está sobre un carbono.
logP = 1,00 − 0 + 0,50 = **1,50** ✓

---

## 4. Cómo te lo pueden volver a tomar

1. **Mismo formato, otros datos.** Procedimiento:

```
1) Mirá β y γ
      β ≠ 0 → anillo central de 7 miembros
      γ ≠ 0 → anillos no coplanares → ANTIDEPRESIVO
      γ = 0 y cadena 3C → NEUROLÉPTICO
      γ = 0 y cadena 2C → ANTIHISTAMÍNICO

2) Contá los nitrógenos de la fórmula molecular
      1 N → el anillo central cierra con CARBONO (dibenzociclohepteno)
      2 N → dibenzoazepina

3) Restá los átomos del tricíclico y repartí el resto
      en la cadena (SIEMPRE 3 C en antidepresivos) y los sustituyentes del N

4) Confirmá con el pKa
      ~10 → amina alifática secundaria o terciaria
```

2. **Que la reacción sea otra de fase 1.** Las más probables:

   | Reacción | Productos |
   |---|---|
   | **N-desalquilación oxidativa** | Amina desalquilada + **carbonilo** |
   | **Desaminación oxidativa** | **Aldehído** + amina |
   | **Oxidación aromática** | Fenol, o *trans*-dihidrodiol → catecol |
   | **Oxidación de OH primario** (ADH/ALDH) | Aldehído → ácido carboxílico |
   | **Oxidación de OH secundario** (ADH) | Cetona |
   | **Hidrólisis de éster** (esterasas) | Ácido + alcohol |

3. **Que pidan el logP del metabolito en lugar del precursor.** Mismo planteo, al revés: restás la amina terciaria y sumás la secundaria.

4. **Que el cambio sea sobre un carbono aromático.** Ahí **sí** usás π(H) = 0 y simplemente sumás el π del grupo nuevo.

5. **Que pregunten si se altera el perfil de actividad.** Hay que contestarlo siempre, aunque no lo pidan explícitamente. En este caso: **el metabolito es activo** (incluso más selectivo por noradrenalina), así que el precursor funciona como **profármaco**.

---

## 5. Las tres cosas que no hay que volver a errar

1. **Cadena de 3 carbonos** en antidepresivos y neurolépticos tricíclicos. Nunca 4. La de 4 es de las **butirofenonas**.
2. **π(H) = 0 solo sobre carbono aromático.** Sobre un heteroátomo: **sacar el grupo entero, poner el grupo entero**.
3. **γ ≠ 0 → antidepresivo.** Es la firma topológica, y la fórmula molecular (número de nitrógenos) decide cuál de los sistemas es.
