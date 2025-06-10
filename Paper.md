

## Autores
Giuliana Herrera López - A01562646, Maria Ramirez - A01562798,
Salvador Alejandro Robles Hernández - A01562588

## 1. Introducción
<div style="text-align: justify;"

  En el ámbito del desarrollo de software, existen productos de carácter internacional cuyas interfaces suelen estar escritas en inglés debido a su amplio uso en el mercado global. Sin embargo, al buscar mejorar la experiencia del usuario, muchas empresas optan por implementar traducciones en sus productos para adaptarse a un público más amplio y diverso.No obstante, este enfoque presenta un desafío significativo: la necesidad de crear y traducir múltiples plantillas para cada idioma en el que se desee ofrecer el producto. Este proceso incrementa notablemente la complejidad del desarrollo del proyecto, tanto en términos técnicos como organizativos.Uno de los principales desafíos que existen en los software de venta internacional son las traducciones de las interfaces. Actualmente, el 50% del contenido en internet está en inglés (Statista, n.d.); sin embargo, solo el 20% de la población mundial habla este idioma, lo que puede representar una barrera para el acceso a la información para quienes no lo dominan, como también para empresas que ofrezcan sus servicios a otros países, esto puede ser una desventaja al solo cubrir los lenguajes más “comunes”.  Sin embargo,  también se encuentran traducciones automáticas en navegadores, pero en muchos de los casos estos navegadores no soportan todas las lenguas o tienden a tener errores semánticos dentro de las traducciones.  Adicionalmente, la ambigüedad intrínseca de los lenguajes, que son las frases o palabras con múltiples significados, requieren un contexto semántico de las palabras y de donde se encuentran. 

  De acuerdo a la revisión a la investigación sobre la traducción automática el uso de la IA ha evolucionado significativamente en la última década abriendo nuevas posibilidades para la traducción, aunque persisten desafíos claves. Estudios recientes destacan que, a pesar del avance de los modelos basados en redes neuronales (RNN) y transformadores (Vaswani et al., 2017), la calidad de las traducciones sigue siendo inconsistente en idiomas con recursos limitados. Este problema se agrava en contextos técnicos, donde la ambigüedad léxica y la falta de datos de entrenamiento especializados generan errores semánticos críticos (Hutchins, 2020).
Ante la problemática descrita, se propone la investigación sobre el empleo de Large Language Models (LLMs) como posible solución para optimizar la calidad de las traducciones en sitios web. Así mismo estos modelos cuentan con la capacidad para analizar y procesar contextos complejos y adaptarse a las variaciones lingüísticas según el contexto en el que se encuentre, sin embargo pueden tener también alucinaciones por lo cual es de suma importancia el prompt que se genere para el modelo a utilizar y con esto determinar una evaluación es decir un valor de precisión al momento de generar las traducciones (Lin, 2024).

</div>

#### Redacción del estado del arte.

Este estudio examina los últimos avances de large language models,
destacando aplicaciones prácticas y direcciones futuras para la traducción de
lenguajes.
###
**_Nombre:_** _Multilingual Machine Translation with Large Language Models: Empirical
Results and Analysis_.
###
**_Autores:_** _‌ Zhu, W., Liu, H., Dong, Q., Xu, J., Huang, S., Kong, L., Chen, J., & Li, L. _
###
**_Fuente:_** _Zhu, W., Liu, H., Dong, Q., Xu, J., Huang, S., Kong, L., Chen, J., & Li, L. (2023). Multilingual Machine Translation with Large Language Models: Empirical Results and Analysis. ArXiv.org. https://arxiv.org/abs/2304.04675_
###
**Enfoques y Hallazgos.**
La literatura muestra a un crecimiento acelerado en el uso de large
language models (LLMs) como GPT-4 y ChatGPT para la traducción automática
multilingüe, especialmente mediante aprendizaje en contexto. A diferencia de
sistemas supervisados tradicionales como NLLB o Google Translate, los LLMs
exhiben una capacidad emergente para traducir más de 100 lenguas sin
necesidad de ajuste fino, logrando resultados competitivos en aproximadamente
el 40% de las direcciones de traducción evaluadas. Entre los hallazgos más
relevantes es que los LLMs pueden traducir incluso lenguas de bajos recursos
mediante ejemplos cruzados entre lenguas, y que la calidad de la traducción
mejora significativamente con el diseño adecuado de plantillas y ejemplos en el
prompt.


