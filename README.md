Ejercicio1.js

function CalcularAreaTriangulo(Base, Altura) {
    return (Base * Altura) /2;
}
const baseTriangulo = prompt ("Ingrese por favor la base del triangulo")
const alturaTriangulo = prompt("Ingrese por favor la altura del triangulo")
const areaTriangulo = CalcularAreaTriangulo(baseTriangulo, alturaTriangulo);
console.log(`El área del triángulo con base ${baseTriangulo} y altura ${alturaTriangulo} es: ${areaTriangulo}`);

Ejercicio2.js

function CambioDolares(pesos, Tcambio) {
    return  (pesos * Tcambio)/2;

}
const Cpesos = prompt("Ingrese por favor cuantos pesos colombianos desea cambiar a dolares")
const Cdolar = prompt("Ingrese el valor el dolar")
const CambioDolar = CambioDolares(Cpesos, Cdolar);
console.log(`el dolar esta en ${Cdolar}, cambiando  ${Cpesos} pesos colombianos, el total seria  ${CambioDolar} dolares`);

Ejercicio3.js

function calcularEdadTrabajo(AniodeNacimiento) {
    const anioAc = new Date().getFullYear();
  
    const Edad = anioAc - AniodeNacimiento;
    return Edad;
  }
   let AniodeNacimiento = prompt("Ingrese por favor su Año de nacimiento")
  const Edad = calcularEdadTrabajo(AniodeNacimiento);
  console.log(`Si naciste en el año ${AniodeNacimiento}, entonces tienes ${Edad} años.`);

  Ejercicio4.js

  function cobroEstacionamiento(horas) {
      
    const PrecioHora = 1000;
    const horasCompletas = Math.ceil(horas);
    const PrecioTotal = PrecioHora * horasCompletas;
    return PrecioTotal;
  }
  let horasCompletas = prompt("Ingrese por favor las horas que estuvo estacionado")
  const PrecioTotal = cobroEstacionamiento(horasCompletas);
  console.log(`El total a cobrar por ${horasCompletas} horas de estacionamiento es: $${PrecioTotal}`);

  Ejercicio5.js

  function calcularPresupuesto(area, costoPorMetroCuadrado) {
    const costoTotal = area * costoPorMetroCuadrado;
    return costoTotal;
  }
  
  let area = prompt("Ingrese por favor el area que desea pintar")
  const costoPorMetroCuadrado = 3000;
  
  const presupuesto = calcularPresupuesto(area, costoPorMetroCuadrado);
  console.log(`El presupuesto para el trabajo de pintura es: ${presupuesto} pesos colombianos`);

  Ejercicio6.js

  function calcularHipotenusa(catetoA, catetoB) {
    const catetoAcuadrado = catetoA * catetoA;
    const catetoBcuadrado = catetoB * catetoB;
    const hipotenusacuadrado = catetoAcuadrado + catetoBcuadrado;
    const hipotenusa = Math.sqrt(hipotenusacuadrado);
  
    return hipotenusa;
  }
  let catetoA = prompt("Ingrese por favor el lado A")
  let catetoB = prompt("Ingrese por favor el lado B")
  
  const hipotenusa = calcularHipotenusa(catetoA, catetoB);
  console.log(`La hipotenusa del triángulo rectángulo es: ${hipotenusa}`);

  Ejercicio7.js

  function calcularPrecioFinal(precioArticulo) {
    const descuento = precioArticulo * 0.2;
    const precioConDescuento = precioArticulo - descuento;
    const iva = precioConDescuento * 0.15;
    const precioFinal = precioConDescuento + iva;
  
    return {
      precioConDescuento: precioConDescuento,
      precioFinal: precioFinal
    };
  }
  
  const precioArticulo = prompt("Ingrese por favor el precio de sus articulos");
  const resultado = calcularPrecioFinal(precioArticulo);
  console.log(`El total de lo que debe pagar con el 20 % de descuento es:  ${resultado.precioConDescuento}`);
  console.log(`El total a pagar final con IVA incluido es:  ${resultado.precioFinal}`);

  Ejercicio8.js

  function calcularAhorroAnual(sueldoMensual) {
    const semanasPorMes = 4;
    const porcentajeAhorro = 0.15;
    const mesesEnAnio = 12;
    const ahorroSemanal = sueldoMensual * porcentajeAhorro / semanasPorMes;
    const ahorroMensual = ahorroSemanal * semanasPorMes;
    const ahorroAnual = ahorroMensual * mesesEnAnio;
  
    return ahorroAnual;
  }
  const sueldoMensual = prompt("Ingrese por favor su sueldo")
  const ahorroAnual = calcularAhorroAnual(sueldoMensual);
  console.log(`El ahorro anual es: $${ahorroAnual}`);

  Ejercicio9.js

  function calcularMontoCheque(numDias) {
    const costoHotelPorDia = 100000;
    const costoComidaPorDia = 70000;
    const otrosGastosPorDia = 200000;
    const gastosTotalesPorDia = costoHotelPorDia + costoComidaPorDia + otrosGastosPorDia;
    const montoTotalCheque = gastosTotalesPorDia * numDias;
  
    return {
      hotel: costoHotelPorDia * numDias,
      comida: costoComidaPorDia * numDias,
      otrosGastos: otrosGastosPorDia * numDias,
      total: montoTotalCheque,
    };
  }
  
  const numeroDiasViaje = prompt("Ingrese por favor el numero de dias que desea viajar para saber el valor de su cheque "); // Ingresa aquí el número de días que el empleado viajará
  const montoCheque = calcularMontoCheque(numeroDiasViaje);
  console.log("Desglose del monto del cheque:");
  console.log(`Hotel: $${montoCheque.hotel}`);
  console.log(`Comida: $${montoCheque.comida}`);
  console.log(`Otros gastos: $${montoCheque.otrosGastos}`);
  console.log(`Total: $${montoCheque.total}`);

  Ejercicio10.js

  function calcularAreaCuadrado(longitudLado) {
    const area = longitudLado * longitudLado;
    return area;
  }
  
  const longitudLadoCuadrado = prompt ("Para darle el area del cuadrado debemos saber la longitud de uno de sus lados, por favor ingrese la longitud de un lado ")
  const areaCuadrado = calcularAreaCuadrado(longitudLadoCuadrado);
  console.log(`El área del cuadrado es: ${areaCuadrado} unidades cuadradas.`);

  Ejercicio11.js

  function calcularPromedio(examen1, examen2, examen3) {
    const ponderacionExamen1 = 0.25;
    const ponderacionExamen2 = 0.25;
    const ponderacionExamen3 = 0.5;
    const notaPonderadaExamen1 = examen1 * ponderacionExamen1;
    const notaPonderadaExamen2 = examen2 * ponderacionExamen2;
    const notaPonderadaExamen3 = examen3 * ponderacionExamen3;
    const promedio = notaPonderadaExamen1 + notaPonderadaExamen2 + notaPonderadaExamen3;
  
    return promedio;
  }
  const notaExamen1 = prompt("Ingrese por favor la nota del primer examen")
  const notaExamen2 = prompt("Ingrese por favor la nota del segundo examen")
  const notaExamen3 = prompt("Ingrese por favor la nota del tercer examen")
  const promedioFinal = calcularPromedio(notaExamen1, notaExamen2, notaExamen3);
  console.log(`El promedio final del alumno es: ${promedioFinal}`);

  Ejercicio12.js

  function calcularFormasDePago(valorTotalCompra) {
    const recargo2Cuotas = 0.05;
    const recargo6Cuotas = 0.40;
    const formaPago1Cuota = {
      cuotas: 1,
      montoPorCuota: valorTotalCompra,
      total: valorTotalCompra,
      recargo: 0,
    };
    const monto2Cuotas = valorTotalCompra / 2;
    const recargo2CuotasTotal = monto2Cuotas * recargo2Cuotas;
    const formaPago2Cuotas = {
      cuotas: 2,
      montoPorCuota: monto2Cuotas,
      total: valorTotalCompra + recargo2CuotasTotal,
      recargo: recargo2CuotasTotal,
    };
    const monto6Cuotas = valorTotalCompra / 6;
    const recargo6CuotasTotal = monto6Cuotas * recargo6Cuotas;
    const formaPago6Cuotas = {
      cuotas: 6,
      montoPorCuota: monto6Cuotas,
      total: valorTotalCompra + recargo6CuotasTotal,
      recargo: recargo6CuotasTotal,
    };
  
    return [formaPago1Cuota, formaPago2Cuotas, formaPago6Cuotas];
  }
  
  // Ejemplo de uso:
  const valorTotalCompra = prompt("Ingresa aquí por favor el valor total de la compra")
  const formasDePago = calcularFormasDePago(valorTotalCompra);
  console.log("Posibles formas de pago:");
  formasDePago.forEach((formaPago, index) => {
    console.log(`Forma de pago ${index + 1}:`);
    console.log(`- Cuotas: ${formaPago.cuotas}`);
    console.log(`- Monto por cuota: $${formaPago.montoPorCuota}`);
    console.log(`- Recargo total: $${formaPago.recargo}`);
    console.log(`- Total a pagar: $${formaPago.total}`);
    console.log("---------------------");
  });

  Index.html

  <!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
