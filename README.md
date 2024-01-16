![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/c290230d-be4c-41f8-8488-433ee746d8d2)# _TALLER 19-20_ <br>

# SPRINT 0 <br>
- Corresponde a la configuraciòn  de herramientas  y entorno de trabajo.  <br>

# CONFIGURACIONES INICIALES <br>
* Ejecutar el comando  "npm init --y"  y habilita el manejo de módulos que sean de tipo module y ya no el clásico commonjs. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743538/78f84cfb-76a6-4ea4-b74c-46d198a08c98) <br>

Ahora debemos instalar los siguientes modulos para el entorno de desarrollo "npm i express bcryptjs mongoose dotenv nodemailer jsonwebtoken cors", "npm i nodemon -D". <br>
<br>
- Estructuras de DIRECTORIOS <br>
"mkdir config controllers helpers middlewares models routers; touch database.js index.js server.js" <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743538/434f3750-1f52-4d0e-b9a2-314251d5c68f) <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743538/4183f405-6da0-4703-8a9d-8aba1e761892) <br>

- SERVIDOR EXPRESS <br>
Programamos la configuración y lógica necesaria para el web server. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743538/ff5ef08f-7a52-4cf2-a28f-466a8a4a09da) <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743538/ff17c3b4-946e-4af5-9e02-6331111f0b8a) <br>

- BASES DE DATOS
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743538/572cbd56-44c5-4223-bd6e-5f31d14f5186)

# SPRINT 1 <br>

- Una vez ya realizada las configuraciones procederemos a realizar el “SPRINT 1”. Para ello importaremos Express, seguido a ello crearemos una instancia de express y haremos las inicializaciones y finalmente exportaremos la instancia de express por medio de app. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/b51745d9-08c0-4c27-bac7-6ce5b3750d39) <br>
- Ahora nos dirigimos al archivo “index.js” e importaremos la variable app. Y después iniciaremos el servidor en el puerto 3000. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/ed1e55c2-0a45-4c6b-9809-25b6c5049962) <br>
- Ahora se procede a ejecutar el siguiente comando node -- watch  .\src\index.js para verificar la funcionalidad del web server. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/6d9cff49-fc15-4ef5-a310-cfbc4717aec8) <br>
- Ahora se procede a programar la configuración de la lógica necesaria para el web server. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/71014ba1-027e-46c5-b8b2-cbe9d960e72f) <br>
- Ahora nos dirigimos a “index.js” ya que en este fragmento de código, utilizando el framework Express. Vamos a desglosar su funcionalidad. De tal manera que al iniciar el servidor Express, lo hace escuchar en el puerto especificado. Después de que el servidor ha sido iniciado con éxito, imprime un mensaje en la consola para indicar que el servidor está funcionando y en qué dirección y puerto se encuentra.
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/47687652-5acb-444e-88a7-5f91569cc608) <br>
- En nuestro “package.json” definimos comandos para ejecutar utilizando el gestor de paquetes npm. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/a27a98fd-ad83-4e05-bf1a-d8607f788969) <br>
- Ahora se procede a ejecutar el siguiente comando  “npm run dev” para verificar la funcionalidad del web server. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/0f174cc2-0715-4b3a-be70-7f15aa96fd24) <br>
- Ahora se programa la configuración y lógica necesaria para la conexión a la Base de datos. Para ello es necesario crear un archivo llamado .env en la raíz del proyecto. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/3bf6d70e-aabf-43ef-89d3-c8e856a68997) <br>
- Importamos el paquete mongoose, y con “strictQuery” permitimos que solo los campos definidos en el schema sean almacenados en la BDD. Después crearemos una función asincrónica llamada  “connection”. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/6648be8f-6d15-4129-af70-51db88e9ee23) <br>
- Importaremos en el “Index.js” la función “connection()”, y hacemos uso de la función. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/dca21fd0-5f25-4be3-ae8f-20acc585a142) <br>
- Ahora se procede a ejecutar el siguiente comando  npm run dev para verificar la funcionalidad de la conexión a la base de datos. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/97b5f4e2-2d68-4057-a4be-15edef6500f1) <br>
- Ahora se procede a modelar los datos (Colecciones y Documentos) mediante el uso de mongoose. Para lo cual se procede a crear un archivo llamado Veterinario.js dentro del directorio models. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/0433d73e-2e4d-49c7-9915-60f7d8088367) <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/23c4bebd-c3dc-495a-a14a-55043252ace2) <br>
# Rutas
- Ahora se procede a crear las respectivas rutas para el modelo Veterinario, en ese sentido, se procede a crear el siguiente archivo en la ruta respectiva. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/c9bbae3a-dcd9-47bb-b322-1b82db803004) <br>
- Ahora se procede a trabajar en la invocación de las rutas. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/031cefc5-9da1-49d1-a366-9d58a59e1188) <br>
# Controladores
- Ahora se procede a crear los respectivos controladores para las rutas del Veterinario, en ese sentido, se procede a crear el siguiente archivo en la ruta respectiva. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/22a8c143-b885-4d47-80b6-49213738e0c9) <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/165fff81-88ca-4d27-90bd-5c2abef2dce8) <br>
- Ahora en “veterinario_routes.js” se procede a trabajar en la invocación de las rutas. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/9066892b-eb7a-479e-93dc-56c743820813) <br>
- Ahora se procede a ejecutar el siguiente comando “npm run dev” para verificar la creación de las rutas con Thunder Client. <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/db86abf7-9c10-49c8-8055-d6c5b9b2c32d) <br>
# Modulo de registro
- Ahora se procede a trabajar en la lógica de cada método del controlador. Importamos el modelo “Veterinario” desde el archivo “Veterinario.js”. Método de registro de nuevo veterinario.  <br>
![image](https://github.com/SandovalBrandon1027/veterinaria/assets/117743120/611bfed1-22e1-4313-9065-ed59725c2720)














