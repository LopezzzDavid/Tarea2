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
  
  <p align = "justify">
    Un computador neuromórfico (también llamado ingeniería neuromórfica) es un sistema de hardware y software diseñado para imitar el funcionamiento del cerebro humano. Integra elementos inspirados en neuronas y sinapsis reales, y procesa información de forma distribuida, paralela y altamente eficiente. <br/>
    Este enfoque busca superar limitaciones de la arquitectura tradicional de von Neumann, especialmente en términos de consumo de energía y latencia.
  </p>

  - ### Arquitectura de un computador neuromórfico
    <ul>
      <li>
        <strong> Entrada y codificación sensorial </strong>
        <p align = "justify">
          Son módulos que toman señales externas como imagen, audio, etc, y las convierten en <i> eventos (o spikes) </i> en lugar de cuadros continuos de datos. Esto reduce datos y latencia, solo emite algo cuando cambia la escena. Por ejemplo, cámaras de eventos (DVS) generan un evento por pixel cuando detectan un cambio de luminancia; si nada cambia, no emiten casi nada. <br/>
        </p>
      </li>
      <li>
        <strong> Núcleos neurosinápticos </strong>
        <p align = "justify">
          Agrupa las neuronas y sus sinapsis. Cada núcleo recibe spikes en axones (entradas), los pondera con una matriz sináptica y actualiza el estado de cada neurona; cuando una neurona supera umbral, emite un spike a la red.
        </p>
      </li>
      <li>
        <strong> Motor de plasticidad </strong>
        <p align = "justify">
          Es la lógica cerca de las sinapsis que actualiza pesos con reglas locales (por ejemplo, STDP, refuerzo, aprendizaje hebbiano). Permite aprendizaje on-chip sin ir a CPU externa, manteniendo el procesamiento en memoria y event-driven
        </p>
      </li>
      <li>
        <strong> Memoria sináptica y representación de pesos </strong>
        <p lign = "justify">
          Es dónde viven los pesos y metadatos (retrasos, “tipo de axón”, etc.). Suele ser SRAM distribuida por núcleo; en plataformas analógicas/memristivas puede ser NVM.dónde viven los pesos y metadatos (retrasos, “tipo de axón”, etc.). Suele ser SRAM distribuida por núcleo; en plataformas analógicas/memristivas puede ser NVM.Habilita el cómputo en memoria: el acceso a los pesos ocurre localmente para cada spike, sin tráfico a DRAM externo.
        </p>
      </li>
      <li>
        <strong> Red de interconexión </strong>
        <p align = "justify">
          Es la “malla” que transporta spikes como paquetes ligeros con la dirección del emisor o del destino: Address-Event Representation (AER). Enruta spikes de forma asíncrona y multicast (un spike se copia a muchos destinos), escalando a redes grandes con baja latencia.
        </p>
      </li>
      <li>
        <strong> Clúster neuromórfico </strong>
        <p align = "justify">
          Son topologías multi-chip/multi-nodo con routers de alto fan-out y encaminamiento tolerante a fallos. Permite simular/controlar redes neuronales masivas en tiempo biológico.
        </p>
      </li>
      <li>
        <strong> Temporización y ejecución asíncrona </strong>
        <p align = "justify">
          Muchos diseños evitan un reloj global; las actualizaciones ocurren al arribo de eventos o por clocks locales. Esto reduce consumo (no hay conmutación si no hay eventos) y elimina cuellos de botella de sincronización global.
        </p>
      </li>
      <li>
        <strong> Control y monitorización </strong>
        <p align = "justify">
          Son microcontroladores/cores de servicio que cargan configuraciones, inician experimentos, colectan métricas y comunican con el host. Esto orquesta el sistema sin intervenir en el tráfico fino de spikes.
        </p>
      </li>
      <li>
        <strong> Software y mapeo </strong>
        <p align = "justify">
          Son toolchains para compilar/redesplegar SNNs a núcleos (particionado, asignación de neuronas/sinapsis, ruteo). Traduce modelos (por ejemplo, PyNN/Loihi API) a configuraciones de hardware cumpliendo límites de fan-in/fan-out, memoria y latencias.
        </p>
      </li>
    </ul>

    Es decir que: Un sensor/event-encoder convierte señales en spikes. ▶️ Los spikes entran a un núcleo; la crossbar/tabla sináptica suma entradas, actualiza neuronas y emite nuevos spikes. ▶️ La NoC/AER reenvía esos spikes (multicast) a otros núcleos/chips. ▶️ Si hay plasticidad, el motor local ajusta pesos en tiempo real. ▶️ Los cores de control orquestan, miden y comunican con el host.
    
  - ### Ventajas y Desventajas
    <p align = "center">