</head>
<body>
    <script src="Ejercicio1.js"></script>
    <script src="Ejercicio2.js"></script>
    <script src="Ejercicio3.js"></script>
    <script src="Ejercicio4.js"></script>
    <script src="Ejercicio5.js"></script>
    <script src="Ejercicio6.js"></script>
    <script src="Ejercicio7.js"></script>
    <script src="Ejercicio8.js"></script>
    <script src="Ejercicio9.js"></script>
    <script src="Ejercicio10.js"></script>
    <script src="Ejercicio11.js"></script>
    <script src="Ejercicio12.js"></script>

</body>
</html>

readme.md

Santiago Arredondo Rios



¿Que es una variable?

R//: En programación, una variable es un espacio de memoria con un nombre asociado que se utiliza para almacenar un valor. Es como una caja etiquetada con un nombre en la que puedes poner diferentes valores, y esos valores pueden cambiar a lo largo del tiempo.


¿Qué es una Condición?

R//: En programación, una condición es una expresión lógica que evalúa si una afirmación es verdadera o falsa. Las condiciones se utilizan principalmente para controlar el flujo del programa, permitiendo que ciertas partes del código se ejecuten solo si se cumple una condición específica.

Las condiciones se expresan utilizando operadores de comparación, como mayor que (>), menor que (<), igual a (=), diferente de (!=), mayor o igual que (>=), menor o igual que (<=), entre otros. También se pueden combinar varias condiciones utilizando operadores lógicos, como "y" (AND), "o" (OR) y "no" (NOT), para construir expresiones más complejas.


