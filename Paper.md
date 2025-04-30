

## Autores
Giuliana Herrera López, A01562646
Maria Ramirez, A01562798
Salvador Alejandro Robles Hernández, A01562588

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

