# Mi Proyecto en GitHub

## Descripción del Proyecto
Mi Proyecto es una aplicación web construida con .NET 8, utilizando el patrón MVC (Model-View-Controller). El proyecto permite gestionar contactos con funcionalidades de CRUD (Crear, Leer, Actualizar, Eliminar).

## Requisitos
- .NET 8 SDK instalado en tu máquina.
- SQL Server instalado y en ejecución en tu máquina local.
- Un editor de código como Visual Studio, Visual Studio Code o cualquier otro editor que soporte .NET.
- Dependencias de NuGet instaladas (se restaurarán automáticamente si usas `dotnet restore`).

## Clonar el Repositorio
Clona el repositorio en tu máquina local:

git clone <URL-del-repositorio>
cd MiProyecto
## Configuración de la Base de Datos
Abre el archivo `appsettings.json` en la raíz del proyecto. Encuentra la sección `ConnectionStrings` y actualiza la cadena de conexión para que coincida con tu configuración de SQL Server.

## Crear la Base de Datos
Si aún no tienes la base de datos configurada, puedes crearla ejecutando las migraciones con el siguiente comando:



dotnet ef database update


## Funcionalidades
- **Crear Contacto**: Permite agregar nuevos contactos con nombre, teléfono, celular, email y fecha de creación.
- **Listar Contactos**: Muestra todos los contactos almacenados en la base de datos.
- **Editar Contacto**: Permite editar los detalles de un contacto existente.
- **Ver Detalles de Contacto**: Muestra los detalles completos de un contacto.
- **Eliminar Contacto**: Permite eliminar un contacto de la base de datos.

## Estructura de Archivos
- `Controllers/InicioController.cs`: Lógica del controlador para la gestión de contactos.
- `Models/Contacto.cs`: Modelo de datos para los contactos.
- `Views/Inicio/Index.cshtml`: Vista para mostrar la lista de contactos.
- `Views/Inicio/Crear.cshtml`: Vista para crear nuevos contactos.
- `Views/Inicio/Editar.cshtml`: Vista para editar contactos existentes.
- `Views/Inicio/Detalle.cshtml`: Vista para ver los detalles de un contacto.
- `Views/Inicio/Borrar.cshtml`: Vista para confirmar la eliminación de un contacto.

