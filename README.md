Integrantes:
* Ana Laura Flores Barcenas
* Carlos Perez Garcia
* Christian Jesus Pacheco Robles
* Keylie Gonzales Soberanis

## Leer comentarios en codigo y documentacion en readme.

### ¿Qué hicieron ?(descripción del proyecto)
- Se tuvo que realizar un proyecto donde teniamos que hacer una calculadora funcional, entre los 4 integrantes pusimos a prueba a la inteligencia artificial para realizar una calculadora funcional y sobre todo con un proyecto un poco grande para hacerlo en Pseint (que solo esta adaptado para programacion baja y como introduccion a la programaccion) es por eso que nos sucedio lo siguiente en este trabajo...
- El objetivo era crear una **Calculadora Multifuncional** que integrara cuatro módulos principales: **1) Operaciones Aritméticas Básicas**, **2) Cálculo de Áreas Geométricas y Dimensiones (Radio/Diámetro)**, **3) Estadística Básica (Media, Mediana, Moda)** y **4) Generación de la Sucesión de Fibonacci**. Este proyecto sirvió como prueba de fuego para evaluar las limitaciones de PSeInt y la eficacia de la ingeniería de prompts en proyectos de mediana complejidad.

  ### ¿Cómo lo hicieron?(explicación de la arquitectura y lógica)
- Nosotros como tal ya teniamos en mente como se tenia que realizar nuestro proyecto (codigo en mente) pero pusimos a prueba a la IA para ver su comportamiento real en un proyecto un poco mas riburoso para un editor de codigo tal vez no tan "rudo"
- Empezamos con varios prompt detallados y tratando de estimular la IA para nuestro codigo pero al ver que no seguia con la logica que nosotros queriamos decidimos tomar un poco de logica al usar una IA.
- Nuestra idea fue : Pedir en diferentes chats de la IA todo lo que conlleva la calculadora pero *Por partes*.
- Tuvimos muy buenos resultados despues de esta idea asi que seguimos haciendo esto para todo el proyecto.
- Despues de pedir todo por partes tuvimos que probar cada uno de los resultados que nos habia dado de codigo y nos dimos cuenta que si ponemos un prompt mas sencillo de poder leer para la IA lo dara mucho mejor.
- Al terminar con esto juntamos todos los resultados para pedir un prompt que juente todo para crear un solo codigo.
- La IA logro entender y realizar bien su trabajo.
- Solamente, lo poco que tuvimos que hacer en este punto del trabajo es usar un poco mas de logica y pedir algunas mejores sencillas.
- Le costo un poco mejorar el codigo pero pudo lograrlo al final.
- Al finalizar ya en este mismo repositorio estamos terminando la documentacion de nuestro trabajo.
- Desde el punto de vista arquitectónico, la solución final adoptó una estructura **Modular (SubProceso)** para aislar la lógica de cada función (Aritmética, Geometría, Estadística, Fibonacci). Esta decisión de diseño fue clave para manejar la extensión del código y mejorar la legibilidad, resolviendo el problema de un código monolítico que era propenso a errores. La lógica central del programa sigue un patrón de **Menú Principal de Control de Flujo (REPETIR... HASTA QUE y SEGÚN)** para redirigir al usuario al módulo deseado.

### ¿ Para qué lo hicieron? (propósito de cada módulo/función)
- Entendimos facilmente el codigo de la IA y la funcionalidad de cada modulo, el codigo sin problemas puede ser modificado por alguno de nosotros o por cualuier desarrollador exterior que quiera "jugar" o experimentar con nuestro proyecto.
- Pensamos que cada modulo es facil de saber usar ya que pensamos mucho en que el usuario nuca se pierda en el menu.
- Nuestro objetivo principal es hacer algo sencillo pero entendible.
- El usuario puede abrir el programa, puede navegar en el, puede hacer operaciones "basicas" y mientras se va desplazando en el codigo sentimos que es tan sencillo que jamas podria hacerlo.
- El propósito de cada módulo es el siguiente:
    * **Operaciones Básicas:** Garantizar cálculos aritméticos robustos e incluir el manejo de la **excepción de División por Cero**, un requisito fundamental de la programación defensiva.
    * **Cálculo Geométrico:** Centralizar el uso de constantes (como PI) y aplicar **validación de entradas** para asegurar que las dimensiones (radio, bases, altura) sean siempre positivas, evitando resultados anómalos.
    * **Estadística Básica:** Demostrar la manipulación de estructuras de datos (arreglos) y la implementación de algoritmos de **ordenamiento (Burbuja)**, necesarios para calcular correctamente la Mediana y la Moda.
    * **Sucesión de Fibonacci:** Implementar la lógica de la sucesión de manera fiel, utilizando ciclos (WHILE y PARA) para generar términos basándose en una entrada inicial definida por el usuario.
  
### ¿Qué dificultades encontraron y cómo las resolvieron?
- La IA no respondio bien al prompt COMPLETO de nuestro proyecto, buscamos màs inteligencias artificiales para realizar este proyecto pero volvia el mismo problema que al inicio, no entendian y menos si eran estimuladas con prompt mas detallados.
- Las inteligencias artificiales no encontraban muchas veces los errores que ellas mismas cometieron en algun codigo.
- Nos dimos cuenta que Pseint no es para u codigo muy extenso o se tiene que saber muy a detalle la logica ya que comete errores o tiene pequeños detalles que no los tiene un lenguaje como C++ que es mas facil realizar trabajos como este tipo.
- La principal dificultad técnica, que provocaba que el programa "se cerrara" o fallara, fue la extensión del código dentro de un único proceso en PSeInt.
- **Resolución:** La solución arquitectónica implementada fue la **modularización exhaustiva** (separando en SubProcesos) combinada con el uso sistemático de **validación de entradas** (`REPETIR... HASTA QUE`) en cada módulo. Esto aseguró que el programa no colapsara por lógica incorrecta o por entradas fuera de rango. La dificultad con la IA se resolvió con la estrategia de **Ingeniería de Prompts Simples y Segmentados** y la posterior **depuración y ensamblaje manual** del código.
