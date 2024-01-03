Despliegue Automatizado con Apache, MariaDB y Git
Este repositorio contiene un script de automatización en Bash para desplegar un entorno web utilizando Apache como servidor web, MariaDB como base de datos, y Git para la gestión del código fuente.

Requisitos Previos
Sistema operativo basado en Debian (probado en Ubuntu)
Acceso de superusuario (root)
Instrucciones de Uso
Clona el repositorio:

git clone https://github.com/tu-usuario/tu-repo.git
cd tu-repo
Ejecuta el script de despliegue:

sudo bash deploy.sh
Sigue las instrucciones proporcionadas por el script para configurar Apache, MariaDB y la base de datos.

¡Listo! El entorno web estará desplegado y accesible en http://localhost.

Detalles del Script
Variables:

REPO: Nombre del repositorio (bootcamp-devops-2023 en este caso).
USERID: ID del usuario actual.
Colores:

Se utilizan códigos de colores para mejorar la legibilidad de las salidas del script.
Actualizaciones:

Actualiza el sistema operativo.
Verificación de Usuario ROOT:

Verifica que el script se esté ejecutando con privilegios de superusuario.
Instalación de Git:

Comprueba si Git está instalado y lo instala si es necesario.
Instalación de Apache:

Comprueba si Apache está instalado y lo instala con PHP y módulos adicionales si es necesario.
Instalación de MariaDB:

Comprueba si MariaDB está instalado y lo instala si es necesario.
Configuración de MariaDB:

Crea una base de datos, un usuario y asigna privilegios.
Carga de Datos Iniciales:

Importa datos iniciales a la base de datos desde el archivo devopstravel.sql.
Gestión del Repositorio Git:

Verifica la existencia del directorio del repositorio y lo clona si no existe. Si existe, realiza un git pull para actualizar.
Configuración de la Dirección IP en el Código:

Utiliza sed para cambiar la dirección IP en el archivo index.php a "localhost".
Recarga de Apache:

Recarga el servicio de Apache para aplicar los cambios.
Este script proporciona una forma rápida y automatizada de configurar un entorno web básico con Apache, MariaDB y Git. Asegúrate de revisar y ajustar las configuraciones según sea necesario para tu entorno específico.
