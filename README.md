# 20180425_Examen02_024313
El patrón de comando requiere la creación de pequeños objetos de "comando" que se derivan de una interfaz de comando . El patrón del Mediador reduce el acoplamiento manteniendo un registro de diferentes objetos y estableciendo cómo un objeto debería reaccionar a un evento de otro sin que estos objetos se conozcan entre sí.
crear una clase abstracta (Tarea ) que extienda todas las tareas, registra los robots que desean monitorear la tarea. Cada vez que se activa un nuevo evento en tarea pasa el comando a los robots. Cree una clase Mediator para que sea el oyente principal de los eventos de la tarea abstracta. 

 Primero el Mediador ejecuta tareota donde configurará con terminada y progreso , y luego ejecutará la tarea. Es importante observar que las implementaciones de ejecutar en terminada y progeso llamarán a los métodos motrar progreso y terminar tarea, respectivamente.

La lógica para cuando se llama al comando es la siguiente: cada vez que Tareota desea comunicar el progreso, llama al método de ejecutar de  Command devuelto al llamar a su método padre getProgreso  y Terminada método hará lo mismo para la devolución de getSucceedCommand .
