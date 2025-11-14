# ¿Ha muerto el rock?

## 1.0.1 Hipótesis General

La música rock, que dominó la escena musical global durante décadas, ha experimentado una pérdida notable de popularidad en los últimos años frente a géneros más actuales como el pop, el hip-hop, la música electrónica y el reggaetón. Esta caída no solo se observa en la disminución de reproducciones de canciones de rock en plataformas de streaming como Spotify, sino también en cambios en las preferencias de los oyentes, en la evolución de las características musicales (como la *bailabilidad* o la *energía*) y en la menor presencia de artistas de rock en rankings globales.

A través del análisis de múltiples datasets de Spotify entre 2000 y 2024, este proyecto busca determinar si el rock ha perdido relevancia cultural y comercial en la era del streaming.

## 1.0.2 Hipótesis Secundarias

1. **Hipótesis Secundaria 1:** La popularidad del rock ha disminuido progresivamente en las listas globales de Spotify desde el año 2000, siendo superado por géneros como el pop y el hip-hop a partir de 2010.
2. **Hipótesis Secundaria 2:** Las características musicales del rock (alta energía, mayor instrumentalidad) son actualmente menos valoradas por los oyentes, que muestran preferencia por canciones con mayor *bailabilidad* y *valence*, típicas del pop y el EDM.
3. **Hipótesis Secundaria 3:** El perfil demográfico de los oyentes de rock es diferente al de otros géneros, con una audiencia de mayor edad y menor interacción con funcionalidades de descubrimiento musical como *Discover Weekly*.

---

## 1.1 Introducción

### 1.1.1 Contexto Histórico y Cultural

El rock nació en los años 50 como una fusión de *rhythm and blues*, country y gospel. Durante las décadas siguientes evolucionó hacia subgéneros como el rock clásico, punk, metal, grunge y alternativo, dando lugar a bandas icónicas como **The Beatles**, **Led Zeppelin**, **Nirvana** o **Radiohead**.

Sin embargo, con la llegada del nuevo milenio, otros géneros como el hip-hop, el pop y la música electrónica comenzaron a dominar el panorama global. Plataformas como Spotify, lanzada en 2008, intensificaron esta transición al priorizar la personalización y los algoritmos de recomendación.

### 1.1.2 La Era del Streaming

Spotify transformó tanto *cómo* escuchamos música como *qué* escuchamos. Sus listas curadas (como *Top 50 Global*) reflejan y moldean las preferencias del público. En este contexto, el rock parece haber perdido terreno frente a géneros más *streaming-friendly*.

---

## 1.2 Importación de librerías y carga de datos

### 1.2.1 Datasets utilizados

| Dataset                                             | Descripción                               |
| --------------------------------------------------- | ----------------------------------------- |
| **history-of-rock-spotify.csv**                     | Canciones de rock con métricas de audio   |
| **Global_Music_Streaming_Listener_Preferences.csv** | Preferencias de oyentes por país y género |
| **Spotify_2024_Global_Streaming_Data.csv**          | Streams globales por artista y género     |
| **high_popularity_spotify_data.csv**                | Canciones con popularidad > 70            |
| **low_popularity_spotify_data.csv**                 | Canciones con popularidad < 30            |

### 1.2.2 Librerías y herramientas empleadas

* **pandas** y **numpy** para manipulación de datos
* **matplotlib** y **seaborn** para visualización
* Filtrado y normalización de columnas numéricas

### 1.2.3 Limpieza de los CSVs

Se eliminaron duplicados, se estandarizaron nombres de columnas y se corrigieron tipos numéricos. Se verificó que no hubiera valores nulos relevantes.

---

## 1.3 Parte 1: Evolución histórica del rock

Se analiza la evolución de la popularidad media del rock entre 2000 y 2024 usando el dataset principal.

### Resultados clave

* La nube de puntos refleja la dispersión anual de popularidad de canciones de rock.
* La línea de tendencia muestra claramente un **descenso progresivo desde 2005**.

Además, se comparó el comportamiento del rock en canciones de alta y baja popularidad:

* Las canciones de rock aparecen **más frecuentemente en la categoría de baja popularidad**, especialmente a partir de 2015.

---

## 1.4 Parte 2: Preferencias globales de oyentes

### Preferencias por edad

El análisis muestra que:

* Los oyentes más jóvenes (15–25 años) tienen un porcentaje muy reducido de preferencia por el rock.
* Los picos más altos aparecen en edades mayores (30–45), reflejando un público más adulto.

Esto refuerza la hipótesis de que el rock **no conecta igual con las nuevas generaciones**.

### Preferencias por país

Ningún país supera el 13 % de oyentes que eligen el rock como género principal.

**Conclusión parcial:** El rock se mantiene como género minoritario o nostálgico, sin liderazgo global.

---

## 1.5 Parte 3: Popularidad actual (2024)

Usando datos recientes de YouTube (2020–2022), se comparó la presencia del rock con otros géneros.

### Observaciones principales

* Los géneros más vistos son el **pop**, el **hip-hop**, y la **música urbana**.
* El rock aparece con un tamaño de burbuja pequeño, indicando bajos niveles de visualización.

Esto muestra que el declive del rock se extiende también a plataformas de vídeo musical.

---

## 1.6 Conclusiones Generales

* La popularidad histórica del rock muestra una **tendencia descendente clara**.
* Las preferencias globales de los oyentes confirman que otros géneros lo superan ampliamente.
* Los datos recientes de 2024 reflejan que el rock **ya no es un género dominante** en ninguna plataforma.

### **Conclusión final:**

Los datos respaldan la hipótesis de que el rock ha perdido relevancia en la industria musical moderna. Aunque sigue siendo un género fundamental desde el punto de vista cultural e histórico, su impacto actual en las plataformas de streaming es muy inferior al de otros géneros emergentes y populares.

