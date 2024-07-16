
Literalura 📚

Literalura es un Gestor de Libros desarrollado en Java como parte del challenge de gestión de libros en Alura Latam en colaboración con Oracle en el programa ONE.

▪️ Descripción

Literalura es una aplicación de consola que te permite buscar libros por título, autores por nombre, listar libros y autores registrados, y obtener estadísticas generales sobre la base de datos de libros. Utiliza la API Gutendex para obtener información sobre libros y una base de datos local (PostgreSQL) para almacenar y gestionar los datos.

Tecnologías Utilizadas 💻

Lenguaje de Programación: Java 17
Framework: Spring Boot
Base de Datos: PostgreSQL
Gestión de Dependencias: Maven
API de Libros: Gutendex
Control de Versiones: Git/GitHub
IDE: IntelliJ IDEA

Funcionalidades 🧩

▪️  Principal.java

El punto de entrada principal del programa. Aquí se maneja la interacción con el usuario a través de la consola, mostrando un menú de opciones y gestionando las consultas sobre libros y autores.

Funcionalidades principales:

✅Buscar libro por título: Permite buscar libros por su título y los registra en la base de datos si no están presentes.

✅Buscar autor por nombre: Permite buscar autores por su nombre.

✅Listar libros registrados: Muestra todos los libros almacenados en la base de datos.

✅Listar autores registrados: Muestra todos los autores almacenados, indicando cuántos libros tienen asociados.

✅Listar autores vivos en un determinado año: Permite buscar autores que estaban vivos en un año específico.

✅Listar libros por idioma: Permite buscar y listar libros según el idioma (ES, EN).

✅Obtener estadísticas generales: Proporciona estadísticas sobre la base de datos de libros.

▪️  ConsumoApi.java

✅Clase responsable de realizar consultas a la API Gutendex para obtener información sobre libros y autores.

▪️  ConvierteDatos.java

✅Clase encargada de convertir los datos obtenidos de la API para su uso en la aplicación.

▪️  AutorRepository.java

✅Interfaz que maneja las operaciones de la base de datos relacionadas con los autores.

▪️  Clases Modelo y Mapeo de Entidades 🗃️

✅En Literalura, utilizamos varias clases modelo para representar las entidades del dominio, como autores y libros. Estas clases están mapeadas a tablas de la base de datos utilizando JPA (Java Persistence API).

▪️  Autor.java

✅La clase Autor representa la entidad "Autor" en la base de datos, incluyendo atributos como el nombre del autor, su fecha de nacimiento y fallecimiento, y una lista de libros asociados.

▪️  Datos.java y DatosLibro.java

✅Estas clases se utilizan para mapear la estructura JSON de la respuesta de la API Gutendex.

Configuración del Proyecto 🚀

1.Clona este repositorio en tu máquina local.

2.Abre el proyecto en IntelliJ IDEA o tu IDE preferido.

3.Configura la conexión a la base de datos PostgreSQL en el archivo de propiedades correspondiente.

4.Ejecuta la clase Principal.java para iniciar la aplicación.


