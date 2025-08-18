<H1 align = "center"> Tarea 2 - ARQUITECTURAS DE COMPUTACIÓN </H1>

<P align = "center">
  <strong> David Santiago López Maldonado </strong></P>
 <P align = "center">
   <strong> Sistemas Digitales III </strong></P>
 <P align = "center">
   <strong> 15.08.2025 </strong></P>


   <img src="https://media1.giphy.com/media/v1.Y2lkPTc5MGI3NjExb2ZmZmR3Zm5jZmJ0MzBpODEwbW4wM3ltZHBuaWV6YWY2YTluMm1oeSZlcD12MV9pbnRlcm5hbF9naWZfYnlfaWQmY3Q9Zw/fdOA43sHFE6Pu/giphy.gif" width="1010"/>
</div>

## Introducción
  <P align = "justify">
    Por medio del siguiente documento se muestran diversas arquitecturas de computación que presentan un cambio importante frente a la computación clásica que aborda mayormente una arquitectura Von Neumann. Teniendo cinco (5) tipos de aarquitectura diferentes como lo son <strong> Computación cuántica </strong>, <strong> Computador neuromórfico </strong>, <strong> Ordenador biológico </strong>, <strong> Computación Heterogénea </strong> y <strong> Computación de borde </strong>.
  
  Cada uno de estos modelos presenta fundamentos, arquitecturas y aplicaciones diferentes, pero todos comparten el objetivo común de <em>mejorar el rendimiento, la eficiencia y la capacidad de procesamiento de la información</em> frente a los desafíos actuales de la tecnología. Asimismo, se explorarán sus ventajas, desventajas, principales hitos históricos y el estado actual de desarrollo, con el fin de comprender su potencial y limitaciones.
  
  </P>

## 1. Computación cuántica 💻⚛️
<p align = "justify">
  La computación cuántica aplica los conceptos físicos y matemáticos de la mecánica cuántica a la informática para poder procesar información de una forma mucho más rápida y eficiente que la computación clásica.<br/>
  
  En lugar de trabajar con **bits** que solo representan un estado o un nivel (_0 o 1_), la computación cuántica emplea **qubits**, es decir, bits cuánticos que gracias al estado de superposición pueden representar ambos estados o niveles (_0 y 1_) al mismo tiempo. Esta propiedad junto con algunas otras, permiten explorar y calcular varias soluciones o respuestas paralelamente. Todo esto como alternativa a problemas que los computadores tradicionales o supercomputadores no pueden resolver o tardan demasiado tiempo en resolverlos [2][3].