| **Ventajas**                                                                 | **Desventajas**                                                                 |
|------------------------------------------------------------------------------|---------------------------------------------------------------------------------|
| ⚡ **Alta eficiencia energética**: consumen mucho menos que los computadores tradicionales para tareas de IA. | 🛠️ **Tecnología inmadura**: aún en fase de investigación y desarrollo, con aplicaciones limitadas. |
| 🧠 **Procesamiento paralelo masivo**: inspirado en el cerebro humano, permite gran capacidad de cómputo en tareas cognitivas. | 💰 **Alto costo de desarrollo**: fabricación y diseño de chips neuromórficos es costosa. |
| 🔎 **Optimización en IA**: muy eficientes en reconocimiento de patrones, visión artificial, procesamiento sensorial y robótica. | 🔌 **Dificultad de integración**: falta de compatibilidad con arquitecturas clásicas de Von Neumann. |
| 🌐 **Escalabilidad biológica**: permite crear redes que imitan al cerebro humano, facilitando avances en IA general. | 📉 **Limitaciones en software**: escasez de lenguajes y herramientas de programación adaptadas. |
| 🔒 **Robustez en condiciones adversas**: algunos diseños toleran fallos y ruido en el procesamiento. | ❓ **Aplicaciones poco claras a gran escala**: su utilidad práctica frente a supercomputadores clásicos aún está en evaluación. |
  
    
  </p>
    
  - ### Tipos de computación neuromórfica
    <ul>
      <li>
        <strong> Computación Neuromórfica Digital </strong>
        <p align = "justify">
          Es hardware construido en tecnología CMOS “clásica” (digital) pero organizado como redes de neuronas que disparan picos (spikes). En lugar de hacer grandes multiplicaciones de matrices (como una GPU), estas máquinas procesan eventos: cada pico es un mensaje diminuto que viaja por una red-on-chip hacia sus sinapsis destino. Así se ahorra energía cuando no hay actividad y se imita la dinámica temporal de los sistemas biológicos. Una revisión técnica que enmarca el área (y compara enfoques analógico vs. digital) es la de Indiveri & Liu (Proc. IEEE, 2015). Se compone por: <br/>
          <ul>
            <li>
              <i> Neuronas y sinapsis digitales </i>
            </li>
            <li>
              <i> Memoria local cercana al cómputo </i>
            </li>
            <li>
              <i> Comunicación NoC / AER </i>
            </li>
          </ul>
        </p>
      </li>
      <li>
        <strong> Computación neuromórfica analógica </strong>
        <p align = "justify">
          En lugar de representar los estados neuronales como números discretos en hardware digital (como en TrueNorth o Loihi), aquí se usan señales analógicas (voltajes, corrientes) y elementos físicos que imitan directamente la dinámica de membranas y sinapsis biológicas. Puede ser analógica pura: todo el cálculo (suma de corrientes, integración de voltajes) ocurre con leyes físicas continuas (Ohm, Kirchhoff, capacitancias). o puede ser mixta: se usan bloques analógicos para la dinámica neuronal/sináptica, pero control digital para configuración, comunicación o calibración. Para su arquitectura se pueden comprender cuatro bloques de funcionamiento: <br/>
          <ul>
            <li>
              <i> Neuronas analógicas </i>
              <p align = "justify">
                Se implementan con transistores y condensadores que replican el modelo LIF (Leaky Integrate-and-Fire). Un capacitor acumula carga (potencial de membrana); cuando supera un umbral, un comparador genera un “spike”.
              </p>
            </li>
            <li>
              <i> Sinapsis analógica </i>
              <p align = "justify">
                Donde Resistores, transistores subumbral o memristores representan pesos sinápticos. La corriente que fluye depende del peso, lo que implementa la multiplicación peso × spike de forma natural.
              </p>
            </li>
            <li>
              <i> Plasticidad local </i>
              <p align = "justify">
                STDP (Spike-Timing Dependent Plasticity) puede implementarse directamente en hardware: el solapamiento temporal de señales cambia la conductancia de un memristor o transistor.
              </p>
            </li>
            <li>
              <i> Comunicación </i>
              <p align = "justify">
                Muchos chips usan AER (Address-Event Representation), como en digital, pero el núcleo neuronal es analógico. Otras implementaciones son completamente analógicas, con redes de voltajes acoplados.
              </p>
            </li>
          </ul>
        </p>
      Conviene cuando se requiere eficiencia extrema (nanowatts por sinapsis), En prototipos de sistemas autónomos de bajo consumo (robots insectoides, sensores inteligentes) y sirve para estudiar modelos biológicos realistas con plasticidad emergente.
      </li>
      <li>
        <strong> Computación neuromórfica Híbrida </strong>
        <p>
          Este enfoque combina lo mejor de los dos mundos:Bloques digitales (para control, programación, escalabilidad y comunicación robusta), Bloques analógicos (para emular la dinámica neuronal y sináptica con alta eficiencia energética) y Algoritmos bioinspirados (modelos simplificados del cerebro como el aprendizaje local, redes oscilatorias, plasticidad, etc.). En este tipo, un chip híbrido suele dividirse en tres niveles:
          <ul>
            <li>
              Capa analógica (neuronal/sináptica)
              <p align = "justify">
                Implementa la dinámica del potencial de membrana y las sinapsis (p. ej., con condensadores, transistores en subumbral o memristores). Aquí ocurre el cómputo físico (integración, disparo, plasticidad local).
              </p>
            </li>
            <li>
              Capa digital (control y comunicación)
              <p align = "justify">
                Controla la configuración de parámetros (umbrales, pesos, tiempos de aprendizaje). Maneja la comunicación entre chips usando protocolos como AER (Address-Event Representation). Permite reprogramar redes sin necesidad de rediseñar el hardware.
              </p>
            </li>
            <li>
              Software bioinspirado (modelos de red)
              <p align = "justify">
                Algoritmos que se acercan al comportamiento del cerebro, como aprendizaje Hebbiano, STDP, homeostasis. Traducción de redes de IA convencionales a redes spiking para aprovechar el hardware híbrido.
              </p>
            </li>
          </ul>
        </p>
      </li>
      <li>
        <strong> Computación neuromórfica con Dispositivos emergentes </strong>
        <p align = "justify">
          Este enfoque usa nuevos materiales y tecnologías de hardware diferentes al silicio tradicional, inspirados directamente en la forma en que funcionan las neuronas y sinapsis biológicas. En lugar de implementar neuronas y sinapsis solo con transistores CMOS clásicos, se aprovechan dispositivos como:
          <ul>
            <li> 
              <i> Memristores </i> ➡️ Componentes que recuerdan la corriente pasada (sinapsis con memoria).
            </li>
            <li>
              <i> RRAM (Resistive RAM) </i> ➡️ Resistencias que cambian su valor según el voltaje aplicado.
            </li>
            <li>
              <i> PCM (Phase-Change Memory) </i> ➡️ Materiales que cambian entre estados amorfo y cristalino (como una sinapsis plástica).
            </li>
            <li>
              <i> Dispositivos spintrónicos </i> ➡️ Usan el espín del electrón, no solo su carga, para procesar.
            </li>
            <li>
              <i> Nanofotónica </i> ➡️ Usa la luz para transmitir información como si fueran spikes neuronales.
            </li>
          </ul>
        </p>
      </li>
      <li>
        <strong> Computación neuromórfica Fotónica </strong>
        <p align = "justify">
          La computación neuromórfica fotónica utiliza luz (fotones) en lugar de electrones para procesar y transmitir información en sistemas que imitan al cerebro.