¿Qué es una Estructura de datos?

R//:Una estructura de datos es una forma organizada de almacenar y organizar datos en una computadora o en cualquier dispositivo de almacenamiento. Estas estructuras permiten manipular y acceder a los datos de manera eficiente y facilitan la implementación de algoritmos y la resolución de problemas.


¿Qué es la Consola?

R//:La consola, también conocida como línea de comandos o terminal, es una interfaz de texto que permite a los usuarios interactuar con un sistema operativo o una aplicación mediante comandos escritos en texto plano. A diferencia de las interfaces gráficas de usuario (GUI), donde los usuarios interactúan con el sistema a través de ventanas, iconos y menús, la consola se basa en el uso de comandos específicos que se ingresan mediante el teclado.


¿Qué es una Entrada?

R//:En el contexto de la informática y la programación, una entrada se refiere a los datos, señales o información que un programa o sistema recibe del usuario, de otro programa o de una fuente externa. Estos datos pueden ser proporcionados de diversas formas y pueden variar según la naturaleza de la aplicación o el sistema en cuestión.


¿Qué es una Salida?

R//:En informática y programación, una salida se refiere a los resultados, datos o información que un programa o sistema produce y muestra al usuario o envía a otra aplicación o dispositivo externo. Es el resultado del procesamiento de las entradas que el programa recibió previamente.


¿Qué es un Proceso?

R//: 
En el contexto de la informática y los sistemas operativos, un proceso es una instancia en ejecución de un programa de computadora. Pueden ser considerados como las unidades fundamentales de ejecución en un sistema operativo y representan una tarea o trabajo que se está realizando en la computadora.


¿Cuál es la estructura de un algoritmo?

R//:La estructura de un algoritmo se refiere a cómo está organizado y diseñado dicho algoritmo. Un algoritmo es una secuencia de pasos o instrucciones bien definidas que resuelven un problema o realizan una tarea específica. Si bien la estructura exacta de un algoritmo puede variar según la tarea que se esté abordando, generalmente sigue una serie de elementos comunes:

Entrada: Todo algoritmo requiere datos de entrada para operar. Estos datos pueden ser proporcionados por el usuario, extraídos de archivos, recibidos a través de una conexión de red, entre otros. La entrada es fundamental para que el algoritmo sepa con qué datos debe trabajar.

Salida: Después de procesar los datos de entrada, el algoritmo produce resultados o salidas. Estos resultados pueden ser valores numéricos, mensajes, archivos generados o cualquier otro tipo de información relevante para la tarea que se esté realizando.

Instrucciones o pasos: La parte central de un algoritmo son las instrucciones o pasos que describen cómo procesar los datos de entrada para obtener los resultados deseados. Estas instrucciones deben ser precisas, claras y deben llevar a la resolución del problema.

Control de flujo: Los algoritmos incluyen estructuras de control de flujo, como decisiones condicionales (if/else), bucles (for, while) y estructuras de selección (switch/case). Estas estructuras permiten al algoritmo tomar diferentes caminos según ciertas condiciones o repetir ciertas acciones varias veces.

Variables y datos auxiliares: Los algoritmos a menudo utilizan variables para almacenar y manipular datos temporales durante la ejecución. Estas variables pueden cambiar su valor a medida que el algoritmo avanza.

Abstracción: Para mantener la legibilidad y facilitar la comprensión, los algoritmos pueden utilizar abstracciones, que son funciones o subrutinas que encapsulan ciertas operaciones o cálculos complejos en bloques más pequeños y manejables.