###
**Brechas Identificadas.**
###
● Limitaciones de contexto: Los LLMs aún enfrentan serias limitaciones al traducir lenguas con
escasa representación digital, mostrando un rendimiento inferior al
de modelos entrenados específicamente para esos contextos.
###
● Persisten riesgos de sesgo y errores críticos en contextos sensibles: los LLMs pueden generar traducciones incorrectas o culturalmente inapropiadas, especialmente en textos relacionados con salud, derecho o política. La literatura señala que estos errores no siempre son detectados por métricas automáticas como BLEU o COMET, lo que plantea desafíos en entornos donde la precisión y neutralidad son fundamentales.
###
**_Nombre:_** _How Good Are LLMs for Literary Translation, Really? Literary Translation
Evaluation with Humans and LLMs._
###
**_Autores:_** _‌ Zhang, R., Zhao, W., & Eger, S._
###
**_Fuente:_** _‌Zhang, R., Zhao, W., & Eger, S. (2024). How Good Are LLMs for Literary Translation, Really? Literary Translation Evaluation with Humans and LLMs. ArXiv.org. https://arxiv.org/abs/2410.18697_
###
**Enfoques y Hallazgos.**
El Articulo se enfoca en la evaluacion de la traduccion realizada por
LLMs en comparacion de traducciones humanas, este estudio evalua tres
esquemas con estudiantes y profesores evaluadores. Se enfoca en en 6
categorias: (1)Terminologia; (2) Precision; (3) Fluencia; (4) Estilo; (5) Convencion
Local; and (6) No Traduccion.
El enfoque de la forumula desarrollada con estas variables es poder definir una metrica de la precision de
la traduccion, si el resultado de la formula es un numero alto indicaria que la
traduccion no tiene una buena calidad. Asi mismo dentro de los hallgazgos
encontrados los LLMs han mejorado notablemente, las traducciones humanas siguen siendo superiores en calidad literaria, especialmente en aspectos estilísticos y creativos. Además, el estudio demuestra que las evaluaciones humanas mediante esquemas simples como Best-Worst Scaling (BWS) son más eficaces que esquemas complejos como MQM, los cuales tienden a subestimar la calidad humana si son aplicados por evaluadores sin experiencia.
###
**Brechas Identificadas.**
###
● Limitaciones de los esquemas de evaluación actuales: El esquema MQM, aunque estándar para textos no literarios, se muestra inadecuado para evaluar traducciones literarias, especialmente cuando es usado por estudiantes sin experiencia. 
###
● Traducciones de LLMs excesivamente literales: A pesar de sus avances, los LLMs siguen generando traducciones más sintácticamente similares al texto fuente, pero con menos creatividad, diversidad y sensibilidad cultural aspectos esenciales en la traducción literaria.

###
**_Nombre:_** _Llama Guard: LLM-based Input-Output Safeguard for Human-AI Conversations_
###
**_Autores:_** _Hakan Inan; Kartikeya Upasani; Jianfeng Chi; Rashi Rungta; Krithika Iyer; Yuning Mao; Michael Tontchev; Qing Hu; Brian Fuller; Davide Testuggine; Madian Khabsa._
###
**_Fuente:_** _Inan, H., Upasani, K., Chi, J., Rungta, R., Iyer, K., Mao, Y., Tontchev, M., Hu, Q., Fuller, B., Testuggine, D., & Khabsa, M. (2023). Llama Guard: LLM-based Input-Output Safeguard for Human-AI Conversations. ArXiv.org. https://arxiv.org/pdf/2312.06674_
###
**_Enfoques y Hallazgos._**  
El artículo introduce un enfoque innovador para la moderación de contenido en conversaciones humano-IA mediante el uso de un modelo de lenguaje grande (LLM) especializado. A diferencia de herramientas tradicionales como OpenAI Moderation API, Llama Guard distingue entre la evaluación de riesgos en entradas de usuarios y sus respuestas, utilizando una taxonomía detallada de riesgos de seguridad. El modelo fue afinado con un conjunto de datos cuidadosamente anotado y demuestra una alta precisión en benchmarks como ToxicChat y el conjunto de evaluación de moderación de OpenAI, destacándose especialmente por su capacidad de adaptación mediante técnicas de zero-shot y few-shot prompting.

Aunque Llama Guard muestra adaptabilidad, su rendimiento y cobertura podrían verse comprometidos en idiomas distintos al inglés, ya que tanto el preentrenamiento como el afinamiento del modelo se realizaron exclusivamente en inglés. Esto limita su aplicabilidad en contextos multilingües, una característica crítica en herramientas de moderación globales.

###
**_Brechas Identificadas._**  
● ¿Qué estrategias de preentrenamiento y afinamiento multilingüe (por ejemplo, traducción automática, datos anotados en otros idiomas o ajustes de prompt) son más efectivas para garantizar que Llama Guard mantenga su desempeño en contextos distintos al inglés?

