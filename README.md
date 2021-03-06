# Curso de Fundamentos de Procesamiento de Lenguaje Natural con Python y NLTK

Aprende cómo los algoritmos pueden aprender a procesar el lenguaje humano con Python y NLTK y entrena tus primeros modelos de procesamiento de lenguaje natural

- Elementos esenciales de la lingüistica y la programación, para poder construir modelos de Machine Learning y Deep Learning

**NOTA**

Para usar Latex en Colab o Jupyter éste recurso es muy importante a tener encuenta
[Learn How to Write Markdown & LaTeX in The Jupyter Notebook](https://towardsdatascience.com/write-markdown-latex-in-the-jupyter-notebook-10985edb91fd)

## Introducción al NLP: Perspectivas y estados del arte

NLP es el camino hacia el ideal de la IA

- **NLP** Natural Language Processing
  Estudia interacciones entre humanos y máquina que los humanos usamos a diario para comunicarnos

- **NLU** Natural Language Understanding

> _… Si un humano no puede distinguir entre una máquina y otra persona en una conversación, entonces esa máquina ha alcanzado un nivel de inteligencia comparable al de un humano …_ Test de Turing

El **lenguaje** es un proxy o una medida de una inteligencia de un algoritmo.

- Blade Runner, 1982 (Película recomendada)
- [NLTK Corpora](http://www.nltk.org/nltk_data/)
- [Expresión regular](https://es.wikipedia.org/wiki/Expresión_regular)

### Usos actuales del NLP

- Máquinas de búsqueda
- Traducción de texto
- Chatbots
- Análisis de discurso
- Reconocimiento del habla

El área del PLN (Procesamiento del Lenguaje Natura), es muy difícil, porque puede tener muchas interpretaciones.

**¿Por qué es tan difícil?**

Porque el lenguaje humano es **difuso**, **ambigüo** y requiere **mucho contexto**.

### Evolución del NLP

- Sistemas basados en Reglas (1950s - 1990s)
- Estadísticas de Corpus (1990s - 2000s)
  Un corpus es una colección de diferentes textos
- Machine Learning (2000s - 2014)
- Deep Learning (2014 - 2020)

Hoy es dia el deep learning es el estado del arte del lenguaje de procesamiento natural.

La inteligencia artificial todavía no tiene el sentido común para entender nuestro lenguaje. (MIT Review - Enero de 2020)

### ¿Qué vamos a utilizar?

- **NLTK**: Permite entender mejor la estadística de corpus para hacer procesamiento del lenguaje y poder realizar modelos sencillos que desarrollen tareas cómo clasificación de textos.
- **spaCy**

**Roadmap del contenido**

| Roadmap        | NLTK | spaCy |
| -------------- | ---- | ----- |
| Fundamentos    | [x]  | [ ]   |
| Aplicaciones   | [x]  | [ ]   |
| NLP industrial | [x]  | [x]   |
| Avanzado       | [x]  | [x]   |

## Introducción al NLP: conceptos básicos

Estructuras básicas del lenguaje humano

- **Lingüística computacional (LC) {Ciencia}:** ¿Qué y cómo computan las personas?
- **NLP {Ingeniería}**

- **Texto** (Normalización de texto)
  - **Tokenización**: Consiste separar las frases en tokens unidades mínimas lingüísticas (palabras)
  - **Lematización**: Convertir cada una de las palabras en su raíz fundamental (Usar el verbo en forma infinitiva, sin conjugarlo)
  - **Segmentación**: Es separar el contenido en frases
- **Corpus** Colección de textos.
- **Corpora** Es una colección de colecciones de textos.

## :sunglasses: :point_right: El contenido del desarrollo del curso se ubica en los siguientes Notebooks

1. :one: :blue_book: [C3. Configuración quickstart](https://github.com/jocode/intro-NPL-python-NLTK/blob/master/notebooks/C3_Configuración_quickstart.ipynb)

2. :two: :green_book: [C4 Text Vocab Statistics](https://github.com/jocode/intro-NPL-python-NLTK/blob/master/notebooks/C4_text_vocab_statistics.ipynb)

3. :three: :ledger: [C5 Language with statistics](https://github.com/jocode/intro-NPL-python-NLTK/blob/master/notebooks/C5_Language_with_statistics.ipynb)

4. :four: :orange_book: [C6 Lexical Resources](https://github.com/jocode/intro-NPL-python-NLTK/blob/master/notebooks/C6_Lexical_Resources.ipynb)

5. :five: :closed_book: [C7 Processing raw text](https://github.com/jocode/intro-NPL-python-NLTK/blob/master/notebooks/C7_Processing_raw_text.ipynb)

## Qué es un N-grama?

Es una secuencia de palabras

- Bi-gramas (Estoy, aprendiendo)
- Tri-gramas (Estoy, aprendiendo cosas)

> Las colocaciones de una palabra son sentencias que indican los lugares que acostumbra a tomar esa palabra en el lenguaje (Sin seguir las reglas del lenguaje)...  
> _Firth (1957), Modes in Meaninf - Paper in Linguistics_

**Colocaciones**

- Le dieron ganas de dormir
  _vs_
- Le introdujeron ganas de dormir

## Introducción a los recursos léxicos

**¿Qué es un recurso léxico?**

Colecciones de palabras o frases con meta-datos

Los significados de las palabras son distintos

- Le puedes decir que se _calle_ o me va a enloquecer...
- Ten cuidado al cruzar la _calle_ porque el semáforo no funciona

## Introducción a WordNet

> Es una base de datos con caráter léxico para el idioma inglés. Se compone por conjuntos de sinónimos (**synsets**), cada uno expresando un concepto diferente. Diferentes synsets se relacionan por su relación semántica.

**Cómo es un synset**

Carro, Automovil, Auto, Coche = Vehículo motorizado de 4 ruedas, propupulsado por un motor.

La base de datos de WordNet tiene una base de datos en forma de grafos.

- **Hipónimo**: Conjunto se sinonimos
