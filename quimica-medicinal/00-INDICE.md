# Química Medicinal — Recuperatorio

Material de estudio para las **seis preguntas a recuperar: 1, 2, 5, 6, 7 y 8**.

---

## Cómo usarlo

Para cada tema hay **dos documentos**:

- **RESUMEN** → el tema explicado, armado con las diapositivas, tus anotaciones de clase y las clases grabadas.
- **FICHA** → la pregunta del examen: consigna, qué pusiste, por qué está mal, la respuesta modelo y las variantes con que te lo pueden volver a tomar.

**Orden sugerido de estudio:** leé primero el resumen del tema, después la ficha. La ficha sola sirve para repasar la noche anterior.

---

## Los seis temas

| Tema | Preg. | Nota | Resumen | Ficha |
|---|---|---|---|---|
| **QSAR / Hansch** | 1 | 2,5/10 | `01-QSAR-RESUMEN.pdf` | `01-QSAR.pdf` |
| **Adrenérgicos** | 2 | 4,5/10 | `02-ADRENERGICOS-RESUMEN.pdf` | `02-ADRENERGICOS.pdf` |
| **Antagonistas H2** | 5 | — | `05-ANTIH2-RESUMEN.pdf` | `05-ANTIH2.pdf` |
| **Tricíclicos y topología** | 6 | 1,5/10 | `06-08-SNC-RESUMEN.pdf` | `06-TRICICLICOS.pdf` |
| **5-HT3 y antidepresivos** | 7 | 3,5/10 | `06-08-SNC-RESUMEN.pdf` | `07-SEROTONINA.pdf` |
| **Metabolismo y logP** | 8 | — | `06-08-SNC-RESUMEN.pdf` | `08-METABOLISMO-LOGP.pdf` |

📌 Los temas 6, 7 y 8 salen del mismo teórico (Dopamina-Serotonina), por eso comparten un único resumen.

---

## Prioridades

Si tenés poco tiempo, este es el orden por rendimiento:

1. **Tema 6 — topología α/β/γ.** Es la peor nota y el contenido más mecánico. La tabla de los tres ángulos más el cuadro de doble entrada resuelve media pregunta sola.
2. **Tema 1 — QSAR.** Segunda peor nota, y son ocho criterios que se aplican siempre igual.
3. **Tema 5 — anti-H2.** Es una historia con una lógica clara; una vez entendida, no se olvida.
4. **Tema 7 — regla orto/para.** Una sola regla define todas las respuestas de mecanismo.
5. **Tema 2 — adrenérgicos.** Vocabulario de familias + configuración R/S.
6. **Tema 8 — logP.** Depende de una sola regla, la misma que aparece en QSAR.

---

## Los cinco errores que se repitieron en el examen

Vale la pena tenerlos presentes porque son transversales, no de un tema:

1. **Mezclar mecanismo de acción con utilidad terapéutica.** Apareció en las preguntas 2, 6 y 7. Mecanismo = agonista/antagonista/inhibidor + blanco. Utilidad = la enfermedad.
2. **Nombres de familias incompletos.** "Ariletilamina" por **ariletanolamina**; "ariloxipropilamina" por **ariloxipropanolamina**; "éter de aminoalquilo" por **ariloxialquilamina**. El sufijo indica el grupo funcional, no es un detalle.
3. **Justificar con el dato equivocado.** En QSAR usaste el R² cuando lo que decidía era el p-valor de Student y el intervalo de confianza.
4. **π(H) = 0 fuera de lugar.** Solo vale sobre carbono aromático. Sobre heteroátomo hay que sacar y poner el grupo entero.
5. **Dejar ítems en blanco.** Las preguntas 1c, 5a y 7d se contestaban en dos o tres renglones cada una.

---

## Las reglas que resuelven más puntos

### Topología tricíclica

|  | γ = 0° | γ ≠ 0° |
|---|---|---|
| **Cadena 2 C** | Antihistamínicos / anticolinérgicos | — |
| **Cadena 3 C** | **Neurolépticos** | **Antidepresivos** |

| Sistema | α | β | γ |
|---|---|---|---|
| Fenotiazina / Tioxanteno | 55° | 0° | 0° |
| Dibenzociclohepteno (insaturado) | 50° | 30° | 0° |
| Dibenzoazepina | 50° | 30° | 20° |

### Familias adrenérgicas

```
¿Hay O entre el anillo y la cadena?
   SÍ → ariloxipropanolamina → antagonista β → hipertensión
   NO → ¿hay OH en el carbono bencílico?
          SÍ → ariletanolamina → agonista
          NO → ariletilamina → indirecto
```

Configuración activa: ariletanolaminas **R**, ariloxipropanolaminas **S** (misma geometría, distinta prioridad CIP).

### Antidepresivos selectivos

- Atractor en **para** → **serotonina** (ISRS)
- Dador en **orto** → **noradrenalina** (ISRNA)

### QSAR — orden de evaluación

1. n ≥ 4v → 2. R² ≥ 0,70 → 3. Fisher p < 0,05 → 4. **Student p < 0,05 en todos** → 5. ningún IC contiene el cero → 6. ortogonalidad < 0,3 → 7. R² ajustado ≥ 0,65 → 8. parsimonia

**Si un solo regresor falla Student, se rechaza el modelo completo.**

### Anti-H2

- Interacciones **electrostáticas** → agonismo
- **Puentes de hidrógeno** → antagonismo
- Mayor hidrofilia → más solvatación → desolvatación más difícil → **menor potencia**

### Signos de descriptores

| Descriptor | Positivo | Negativo |
|---|---|---|
| σ de Hammett / σ* de Taft | atractor | dador |
| π | lipofílico | hidrofílico |
| **Es de Taft** | — | **más negativo = más voluminoso** |

---

## Material original

Los PDFs de la cátedra están en la carpeta `pdfs/`:

| Archivo | Tema |
|---|---|
| `01-SAR.pdf` | Farmacomodulación, bioisosterismo |
| `02-QSAR-I.pdf` · `03-QSAR-II.pdf` | QSAR |
| `04-Metabolismo.pdf` | Metabolismo |
| `05-Profarmacos.pdf` | Profármacos |
| `06-Adrenergicos-Colinergicos.pdf` | Adrenérgicos |
| `07-Antihistaminicos.pdf` | H1 y H2 |
| `08-Dopamina-Serotonina.pdf` | SNC |