###
**_Nombre:_** _GenTranslate: Large Language Models are Generative Multilingual  Speech and Machine Translators_
###
**_Autores:_** _Yuchen Hu, ChenChen, Chao-HanHuckYang, Ruizhe Li, Dong Zhang,  Zhehuai Chen,  EngSiongChng._
###
**_Año:_** _2024_
###
**_Fuente:_** _Hu, Y., Chen, C., Yang, C. H., Li, R., Zhang, D., Chen, Z., & Chng, E. S. (2024, 10 febrero). GenTranslate: Large Language Models are Generative Multilingual Speech and Machine Translators. arXiv.org. https://arxiv.org/abs/2402.06894_

###
**_Enfoques y Hallazgos:_**

Este artículo científico propone GenTranslate, un paradigma de IA generativa para traducción automática que aprovecha las capacidades de los modelos de lenguaje (LLMs) mediante un innovador proceso de fusión de hipótesis múltiples. A diferencia de los sistemas convencionales que seleccionan una única mejor traducción (top-1), este método recibe como entrada la lista N-best hypotheses (las N traducciones más probables generadas por el modelo base, ordenadas por puntuación), sintetiza estas variantes mediante razonamiento lingüístico con LLM para luego generar una traducción final enriquecida. 

Los experimentos validan el enfoque en benchmarks estándar de la industria, WMT (Conference on Machine Translation): La principal competencia académica para evaluación de traducción de texto (MT), donde se reportan mejoras de +4.7 puntos BLEU (métrica que compara la superposición de n-gramas entre la traducción automática y referencias humanas)

**Hallazgos clave:**  
- El sistema demuestra versatilidad al procesar traducción texto-a-texto entre idiomas.  
- Superioridad sobre métodos top-1 (los cuales eligen la traducción con mejor probabilidad) en 11 idiomas.  
- Escalabilidad a dominios especializados (ej. médico, legal)

###
**_Brechas identificadas:_**  
- Los LLMs (LLama2) en GenTranslate sólo se utilizan para integrar las hipótesis N-best generadas por el modelo base (SeamlessM4T), pero no participan directamente en la generación de traducciones.  
- ¿Representaría una desventaja el seguir esta arquitectura modular (GenTranslate + SeamlessM4T) a diferencia de las arquitecturas monolíticas para la integración de nuestro reto?

###
**_Nombre:_** _Machine Translation with Large Language Models: Prompting, Few-shot Learning, and Fine-tuning with QLoRA_
###
**_Autores:_** _Xuan Zhang, Kevin Duh,  Navid Rajabi, Philipp Koehn._
###
**_Año:_** _2023_
###
**_Fuente:_** _Zhang, B., Haddow, B., & Birch, A. (2023). Machine translation with large language models: Prompting, few-shot learning, and fine-tuning with QLoRA. Proceedings of the Eighth Conference on Machine Translation, 446-462. https://aclanthology.org/2023.wmt-1.43/_

###
**_Enfoques y Hallazgos:_**

El estudio destaca que el zero-shot prompting es el enfoque más viable para implementar APIs de traducción, debido a su bajo costo computacional y flexibilidad. Los experimentos revelan que, aunque el fine-tuning con QLoRA (que ajusta solo el 0.77% de los parámetros) logra mejoras significativas (+28.93 BLEU en francés-inglés), el prompting zero-shot permite obtener traducciones aceptables sin necesidad de datos etiquetados o ajustes específicos 1. Esto lo hace ideal para APIs que requieren escalabilidad y soporte multilingüe inmediato, especialmente en lenguajes con recursos limitados. Además, el trabajo demuestra que los LLMs pueden generar traducciones coherentes incluso sin ejemplos previos, aunque con menor precisión que métodos supervisados. 

###
**_Brechas identificadas:_**
- Aunque el zero-shot prompting funciona bien en idiomas con amplia representación en los datos de pre-entrenamiento (como inglés o francés), su rendimiento es irregular en lenguas minoritarias o con estructuras complejas, donde la falta de contexto bilingüe afecta la fluidez y exactitud.
- El estudio señala que la calidad de las traducciones zero-shot varía drásticamente según la formulación del prompt (instrucciones dadas al modelo), pero no ofrece una metodología estandarizada para optimizarlas. Esto deja una brecha crítica en la implementación práctica, donde prompts subóptimos pueden degradar los resultados.

###
**_Esquema Metodológico:_**

### **_Tipo de investigación:_**  
Mixta

### **_Técnica principal de recolección de datos:_**

