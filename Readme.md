
## Deploy local

1. Crear un directorio e ingresar en el mismo
```bash
   mkdir proyecto
   cd proyecto
```

2. Clonar el repositorio
```bash
   git clone https://github.com/xarcraft/gestor_torneos.git
```
   
3. Crear un entorno virtual dentro del directorio a utilizar
```bash
   python -m venv .venv
```
   
4. Activar el entorno
```bash
   .\.venv\Scripts\activate
```

5. Deslplazarce al directorio del aplicativo
```bash
   cd gestor_torneos
```  

6. Instalar las dependencias
```bash
   pip install -r requirements.txt
```

7. Crear base de datos - corra el siguiente comando en una terminal de ***Mysql*** (preferiblemente en una terminal diferente a la que hemos usado para los comandos anteriores):
```sql
CREATE DATABASE `nombredelabase` /*!40100 DEFAULT CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci */;
```
___Opcionalmente puede usar un gestor de bases de datos de su preferencia y crear el esquema en manual solo debe asegurarse de digitar el mismo nombre que configuro en el paso anterior___

Importa el archivo sql en tu gestor de bases de datos para cargar el esquema completo.


## Levantar la aplicación

2. Levante la aplicación con este comando
```bash
python manage.py runserver
```
  
4. Acceda a la aplicación - `http://127.0.0.1:8000/`
