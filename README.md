# Camaron
Proyecto de Plataforma Digital de Empleos v1
🦐 Camaron YA
¡Bienvenido al repositorio oficial de Camarón Ya, la plataforma full-stack diseñada para conectar de forma rápida y segura a trabajadores independientes y empresas en Panamá!

🚀 Sobre el Proyecto
Camarón Ya es una solución tecnológica moderna que facilita la contratación de servicios y la búsqueda de empleo puntual o a corto plazo. El sistema está optimizado para ofrecer una experiencia fluida tanto en dispositivos móviles como en paneles de control profesionales de escritorio.

🛠️ Arquitectura y Tecnologías
El proyecto está desarrollado con una arquitectura Full-Stack moderna:

Frontend: Desarrollado con React y estilizado con Tailwind CSS, adaptado para ofrecer una interfaz de usuario limpia, responsiva y en formato de escritorio (Dashboard).

Backend: Construido en Python utilizando FastAPI, implementando rutas estructuradas para la gestión de usuarios, autenticación, subida de documentos y verificación por SMS.

Base de Datos: MongoDB (gestionada localmente mediante MongoDB Compass), encargada de almacenar perfiles, estados de conexión, mensajería y referencias a documentos de verificación.

✨ Características Principales
Modo Empresa y Modo Trabajador: Perfiles diferenciados para la gestión de ofertas de empleo y postulaciones.

Verificación de Identidad: Módulo integrado para la subida segura de documentos de identidad (cédula panameña, récord policivo y selfie de verificación) almacenados de forma persistente en la base de datos.

Verificación por SMS (Twilio): Sistema de validación de número telefónico mediante códigos de 6 dígitos para asegurar la autenticidad de los usuarios.

Mensajería y Chat en Tiempo Real: Canales de comunicación directos entre empresas y trabajadores para coordinar los detalles de los servicios.

Mapa Interactivo: Visualización geolocalizada de ofertas y puntos de interés en la ciudad (como Bella Vista, San Francisco, etc.).

💻 Guía de Instalación y Ejecución Local (Sin Docker)
Si estás ejecutando el proyecto en entornos locales (por ejemplo, sistemas optimizados como Windows MiniOS):

1. Configurar el Backend (Python / FastAPI)
Abre una terminal y navega a la carpeta del backend:

Bash
cd backend
Crea y activa tu entorno virtual:

Bash
python -m venv venv
# En Windows:
venv\Scripts\activate
# En Mac/Linux:
source venv/bin/activate
Instala las dependencias necesarias:

Bash
pip install -r requirements.txt
pip install python-multipart aiofiles twilio
Configura tu archivo .env conectándolo a tu instancia local de MongoDB (mongodb://localhost:27017).

Inicia el servidor con Uvicorn:

Bash
uvicorn server:app --reload --port 8000
2. Configurar el Frontend (React)
Abre una segunda terminal y navega a la carpeta del frontend:

Bash
cd frontend
Instala las dependencias:

Bash
npm install
Inicia el servidor de desarrollo:

Bash
npm start
Accede a la aplicación en tu navegador web a través de http://localhost:3000.

Consulta más detalles y notas de desarrollo en el notebook del proyecto: 💻 Camaron YA.
