# Ex_JS_Asincronia_and_PromesasEx JS - Asincronía & Promesas


Investigación

¿Qué es un archivo JSON?

¿Qué es la asincronía en Javascript?

¿Qué son las Promesas?

¿Qué es y cómo se usa ‘Fetch’ en JS?

¿Cómo se usa Async/Await?

¿Cuándo deberíamos usar código asíncrono?



Presentación:

El formato JSON (JavaScript Object Notation) es un formato abierto utilizado como alternativa al XML para la transferencia de datos estructurados entre un servidor de Web y una aplicación Web. Su lógica de organización tiene puntos de semejanza con el XML, pero posee una notación diferente.
La programación asíncrona en javascript, hace uso de los llamados threads o hilos de ejecución del procesador para que puedas ejecutar más de un proceso a la vez en tu aplicación. La programación asíncrona en JavaScript, es una técnica que permite a un programa iniciar una tarea de larga duración y seguir respondiendo a otros eventos mientras esa tarea se ejecuta, en lugar de tener que esperar hasta que esa tarea haya terminado. Una vez que dicha tarea ha finalizado, tu programa presenta el resultado.
Una Promesa ( Promise) es un valor pendiente que no obstante se conoce cuando se crea la promesa. Le permite asociar controladores con el valor eventual de éxito o el motivo de falla de una acción asíncrona. Esto permite que los métodos asíncronos devuelvan valores como los métodos síncronos: en lugar de devolver inmediatamente el valor final, el método asíncrono devuelve la promesa de proporcionar el valor en algún momento en el futuro.
La API Fetch proporciona una interfaz JavaScript para acceder y manipular partes del canal HTTP, tales como peticiones y respuestas. También proporciona un método global fetch() que proporciona una forma fácil y lógica de obtener recursos de forma asíncrona por la red.
Cuando se llama a una función async, esta devuelve un elemento Promise. Cuando la función async devuelve un valor, Promise se resolverá con el valor devuelto. Si la función async genera una excepción o algún valor, Promise se rechazará con el valor generado.
La API Fetch proporciona una interfaz JavaScript para acceder y manipular partes del canal HTTP, tales como peticiones y respuestas. También proporciona un método global fetch que proporciona una forma fácil y lógica de obtener recursos de forma asíncrona por la red.
Una función async puede contener una expresión await, la cual pausa la ejecución de la función asíncrona y espera la resolución de la Promise pasada y, a continuación, reanuda la ejecución de la función async y devuelve el valor resuelto.
Es buena práctica aplicar la programación asíncrona en las situaciones que no se tiene el control del proceso, por ejemplo:
Llamadas a bases de datos, no sabemos cuánto tarde en devolvernos la data solicitada o en que termine de insertar los registros enviados, en resumen no tenemos control del servidor de base de datos.
Cuando se trabaja con archivos, también no se tiene el control, puede que necesite permisos al sistema operativo o mil situaciones, dejar paralizada nuestra aplicación por esto sería mortal.
Mejor control de los procesos, si no ejecutamos await por ejemplo, puede que nuestra aplicación quiera continuar en el mismo thread sin que haya terminado de traer la información de la base de datos, con esto se generan inconsistencias, también podría generar colisiones en las llamadas a la base de datos dejándola no disponible para algunos usuarios mientras que otros sí obtienen lo esperado.
Mayor disponibilidad del sistema, ya que permite ejecutar múltiples acciones al mismo tiempo.
