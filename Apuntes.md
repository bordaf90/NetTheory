
### ASP.NET Core es un marco web creado por Microsoft para crear aplicaciones web, API y microservicios.
Otros marcos web son Node js, Laravel, Spring, Django, entre otras.
####ASP.NET corre en .NET .
### NuGet es el administrador de paquetes de .NET.
NuGet vendría a ser el equivalente a npm, Maven, etc.
### .NET Standard es una interfaz independiente de la plataforma que define características y API.
no representa ningún código o funcionalidad real, solo la definición de API. Existen diferentes "versiones" o niveles de .NET Standard que reflejan cuántas API están disponibles (o qué tan amplia es la superficie de la API). Por ejemplo, .NET Standard 2.0 tiene más API disponibles que .NET Standard 1.5, que tiene más API que .NET Standard 1.0.

### .NET Framework es una implementación diferente de .NET Standard que es solo para Windows.
Este fue el único tiempo de ejecución de .NET hasta que apareció .NET Core y trajo .NET a Mac y Linux. 

## ¿Qué se necesita para empezar a trabajar?

1) Editor de código (Atom, Visual Studio, etc).
2) El SDK de .NET Core

Para saber si tengo el sdk instalado:

dotnet --version

## Creando una aplicación en c#:

1) dotnet new console -o CsharpHelloWorld
2) cd CsharpHelloWorld
3) dotnet run

##  Nuevo proyecto, más complejo:

dotnet new mvc --auth Individual -o AspNetCoreTodo

## Las partes de un proyecto ASP.NET Core
La dotnet new mvcplantilla genera una serie de archivos y directorios. Estas son los archivos más importantes que se obtienen:

Los archivos Program.cs y Startup.cs configuran el servidor web y la canalización de ASP.NET Core. La Startupclase es donde puede agregar middleware que maneja y modifica las solicitudes entrantes y sirve cosas como contenido estático o páginas de error. También es donde agrega sus propios servicios al contenedor de inyección de dependencia.

Los directorios Modelos , Vistas y Controladores contienen los componentes de la arquitectura Modelo-Vista-Controlador (MVC).

El directorio wwwroot contiene activos estáticos como CSS, JavaScript y archivos de imagen. Los archivos en se wwwrootservirán como contenido estático y se pueden agrupar y minificar automáticamente.

El archivo appsettings.json contiene opciones de configuración que ASP.NET Core se cargará al inicio. Puede usar esto para almacenar cadenas de conexión de base de datos u otras cosas que quieras codificar.



