# Capa Común de Acceso a Datos y Estructura del Proyecto

## 📁 Estructura de Carpetas Acordada
* `/services/`: Contiene los módulos centralizados para todas las lecturas y escrituras de la base de datos.
* `/views/` o raíz: Pantallas e interfaces de usuario de la aplicación.

## 📜 Norma Escrita de Desarrollo
1. **Acceso centralizado:** Queda prohibido realizar peticiones directas a la base de datos desde los componentes visuales o pantallas.
2. **Uso obligatorio de servicios:** Cualquier lectura o escritura debe hacerse invocando las funciones exportadas dentro de la carpeta `/services/`.
3. **Mantenibilidad:** Si el modelo de datos cambia en el futuro, solo será necesario actualizar el código dentro de esta capa común.