**Evaluación cuantitativa:**  
Se emplean métricas automáticas (como BLEU, MQM, SQM, GEMBA-MQM) para obtener puntuaciones numéricas sobre la calidad de las traducciones generadas por diferentes modelos de LLM. Estas métricas permiten comparar el rendimiento entre modelos de forma objetiva y reproducible.

**Evaluación cualitativa:**  
Se utilizan anotaciones de errores y escalas de valoración por parte de evaluadores humanos (estudiantes y profesionales), quienes identifican aspectos estilísticos, literarios y de adecuación cultural que los sistemas automáticos no capturan. Esta información se obtiene mediante esquemas como Best-Worst Scaling (BWS), anotación libre y análisis por categorías (como estilo, fluidez, terminología).

La evaluación cuantitativa con métricas como BLEU y MQM permite identificar de forma sistemática en qué idiomas o estructuras los LLMs flaquean, señalando exactamente dónde falla el zero-shot prompting en lenguas minoritarias. Al mismo tiempo, el análisis cualitativo mediante Best-Worst Scaling y anotaciones humanas ofrece insights sobre cómo la formulación del prompt impacta la fluidez y la adecuación cultural, guiando la creación de plantillas estandarizadas que optimicen el diseño de prompts.

### **_Datos cualitativos:_**  
- Opiniones y juicios de evaluadores sobre el estilo, creatividad y adecuación de las traducciones.  
- Análisis de errores o decisiones de traducción no detectadas por los sistemas automáticos.  
- Argumentos sobre por qué una traducción humana puede ser mejor en términos literarios, corroborados con expertos.

### **_Datos cuantitativos:_**  
- Resultados de evaluaciones automáticas (BLEU, MQM score, SQM).  
- Estadísticas de preferencia de traducción (porcentaje de veces que se elige la traducción humana sobre la de IA).  
- Correlaciones entre métricas automáticas y evaluaciones humanas.  


## Referencias
  Capellini, R., Atienza, F., & Sconfield, M. (2024). Knowledge Accuracy and Reducing Hallucinations in LLMs via Dynamic Domain Knowledge Injection. https://doi.org/10.21203/rs.3.rs-4540506/v1
  
  ‌Zhang, R., Zhao, W., & Eger, S. (2024). How Good Are LLMs for Literary Translation, Really? Literary Translation Evaluation with Humans and LLMs. ArXiv.org. https://arxiv.org/abs/2410.18697
  
‌	Lin, Z. (2024). How to write effective prompts for large language models. Nature Human Behaviour, 8(4), 611–615. https://doi.org/10.1038/s41562-024-01847-2
‌Chen, Y., Arkin, J., Hao, Y., Zhang, Y., Roy, N., & Fan, C. (2024). PRompt Optimization in Multi-Step Tasks (PROMST): Integrating Human Feedback and Heuristic-based Sampling. ArXiv.org. https://arxiv.org/abs/2402.08702

  Matviienko, L., Khomenko, L., Denysovets, I., Horodenska, K., Nikolashyna, T., & Pavlova, I. (2024). Comparative Analysis of Online Translators in the Machine Translation System. Romanian Journal for Multidimensional Education / Revista Românească Pentru Educaţie Multidimensională, 16(3), 101–118. https://doi.org/10.18662/rrem/16.3/885
  
  Hu, Y., Chen, C., Yang, C. H., Li, R., Zhang, D., Chen, Z., & Chng, E. S. (2024, 10 febrero). GenTranslate: Large Language Models are Generative Multilingual Speech and Machine Translators. arXiv.org. https://arxiv.org/abs/2402.06894
  
  Naveed, H., Khan, A. U., Qiu, S., Saqib, M., Anwar, S., Usman, M., Akhtar, N.,
Barnes, N., & Mian, A. (2023). A Comprehensive Overview of Large Language
Models. ArXiv.org. https://arxiv.org/abs/2307.06435

  ‌Vaswani, A., Shazeer, N., Parmar, N., Uszkoreit, J., Jones, L., Gomez, A. N., Kaiser, L., & Polosukhin, I. (2017). Attention is all you need. arXiv:1706.03762. https://doi.org/10.48550/arXiv.1706.03762
  
  Huan, X., & Zhou, H. (2024). Integrating Advanced Language Models and Vector Database for Enhanced AI Query Retrieval in Web Development. International Journal of Advanced Computer Science and Applications, 15(6). https://doi.org/10.14569/ijacsa.2024.0150601
  
  Inan, H., Upasani, K., Chi, J., Rungta, R., Iyer, K., Mao, Y., Tontchev, M., Hu, Q., Fuller, B., Testuggine, D., & Khabsa, M. (2023). Llama Guard: LLM-based Input-Output Safeguard for Human-AI Conversations. https://arxiv.org/pdf/2312.06674

