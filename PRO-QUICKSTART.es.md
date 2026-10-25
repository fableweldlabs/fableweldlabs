Calendar & Growth Pro — Inicio rápido
Documentación de la versión candidata 2.1.0; todavía no publicada.

1. Copia addons/rpg_time en tu proyecto. Activa el complemento en Project > Project Settings > Plugins. Para probar el proyecto de ejemplo, extrae su descarga por separado y abre su project.godot; no reemplaces el archivo de tu juego.
2. Abre Time & Seasons y selecciona Español en Language. El idioma del panel no cambia el idioma de Godot ni el de tu juego.
3. En Configuración, elige una ruta res:// fuera de addons y pulsa Guardar perfil. Los campos modificados solo se aplican al pulsar Aplicar. Aplica o revierte los campos antes de cambiar de sección.
4. En Calendario, configura meses, días y estaciones. Los nombres personalizados se guardan tal como los escribes. En Períodos, el primero empieza a las 00:00 y los demás deben ir en orden.
5. Para crecimiento, elige un preajuste y ajusta el ritmo. Puedes editar después la madurez y las etapas. Mover el control o elegir otro preajuste sustituye esas ediciones. Estos valores se usan para la siguiente escena generada.
6. Guarda el perfil y crea el montaje deseado. Arrastra la escena generada a tu mundo o usa la inserción del panel. Mantén un único reloj principal; no añadas un segundo CanvasModulate a un lienzo ya conectado.
7. Usa Vista previa para probar avances, estaciones y eventos sin alterar el reloj del juego ni los guardados. Los saltos que atraviesen más de 10.000 eventos se rechazan.

Los controles reutilizables tienen interface_language en el Inspector. Tras cambiarlo durante el juego, llama a refresh(). Los títulos, nombres y mensajes personalizados siguen siendo tuyos para traducir. Deja vacío el texto del botón de dormir para usar su etiqueta traducida automática.

save_file/load_file guardan el estado del reloj, no un juego completo. Conserva los guardados originales al probar una actualización. Cambiar las definiciones del calendario o eventos puede exigir una migración. Los perfiles opcionales de atmósfera amplían la iluminación básica; no contiene un sistema de clima, combate o movimiento de NPC.


Atmósfera y herramientas de desarrollo
En Iluminación, elige y aplica un preajuste de atmósfera. Los interruptores conservan las curvas editadas manualmente. Guarda el perfil y crea una nueva configuración. En el ejemplo opcional Lumen Vale, abre Calendario y desplázate hasta Atmósfera. Sin atmósfera conserva el aspecto original. La vista previa y el interruptor de niebla no cambian el perfil guardado; quitar la vista previa restaura la iluminación original.

Las herramientas de desarrollo locales se incluyen solo si las seleccionas al generar. Están desactivadas de forma predeterminada, se conectan automáticamente al reloj y permanecen desactivadas en el ejecutable de distribución. DEVELOPMENT-BRIDGE.md describe el contrato de Fableweld; no abre acceso a la red.
