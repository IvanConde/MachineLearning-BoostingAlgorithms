![INFORME COMPLETO](Informe.pdf)

# Objetivo

El objetivo  es resolver un problema de machine learning con los datos del TP1. Puntualmente, se debe predecir la variable `damage_grade` que representa el nivel de daño recibido por la edificación. El error de la solución se calculará con la métrica F1 Score, particularmente con la variación no binaria micro averaged F1 score.

Podríamos pensar que una opción alternativa de métrica para el error sería promediar los F1 Score individuales de cada clasificación. El promedio de eso nos daría una métrica llamada macro-F1-score, que daría igual relevancia a todas los F1-score por igual sin importar su peso en la estimación.
 Ej: supongamos que F1-grade-1 = 50%; F1-grade-2 = 62% y F1-grade-3 = 34%. Macro-F1 = 48,66% 

La alternativa utilizada para el ejercicio,  micro-F1-score,  pone más énfasis en los labels más comunes logrando de esta manera que aquellos labels poco comunes no afecten a la métrica general. Se deja el siguiente paper para aquellos interesados en leer con más profundidad al respecto.

El ejercicio se desarrollará en el contexto de una competencia de Driven Data. Para esto deben tener dos conjuntos de datos:

El de entrenamiento `Train Values` con sus respectivos labels `Train Labels`, sobre el cual ajustarán su/s modelo/s junto con sus hiperparámetros.

El de test `Test Values`, sobre el cual realizarán predicciones y subirán los resultados a Driven Data. El score estará dado por la ecuación anterior.

También contarán con un modelo de submission que deberán respetar.

## Trabajo esperado

Se espera que armen un pipeline completo de machine learning experimentando en cada etapa. Esto quiere decir:

Realizar feature engineering, encontrando codificaciones que sirvan, generando nuevos atributos, analizando cuáles atributos aportan y cuáles no.

Probar modelos predictivos que crean que se encuadran al problema. Esto puede incluir realización de ensambles, también.

Búsqueda de hiperparámetros óptimos de alguna manera automatizada.

Como sugerencia, recomendamos realizar una primera versión de cada etapa y que luego vayan en profundidad en cada una.

Además de los aspectos funcionales del código, también esperamos que trabajen de manera científica. Esto implica:

Plantear preguntas o hipótesis y responderlas con experimentos y resultados. Las cosas no se hacen por que sí; debe haber una motivación basada en el conocimiento.

Trabajo en equipo. Entendemos que la virtualidad y la asincronía complican la comunicación, pero en cualquier trabajo científico, en particular en los trabajos de aprendizaje automático, es fundamental la difusión de conocimiento entre las personas. Esto evita la redundancia de experimentos, genera un trabajo más cohesivo y hace que cada integrante tenga una visión más completa del problema.

Realizar un poco de investigación del problema. En los apuntes de la materia, en las bibliotecas del lenguaje que utilizan, en internet. Esto no implica probar cosas a mansalva y sin criterio -- como mencionamos antes, debe haber una motivación o justificación.

Interpretación de los resultados. Una vez que se realiza un experimento hay que considerar si funcionó como fue esperado o no y por qué. Los resultados negativos también son resultados. Es parte de la interpretación entender el problema en específico y encuadrar bien la solución.

Presentación. Cualquier trabajo en ingeniería o ciencia requiere de una presentación a los colegas. Como pares de ustedes, esperamos que la comunicación que hagan del proceso y de los resultados se sustente en argumentos, datos y gráficos.
