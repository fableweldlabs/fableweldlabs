# Inventario y equipo — inicio rápido

Inventario y equipo 1.0.0. Godot 4.7.2, Windows x64. Consulta la licencia y los avisos de componentes incluidos.

1. Conserva una copia del proyecto y las partidas. Copia
   `addons/fableweld_inventory` al juego. Compara versiones y conserva tus
   modificaciones antes de sustituir archivos. No requiere reloj ni complemento NPC.
2. Activa Fableweld Inventory & Equipment en Ajustes del proyecto > Plugins.
   Elige el idioma del panel. No cambia la configuración regional global del juego.
3. Crea objetos o añade objetos iniciales. Edítalos en el Inspector y valida el
   catálogo. Guarda un `.tres` fuera de `addons`. Carga un destino existente antes
   de actualizarlo; la carga requiere confirmación. Mantén estables los ID.
4. En el proyecto de ejemplo, abre `demo/inventory_quick_start.tscn` y pulsa F6.
   El selector superior coordina pestañas y paneles. Equipa la espada inicial,
   asigna una poción al acceso rápido, divide una pila y transfiere al cofre.
5. En tus escenas, apunta `controller_path` de los paneles a un
   `FWSlotInventoryController`. Las cuadrículas que intercambian objetos deben
   compartir el recurso de catálogo y un `transfer_group` no vacío. Tu juego
   proporciona los efectos de objetos y las estadísticas base.
6. Registra los controladores en `FWInventorySession.controllers` mediante ID de
   guardado estables y NodePaths. Conecta `FWInventorySavePanel.session_path` a
   esa sesión. Usa una ruta `user://...json` distinta para cada partida o mundo.
7. Guarda y carga la sesión de inventario. Incluye bolsas registradas, equipo y
   accesos rápidos; no guarda todo el juego. La demo antigua pierde su punto de
   control al cerrarse. Conserva cualquier archivo `.fw-writing` antes de
   reintentar un guardado bloqueado. No se admiten escritores simultáneos.
8. Actualiza primero una copia. Mantén catálogos, escenas y partidas fuera de las
   carpetas del proveedor. Para desinstalar, sustituye las referencias
   dependientes, desactiva el plugin y elimina su carpeta. Borrar scripts aún
   referenciados rompe las escenas.

Cambiar el idioma conserva los ID y el texto personalizado. La traducción de
categorías y estadísticas del ejemplo se activa con `translate_example_names`;
está desactivada por defecto en las vistas reutilizables. El texto personalizado
desconocido se conserva. No se afirma revisión lingüística nativa, compatibilidad
con cualquier proyecto ni aceptación final de los paquetes exportados.
