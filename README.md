CASO DE ESTUDIO: SISTEMA DE PRÉSTAMO DE LIBROS RAROS Y ANTIGUOS
El sistema está diseñado con un esquema tipo estrella (star schema), que consta de una tabla de hechos central y varias tablas de dimensiones que la rodean, esto facilita consultas rápidas y análisis detallados.

•	Tabla de hechos: Loans (Préstamos):
Contiene las transacciones de préstamos con referencias a las dimensiones.
Campos principales: LoanID (clave primaria), BookID, UserID, LocationID, DateID (claves foráneas).


•	Tablas de dimensiones:
o	Books (Libros): información sobre los libros, como título, autor, año, nivel de rareza, idioma y categoría. 

o	Users (Usuarios): datos demográficos y tipo de membresía de los usuarios.

o	Locations (Ubicaciones): sucursal, ciudad y país donde se realiza el préstamo.

o	Time (Tiempo): fechas con desgloses de día, mes, año y trimestre.

Este esquema permite analizar patrones de préstamos según características del libro, perfil del usuario, ubicación y periodo temporal.