En vez de transistores o memristores, se emplean láseres, moduladores ópticos, guías de onda y detectores de luz para construir "neuronas" y "sinapsis" artificiales. Funciona con una señal de entrada (un pulso de luz entra en un modulador óptico), luego ocurre un procesamiento neuromórfico, aquí la intensidad, fase o polarización de la luz se modifica (imitando cómo cambia la fuerza de una sinapsis), sigue una suma de señales en donde múltiples señales ópticas se combinan en un interferómetro, tal como lo hacen las neuronas al integrar impulsos. Por último ocurre una activación, es decir, un láser o detector convierte el resultado en una señal de salida óptica, lista para ser enviada a la siguiente "neurona".
        </p>
      </li>
    </ul>
  
# Referencias
1. [Sintáxis de escritura y formato básicos](https://docs.github.com/es/get-started/writing-on-github/getting-started-with-writing-and-formatting-on-github/basic-writing-and-formatting-syntax)
2. [Listas en HTML](https://www.mclibre.org/consultar/htmlcss/html/html-listas.html)
3. [¿Qué es la computación cuántica? IBM](https://www.ibm.com/es-es/topics/quantum-computing)
4. [¿Qué es la computación cuántica? AWS](https://aws.amazon.com/es/what-is/quantum-computing/)
5. [¿Cómo es una computadora cuántica? - La estructura física de una computadora cuántica](https://www.spinquanta.com/news-detail/what-does-a-quantum-computer-look-like-explain-key-parts20250116063551+)
6. [Quantum Computing History: Path to Pasqal](https://www.pasqal.com/quantum-computing-history-path-to-pasqal/#1900s)
7. [Quantum Computing: a Timeline](https://www.btq.com/blog/quantum-computing-a-timeline)
8. [History of Quantum computing](https://www.livescience.com/technology/computing/history-of-quantum-computing-key-moments-that-shaped-the-future-of-computing)
9. [¿Qué es la computación neuromórfica? IBM](https://www.ibm.com/es-es/think/topics/neuromorphic-computing)
10. [Overview of the SpiNNaker system Architecture](https://www.researchgate.net/publication/260585643_Overview_of_the_SpiNNaker_System_Architecture)
11. 