¿Características de un Algoritmo?

R//:Las características de un algoritmo son atributos clave que definen la naturaleza y el comportamiento de un algoritmo. Un algoritmo efectivo debe tener las siguientes características:

Precisión: Un algoritmo debe estar bien definido y ser preciso en sus pasos e instrucciones. Cada paso debe ser claramente entendible y no debe haber ambigüedad en su interpretación.

Finitud: Un algoritmo debe terminar después de un número finito de pasos. Esto significa que debe tener un punto final y no puede ejecutarse infinitamente.

Entrada: Todo algoritmo debe tener datos de entrada especificados. Estos datos son necesarios para que el algoritmo realice su tarea.

Salida: Un algoritmo debe producir resultados o salida después de procesar los datos de entrada. La salida debe estar relacionada con el problema que el algoritmo resuelve.

Claridad y legibilidad: Un algoritmo debe ser fácil de entender y leer, tanto para el programador que lo escribió como para otros que lo revisen o mantengan en el futuro.

Eficacia y eficiencia: Un algoritmo debe resolver el problema de manera efectiva y en un tiempo razonable. Debe utilizar los recursos disponibles de manera eficiente, como tiempo de ejecución y memoria.

Generalidad: Un algoritmo debe ser general y aplicable a un conjunto amplio de casos, no solo a situaciones específicas.

Independencia de plataforma: Un buen algoritmo debe ser independiente de la plataforma o sistema operativo. Debería poder ejecutarse en diferentes entornos sin modificaciones significativas.

División y modularidad: Los algoritmos pueden dividirse en partes más pequeñas o módulos para facilitar la comprensión y el mantenimiento. La modularidad permite abstraer partes complejas del algoritmo en funciones o subrutinas reutilizables.

Robustez: Un algoritmo debe manejar situaciones excepcionales o inesperadas de manera adecuada y producir resultados coherentes y razonables.


¿Cuáles consolas usamos en programación?

R//:En programación, las consolas o líneas de comandos son herramientas que permiten a los programadores interactuar con el sistema operativo y ejecutar comandos o programas mediante texto plano. Estas consolas son especialmente útiles para tareas de desarrollo, pruebas, automatización y gestión de sistemas. Algunas de las consolas más utilizadas en programación son:

Terminal (Bash o Shell): Es la consola estándar en sistemas Unix/Linux y macOS. Utiliza el interprete de comandos Bash o Shell para ejecutar comandos y scripts en lenguaje de comandos.

Símbolo del sistema (Command Prompt): Es la consola predeterminada en sistemas Windows. Permite ejecutar comandos y scripts en el lenguaje de comandos de Windows.

PowerShell: Es una consola más avanzada y versátil que se encuentra en sistemas Windows. Proporciona una poderosa interfaz de línea de comandos con capacidades de scripting más sofisticadas.

Python Interactive Shell: El intérprete interactivo de Python, también conocido como REPL (Read-Eval-Print Loop), permite ejecutar comandos Python de forma interactiva y ver los resultados inmediatamente.

Node.js REPL: Es una consola interactiva que permite ejecutar comandos JavaScript en tiempo real utilizando Node.js.

R: Es una consola interactiva utilizada para programación estadística y análisis de datos con el lenguaje de programación R.

Jupyter Notebook: Aunque técnicamente no es una consola en el sentido tradicional, Jupyter Notebook proporciona una interfaz interactiva basada en navegador que permite a los usuarios ejecutar celdas de código en varios lenguajes, como Python, R, Julia, entre otros.



¿Cuál es el ciclo de vida de una variable?

R//:El ciclo de vida de una variable se refiere a las diferentes etapas por las que pasa desde su creación hasta su eliminación o desaparición en un programa. Las variables son elementos fundamentales en la programación, ya que se utilizan para almacenar y manipular datos durante la ejecución del programa. El ciclo de vida de una variable generalmente consta de cuatro fases:

Declaración: En esta etapa, se define la variable y se reserva espacio en la memoria para almacenar el valor que contendrá. La declaración generalmente incluye el nombre de la variable y su tipo de datos.

Inicialización: Después de la declaración, la variable puede ser inicializada, lo que significa asignar un valor inicial a la variable. La inicialización no siempre es necesaria, pero es una buena práctica para evitar comportamientos inesperados debido a valores no inicializados.

Uso: Durante esta fase, la variable puede ser utilizada y modificada en el programa. Puede ser leída para obtener su valor o actualizada con un nuevo valor en diferentes partes del programa.

Finalización: Cuando una variable ya no es necesaria o su alcance (ámbito) termina, se dice que ha llegado al final de su ciclo de vida. En este punto, la variable puede ser desechada o liberada de la memoria, lo que generalmente ocurre automáticamente cuando el programa alcanza el final de su ejecución o cuando la variable sale de su ámbito.
