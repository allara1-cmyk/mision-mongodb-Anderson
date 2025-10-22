# Tarea 2 Individual: El Cronista de Datos NoSQL

**Autor:** Lara Anderson  
**Carrera:** Ingeniería en Tecnologías de la Información  
**Asignatura:** Modelado Avanzado de Base de Datos  
**Docente:** Ing. Paulo César Galarza Sánchez  
**Periodo:** Octubre 2025 – Mayo 2026  
**Fecha de Entrega:** 21/10/2025  
**Sede:** Universidad de las Fuerzas Armadas ESPE – Santo Domingo  

---

## Descripción del Escenario — *El Bestiario Digital*

El **Bestiario Digital** es un proyecto diseñado para explorar el uso de **bases de datos NoSQL**, específicamente **MongoDB**, en el manejo de información semi-estructurada.  
El propósito es crear un registro de criaturas fantásticas con atributos variados (como alas, escamas, poderes mágicos o múltiples cabezas), algo difícil de representar en modelos relacionales.

El proyecto se implementó en **MongoDB Atlas**, utilizando **Visual Studio Code** y la extensión oficial **MongoDB for VS Code**, que permitió la conexión directa al clúster en la nube y la ejecución del script mediante Playground.  
Durante el desarrollo se aplicaron los métodos **CRUD (Create, Read, Update, Delete)** para manipular los documentos de la colección principal `criaturas`.

---

## Instrucciones para ejecutar el script `misiones_mongodb.mongodb`

### Abrir el proyecto
- Abra **Visual Studio Code**.  
- Descargue o clone el repositorio desde GitHub.  
- Localice el archivo:  
![Figura 1. Clonacion de repositorio](./images/Clonacion%20del%20repositorio%20de%20Github.png)
---

### Instalar la extensión oficial de MongoDB
- En la barra lateral de VS Code, abra **Extensiones (Ctrl + Shift + X)**.  
- Busque e instale **“MongoDB for VS Code”** (desarrollada por MongoDB Inc.).  
- Asegúrese de tener una conexión activa (local o **MongoDB Atlas**).
![Figura 2. Creacion de Cluster](./images/Creacion%20de%20cluster.png)
---

### Conectarse a la base de datos
- En la barra lateral izquierda, abra la vista **MongoDB** (ícono de hoja verde).  
- Haga clic en **“Connect”** y seleccione:  
- *Local Connection* si usa MongoDB Community Server, o  
- *MongoDB Atlas Cluster* si usa la nube.  
- Una vez conectado, podrá ver las bases de datos existentes.  
![Figura 3. Conexion con Mongo](./images/Conexion%20Mongo%20VSC.png)
---

### Ejecutar el script del Bestiario Digital
- Abra el archivo `misiones_mongodb.mongodb`.  
- En la esquina superior derecha, haga clic en **“Playground ▶️ Run All”**.  
- Esto ejecutará automáticamente todos los comandos definidos en el archivo:
- Creación de la base de datos `bestiario2`.  
- Creación de la colección `criaturas`.  
- Inserciones, consultas, actualizaciones y eliminaciones.
![Figura 4. Ejecucion de Script](./images/Ejecucion%20Script.png)
---

### Verificar los resultados
- En la vista **MongoDB** de VS Code, abra la colección:  