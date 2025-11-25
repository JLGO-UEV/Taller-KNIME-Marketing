# Taller-KNIME-Marketing


# 🏆 Classroom ML Leaderboard

Bienvenido al sistema de evaluación automatizada para el ejercicio de Machine Learning. Esta aplicación gestiona las entregas de los equipos, valida los resultados contra la solución real ("Ground Truth") y actualiza el ranking en tiempo real.

---

## 🧑‍🎓 Parte 1: Instrucciones

### 🎯 El Objetivo
Vuestro objetivo es entrenar el mejor modelo de Machine Learning posible para el dataset proporcionado en clase. Una vez tengáis vuestras predicciones, debéis subirlas a esta plataforma para ver qué tal rendís frente al resto de equipos.

### 📂 Formato de Entrega (Submission)
El archivo que subáis **debe ser obligatoriamente un CSV** (`.csv`) y cumplir estrictamente con el siguiente formato:

1.  **Separador:** Coma (`,`).
2.  **Cabeceras:** Debe tener dos columnas llamadas exactamente `ID` y `PRED`.
3.  **Contenido:**
    *   `ID`: El identificador de la fila (correspondiente al dataset de test).
    *   `PRED`: La clase predicha por vuestro modelo (ej. 0 o 1).

**Ejemplo de archivo `submission.csv` válido:**

```csv
ID,PRED
1,0
2,1
3,0
4,1
...
```

> ⚠️ **Importante:** Si los nombres de las columnas no son exactos o los IDs no coinciden con los esperados, la plataforma rechazará la entrega.

### 📏 Métrica de Evaluación
La clasificación se basa en **Accuracy** (Exactitud).
$$ Accuracy = \frac{\text{Predicciones Correctas}}{\text{Total de Muestras}} $$

### 🚀 Cómo enviar tu solución
1.  Entra en la aplicación.
2.  Haz clic en el botón **"🚀 Submit Predictions"**.
3.  Selecciona tu **Nombre de Equipo** en el desplegable (Equipo 1 - Equipo 10).
4.  Selecciona tu archivo `.csv`.
5.  Pulsa **"Evaluar Modelo"**.

Si todo ha ido bien, el sistema te devolverá tu puntuación y actualizará el Leaderboard si has entrado en el TOP 3.

---

## 🛠️ Parte 2: Documentación Técnica (Backend)

Archivos:

**train.csv** -> Para hacer todos los entrenamientos y pruebas
**test.csv** -> No tiene la columna ***y*** que es la que hay que predecir
**submission_template.csv** -> hay que poner las predicciones hechas con el **test.csv** en la columna **PRED**

Una vez preparado el **submission_template.csv**, se subes las predicciones a la plataforma y a ver qué tal!!

>https://submission-marketing-knime.onrender.com/
