# clase-10
05/16/2024

# De MIDI a grasshopper
Necesito conseguir un controlaodr MIDI para poder conectarlo a mi computadora y usarlo para manupular sliders en grasshopper.

- El controlador MIDI Korg nanopad2. Este controlador se puede conectar por USB, incluye muchos botones y un trackpad que emite mensajes de cambio de control.
- Burcar en facebook marketplace...

Necesito conseguir una forma de comunicar a grasshopper con el controlador.

Por ahora estoy aprendiendo lo basico. Decidí usar C# ya que me permitirá eventualmente crear mi propio plugin para grasshopper para usa controladores MIDI en grasshopper.

Por ahora puedo hacer codigos muy básicos, ya puedo crear y manipular objetos en rhino desde grasshopper usando bloques de C# script.

Seguiré aprendiendo a travez de esta fuente. [RhinoCommon](<https://developer.rhino3d.com/api/rhinocommon/?version=8.x>)

Antes de esto estuve viendo las clases del profesor [Long Nguyen](<https://www.youtube.com/watch?v=pFCrIzENDn8&t=4709s>).

![image](https://github.com/MarcialLeaplaza/dis145/assets/165319963/4d7fff8f-0105-4ae2-b527-f88d22262cdb)

- Aprender a leer inputs de MIDI.

Para leer los inputs de midi encontre este [codigo](<https://stackoverflow.com/questions/1991159/getting-signals-from-a-midi-port-in-c-sharp>), Tiene una breve explicacion pero necesito saber bien como funciona. Segun el autor solo funciona para mensajes cortos y dice que se puede volver mas complejo si tratamos de hacer streaming, lo que me preocupa ya que podria ser un desafio necesario de superar para mi proyecto, espero que grasshopper me facilite esta parte del proyecto.

Este condigo usa lo que se llama una Callbach funtion, lo cual es una funcion que usa como argumento a otra funcion, en este caso para encargarse de los mensages en MIDI.

Encontre un [video](<https://www.youtube.com/watch?v=wKEyzLfvJH8&list=PLT1oacQFeNK5Q5LVx82_Rv_7fH4X5lYp9>) guia para aprender a leer e interpretar midi en c#.
- Traducir los inputs a valores utiles.
- Asignar esos valores a un grasshopper.



Necesito crear una interfase que me permita asignar un componente de grasshopper con un componente del controlador.