-![Computadora cuántica IBM](https://github.com/user-attachments/assets/b1b908d9-f8bb-4899-a17b-ff1778e21e5e)

  
  </p>
  
  - ### Arquitectura de un computador cuántico
    - ### Unidad de Procesamiento Cuántico (QPU):
      <p align = "justify">
        Esta unidad de procesamiento cuántico es análoga a la CPU de un computador tradicional, sin embargo, como se explicó antes, no se procesan bits comunes sino bits cuánticos (qubits) los cuales funcionan mediante fenómenos cuánticos como la <i> superposición </i> y el <i> entrelazamiento </i>. Estos procesadores son los encargados de realizar las operaciones cuánticas que se definieron mediante algoritmos cuánticos, incluyendo las compuertas cuánticas, que son las que alteran los estados de los qubits. Es también conocido como el corazón de la computadora, alberga los qubits y controla las operaciones que la máquina hará. <br/>
        <img width="1515" height="852" alt="QPU NVIDIA" src="https://github.com/user-attachments/assets/0895196c-638b-49bf-a43c-d82b589ea64b" />
  
        Los componentes de las QPU son los siguientes:     
      </p>
      <ul>
        <li>
          <strong> <ins> Qubits  </ins> </strong>: Son las unidades fundamentales de la computación cuántica. Son capaces de representar dos estados simultáneamente (0 y 1) mediante el fenómeno de superposición. <br/>
          Los qubits se pueden crear mediante tecnologías como: <br/>
          <ul>
            <li>
              <strong> <i> circuitos superconductores </i> </strong>: Son circuitos fabricados con materiales superconductores que están enfriados con una temperatura cercana al cero absoluto <strong> (0° k = -273.15° C = -459.63° F). </strong> <br/>
            </li>
            <li>
               <strong> <i> Iones atrapados </i> </strong>: Son átomos cargados suspendidos en trampas electroagnéticas. <br/>
            </li>
            <li>
               <strong> <i> Fotones </i> </strong>: Aprovechan parículas de luz para procesar información.<br/>
            </li>
            <li>
               <strong> <i> Puntos cuánticos </i> </strong>: Son nanoestructuras que aislan electrones. <br/>
            </li>
            <li>
               <strong> <i> Qubits de Espín </i> </strong>: Dependen del espín de los electrones o núcleos. <br/>
            </li>
          </ul>
          <li>
            <strong> <ins> Compuertas cuánticas </ins> </strong>: Análogas a las compuertas lógicas, las compuertas cuánticas manipulan qubits de formas controladas para poder realizar cálculos complejos y resolver problemas que serían imposibles de resolver con computadores convencionales.
          </li>
        <li>
          <strong> <ins> Interconexiones </ins> </strong>: Permiten la comunicación entre qubits y demás QPU para poder escalar los computadores cuánticos y realizar cálculos más complejos
        </li>
        </li>
      </ul>
       
    - ### Electrónica de control:
      <p align = "justify">
        Gestiona las operaciones del computador cuántico, genera y envía señales precisas (microondas, radiofrecuencia o láser) que manipulan los qubits y las compuertas cuánticas en la QPU, además sincronizan las operaciones para que  los resultados precisos sean garantizados. 
      </p>

    - ### Infraestructura de refrigeración:
       <p align = "justify">
          Para garantizar la coherencia de los qubits y minimizar el ruido térmico, es necesario que el computador se mantenga a temperaturas cercanas al cero absoluto. Este sistema está alimentado por refrigeradores de dilución que mantienen el hardware a temperaturas de unos 10mK-20mK y permiten el aislamiento del procesador al calor y al ruido. Estos refrigeradores funcionan mediante la mezcla de isótpos de Helio. Los aisladores criogénicos protegen la QPU de interferencias térmicas y del ruido externo. Los amplificadores criogénicos amplifican las señales débiles emitidas por los qubits para medirlas con precisión sin agregar ruido adicional.
        </p>

     - ### Infraestructura de corrección de errores cuánticos:
        <p align = "justify">
          Conocida como QEC (Quantum Error Correction), esta infraestructura se encarga de darle fiabilidad a los qubits, estos son demasiado sensibles a interferencias ambientales y a imperfecciones de la máquina. Los estados cuánticos de los qubits pueden degradarse rápidamente y esto conlleva a errores computacionales y entre mayor escalabilidad, mayor probabilidad de error, de ahí la justificación de esta infraestructura. <br/>
          Para evitar la alteración en los estados cuánticos de los qubits, los qubits lógicos se codifican en diferentes qubits fisicos, permitiendo la detección de errores. Los circuitos especializados detectan la ubicación de los errores y se aplica la corrección correspondiente como, por ejemplo, invertir los qubits para poder restaurar el qubit lógico.
        </p>
      - ### Interfaz de computación clásica:
        <p align = "justify">
          Esta interfaz de computación clásica controla el flujo de operaciones de la computadora cuántica, sirve como un puente entre lo convencional y lo cuántico. Es capaz de gestionar la entrada y salida de los cálculos cuánticos, asiste en las tareas como los cálculos de corrección de errores e interpreta los resultados de las mediciónes obtenidas.
        </p>
      - ### Interconexiones cuánticas:
        <p>
          Permiten las comunicaciones cuánticas y las redes cuánticas, son las responsables de transmitir información cuántica entre computadoras cuánticas. Son imporantes para la escalabilidad de estas computadoras y para permitir el procesamiento cuántico colaborativo en diferentes sistemas.
        </p>
 
  - ### Historia
    <p align = "justify">
      <ul>
        <li>
          <strong> 1900 - 1930 </strong> <br/>
          <ul>
            <li>
              <p align = "justify">
            <strong> <i> 1900 </i> </strong> ➡️ Max Planck descubrió que la energía es emitida y absorbida por paquetes discretos llamados "quanta", esto solucionó el problema de radiación de cuerpo negro que los físicos aún no podían entender. Además, desafió la fisica clásica al introducir la discresión a escala atómica, dando como origen la teoría cuántica. <br/>
              </p>
            </li>
            <li>
              <p align = "justify">
                 <strong> <i> 1913 </i> </strong> ➡️ Niels Bohr desarrolló un modelo atómico en donde postulaba que los electrones se movían en niveles específicos y cuantificados de energía. Explica el por qué los átomos, en longitudes de onda específicas absorben y emiten luz (Fotones con cantidades precisas de energía). <br/>
              </p>
            </li>
            <li>
              <p align = "justify">
                <strong> <i> 1925-1926 </i> </strong> ➡️ La mecánica matricial fue desarrollada por Werner Heisenberg, la mecánica ondulatoria formulada por Erwin Schrödinger. Por medio de estos marcos matemáticos se estableció la mecánica cuántica moderna, que establece que las partículas están en una dualidad de <i>onda-partícula</i>, siguiendo el principio de <strong>incertidumbre</strong> y sentando las bases para la computación cuántica.
              </p>
            </li>
          </ul>
        </li>
        <li>
          <strong> 1930 - 1940 </strong>
          <ul>
            <li>
              <strong> <i> 1935 </i> </strong> ➡️ Einstein, Podolsky y Rosen publicaron un experimento mental en el que se destacó el fenómeno de <strong>entrelazamiento cuántico</strong>, recurso que se volvió fundamental en la computació cuántica. <br/>
            </li>
            <li>
              <strong> <i> 1939 </i> </strong> ➡️ Isidor Rabi mostró cómo pueden cambiar los estados cuánticos de un núcleo atómico mediante ondas de radio por medio de la Resonancia Magnética Nuclear. Esta técnica fué la primera en poder controlar los estados cuánticos mediante radiación electromagnética, estableciendo los principios que evolucionaron en métodos capaces de manipular los qubits empleados en las computadoras cuánticas. <br/>
            </li>
          </ul>
        </li>
        <li>
          <strong> 1950 - 1970 </strong>
        </li>
        <ul>
          <li>
            <strong> <i> 1952 </i> </strong> ➡️ Félix Bloch y Edward Mills Purcell desarrollaron métodos precisos que permitieron a los científicos observar precisamente las propiedades cuánticas de los átomos. Esto permitió establecer herramientas experimentales esenciales para el estudio y manipulación de los sistemas cuánticos. <br/>
          </li>
          <li>
            <strong> <i> 1965 </i> </strong> ➡️ El teorema de Bell proporcionó el marco para eventuales experimentos que confirmarían la naturaleza no local del entrelazamiento y cuestionarían nuestra comprensión fundamental de la realidad. <br/>
          </li>
          <li>
            <strong> <i> 1972 </i> </strong> ➡️ Alain Aspect, a inicios de los años 80, realizó experimentos que confirmaron el entrelazamiento cuántico, validando la <i>acción fantasmal a distancia</i> propuesta por la mecánica cuántica. Sus hallazgos sentaron bases fundamentales para el desarrollo de la computación cuántica. <br/>
          </li>
        </ul>
        <li>
          <strong> 1980 - 1990 </strong>
        </li>
        <ul>
          <li>
            <strong> <i> 1981 </i> </strong> ➡️Richard Feynman propuso que solo las computadoras cuánticas podían simular eficazmente sistemas cuánticos, planteando que resolverían ciertos problemas mucho más rápido que las clásicas y estableciendo las bases teóricas de la computación cuántica.
          </li>
          <li>
            <strong> <i> 1983 </i> </strong> ➡️ Alain Aspect confirmó experimentalmente las violaciones de la desigualdad de Bell, demostrando de forma definitiva la realidad del entrelazamiento cuántico y consolidando su papel como base para la computación cuántica.
          </li>
          <li>
            <strong> <i> 1985 </i> </strong> ➡️ David Deutsch formuló el primer modelo teórico de una computadora cuántica universal, mostrando que las puertas cuánticas podían realizar cualquier cálculo cuántico. Con ello extendió la computación universal al ámbito cuántico y planteó la posibilidad de resolver problemas imposibles para las computadoras clásicas.
          </li>
          <li>
            <strong> <i> 1994 </i> </strong> ➡️ Peter Shor creó un algoritmo de factorización cuántica que resolvía grandes números mucho más rápido que los métodos clásicos, demostrando la ventaja práctica de la computación cuántica y generando gran impacto en la criptografía y en la inversión en este campo.
          </li>
          <li>
            <strong> <i> 1995 </i> </strong> ➡️ El NIST demostró experimentalmente la primera puerta cuántica controlada-NOT (CNOT), validando la posibilidad física de operaciones básicas entre cúbits y marcando el paso de la teoría a la implementación práctica de circuitos cuánticos.
          </li>
        </ul>
        <li>
          <strong> 2000 - Presente </strong>
        </li>
        <ul>
          <li>
            <strong> <i> 2001 </i> </strong> ➡️ Georges-Olivier Reymond y otros científicos demostraron el uso de pinzas ópticas para atrapar átomos neutros individuales, logrando un control cuántico preciso partícula por partícula. Este avance abrió una nueva plataforma para el procesamiento de información cuántica y dio origen a la tecnología de Pasqal.
          </li>
          <li>
             <strong> <i> 2011 </i> </strong> ➡️ D-Wave One (128 qubits) se convierte en la primera computadora cuántica disponible comercialmente
          </li>
          <li>
            <strong> <i> 2016 </i> </strong> ➡️ IBM ofrece acceso público a computación cuántica vía su plataforma en la nube (IBM Quantum Experience), democratizando el acceso a hardware cuántico experimental.
          </li>
          <li>
            <strong> <i> 2016 </i> </strong> ➡️ 2019 – Google, en colaboración con NASA, anuncia la consecución de la supremacía cuántica con su procesador de 54 qubits, al ejecutar una tarea que afirmaban sería impracticable para computadoras clásicas. IBM refutó parte de esta afirmación, generando debate científico.
          </li>
          <li>
            <strong> <i> 2018-2025 </i> </strong> ➡️ Esta fase se conoce como la era NISQ (Noisy Intermediate-Scale Quantum), caracterizada por dispositivos con hasta ~1000 qubits, aunque aún sin corrección de errores completa. John Preskill acuña el término en 2018, y en 2023 se supera la barrera de los 1,000 qubits físicos (Atom Computing, 1,180 qubits)
          </li>
        </ul>
      </ul>
    </p>

    
  - ### Ventajas y desventajas
<p align = "center" >

| **Ventajas**                                                                 | **Desventajas**                                                                 |
|------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| 🚀 Velocidad y eficiencia en ciertos problemas: resolución exponencialmente más rápida que en computadores clásicos. | ⚠️ Fragilidad de los cúbits: muy sensibles al ruido y la decoherencia.           |
| 🧪 Simulación precisa de sistemas cuánticos: moléculas, materiales y reacciones químicas. | ❄️ Necesidad de condiciones extremas: refrigeración casi al cero absoluto.      |
| 🔎 Optimización avanzada en logística, finanzas, energía y telecomunicaciones. | 📉 Escalabilidad limitada: actualmente solo decenas o cientos de cúbits.        |
| 🔐 Criptografía cuántica: desarrollo de comunicaciones ultra seguras (QKD).   | 💰 Altos costos y complejidad técnica en infraestructura y mantenimiento.       |
| 🌐 Posibilidad de resolver problemas inalcanzables para supercomputadores clásicos. | 🔓 Riesgo para la seguridad actual: amenaza a los sistemas criptográficos clásicos (RSA, ECC). |
|                                                                              | 🧪 Madurez tecnológica insuficiente: aún en fase experimental con aplicaciones limitadas. |

</p>

  - ### Conceptos clave
    <ul>
      <li>
        <ins> <i> Superposición </i> </ins>
        <p align = "justify">
          Habla de la capacidad de una particula de estar en más de un estado al mismo tiempo. <br/>
          🪙 Imaginemos una moneda lanzada al aire: mientras está girando, no es solo cara o sello, sino una mezcla de ambos. Cuando cae al piso (cuando se mide), se convierte en un resultado concreto.
        </p>
      </li>
      <li>
         <ins> <i> Entrelazamiento </i> </ins>
        <p align = "justify">
          Establece que, sin importar la distancia, dos partículas cuánticas pueden conectarse de tal forma que lo que le sucede a una, instantáneamente afecta a la otra. <br/>
          🛣️ Si entrelazamos dos monedas cuánticas y una resulta "cara", automáticamente la otra será "sello", incluso si están separadas por kilómetros.
        </p>
      </li>
      <li>
         <ins> <i> Interferencia cuántica </i> </ins>
        <p align = "justify">
          Al estar las partículas en el estado de superposición, los posibles estados pueden sumarse o anularse, esto permite crear algoritmos que favorezcan respuestas o resultados correctos. <br/>
          🌊 Pensemos en dos olas de agua: si coinciden, se refuerzan (interferencia constructiva); si están opuestas, se cancelan (interferencia destructiva).
        </p>
      </li>
      <li>
         <ins> <i> Medición probabilística </i> </ins>
        <p align = "justify">
          Al tomar la medición de un qubit en estado de superposición, su medición no es concreta sino se determina por probabilidad. Esto explica el por qué es necesario repetir muchas veces los algoritmos cuánticos para obtener un resultado confiable. <br/>
          📈 un cúbit puede estar en 70% de probabilidad de ser 0 y 30% de ser 1. Al medirlo, el resultado será 0 la mayoría de veces, pero a veces será 1.
        </p>
      </li>
      <li>
         <ins> <i> Desafío de decoherencia </i> </ins>
        <p>
          Sucede cuando un qubit pierde su estado cuántico debido a interacciones con el ambiente, ya sea ruido, calor o radiación. <br/>
          ⁉️ Es como si la moneda en el aire fuera golpeada por el viento antes de caer: ya no refleja la verdadera probabilidad, sino un error.
        </p>
      </li>
      <li>
         <ins> <i> Tipos de comunicación cuántica </i> </ins>
        <ul>
          <li>
            <p align = "justify">
              <ins> Distribución cuántica de claves </ins>: Esta distribución usa entrelazamiento para generar claves criptográficas imposibles de detectar.
            </p>
          </li>
          <li>
            <p align = "justify">
              <ins> Teletransportación cuántica </ins>: transmite el estado cuántico de una partícula a otra distante, usando entrelazamiento, aunque la partícula en sí no viaja.
            </p>
          </li>
          <li>
            <p align = "justify">
              <ins> Redes cuántica </ins>: Es la idea de un “Internet cuántico” basado en cúbits entrelazados.
            </p>
          </li>
        </ul>
        🏛️ La Universidad de Delft, en Países Bajos, logró en 2022 transmitir información cuántica entre tres nodos distintos usando entrelazamiento.
      </li>
      <li>
         <ins> <i> Compuertas cuánticas </i> </ins>
        <p align = "justify">
          Análogas a las compuertas lógicas clásicas, las compuertas cuánticas manipulan los qubits según un algoritmo o circuito. <br/>
          - <strong> X gate <i>(NOT cuántico)</i> </strong>: invierte el estado del qubit. <br/>
          - <strong> H gate <i>(Hadamard)</i> </strong>: Coloca a los qubits en estado de superposición. <br/>
          - <strong> CNOT <i>(Controlled-NOT)</i> </strong>: genera entrelazamiento, cambia el segundo cúbit solo si el primero es 1. <br/>
        </p>
        ⚛️ Si tenemos dos cúbits: El primero = 1, El segundo = 0. Después de pasar por una CNOT ➡️ el segundo se convierte en 1.
      </li>
    </ul>
## 2. Computador Neuromórfico


# Referencias
1. [Sintáxis de escritura y formato básicos](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
2. [Listas en HTML](https://www.mclibre.org/consultar/htmlcss/html/html-listas.html)
3. [¿Qué es la computación cuántica? IBM](https://www.ibm.com/es-es/topics/quantum-computing)
4. [¿Qué es la computación cuántica? AWS](https://aws.amazon.com/es/what-is/quantum-computing/)
5. [¿Cómo es una computadora cuántica? - La estructura física de una computadora cuántica](https://www.spinquanta.com/news-detail/what-does-a-quantum-computer-look-like-explain-key-parts20250116063551+)
6. [Quantum Computing History: Path to Pasqal](https://www.pasqal.com/quantum-computing-history-path-to-pasqal/#1900s)
7. [Quantum Computing: a Timeline](https://www.btq.com/blog/quantum-computing-a-timeline)
8. [History of Quantum computing](https://www.livescience.com/technology/computing/history-of-quantum-computing-key-moments-that-shaped-the-future-of-computing)
