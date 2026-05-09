# 🏠 Home About Project

[![Django](https://img.shields.io/badge/Django-6.0.4-green.svg)](https://www.djangoproject.com/)
[![Python](https://img.shields.io/badge/Python-3.8+-blue.svg)](https://www.python.org/)
[![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

Un proyecto web simple construido con Django que presenta páginas de inicio (Home) y acerca de (About). Este proyecto demuestra la estructura básica de una aplicación Django con vistas basadas en plantillas, navegación y diseño responsivo.

## 📋 Tabla de Contenidos

- [Características](#-características)
- [Tecnologías Utilizadas](#-tecnologías-utilizadas)
- [Requisitos Previos](#-requisitos-previos)
- [Instalación](#-instalación)
- [Configuración](#-configuración)
- [Uso](#-uso)
- [Estructura del Proyecto](#-estructura-del-proyecto)
- [Desarrollo](#-desarrollo)
- [Despliegue](#-despliegue)
- [Contribución](#-contribución)
- [Licencia](#-licencia)
- [Contacto](#-contacto)

## ✨ Características

- 🏠 **Página de Inicio**: Una página de bienvenida simple y atractiva
- ℹ️ **Página Acerca de**: Información sobre el proyecto y el desarrollador
- 🧭 **Navegación Intuitiva**: Menú de navegación fácil de usar entre páginas
- 📱 **Diseño Responsivo**: Compatible con dispositivos móviles y de escritorio
- 🎨 **Plantillas HTML**: Uso de plantillas Django con herencia
- 🔧 **Configuración Flexible**: Fácil de personalizar y extender

## 🛠 Tecnologías Utilizadas

- **Backend**: Django 6.0.4
- **Frontend**: HTML5, CSS3
- **Base de Datos**: SQLite3 (por defecto)
- **Lenguaje**: Python 3.8+
- **Dependencias**:
  - asgiref==3.11.1
  - Django==6.0.4
  - sqlparse==0.5.5
  - tzdata==2026.2

## 📋 Requisitos Previos

Antes de comenzar, asegúrate de tener instalado:

- Python 3.8 o superior
- pip (gestor de paquetes de Python)
- Git (opcional, para clonar el repositorio)

## 🚀 Instalación

Sigue estos pasos para configurar el proyecto en tu máquina local:

### 1. Clona el repositorio

```bash
git clone https://github.com/tu-usuario/home-about.git
cd home-about
```

### 2. Crea un entorno virtual

```bash
python -m venv .venv
```

### 3. Activa el entorno virtual

**En Windows:**
```bash
.venv\Scripts\activate
```

**En macOS/Linux:**
```bash
source .venv/bin/activate
```

### 4. Instala las dependencias

```bash
pip install -r requirements.txt
```

### 5. Realiza las migraciones de la base de datos

```bash
python manage.py migrate
```

### 6. Ejecuta el servidor de desarrollo

```bash
python manage.py runserver
```

¡El proyecto estará disponible en `http://127.0.0.1:8000/`!

## ⚙️ Configuración

### Variables de Entorno

Para producción, configura las siguientes variables de entorno en `base_project/settings.py`:

- `DEBUG=False`
- `SECRET_KEY`: Una clave secreta segura
- `ALLOWED_HOSTS`: Lista de hosts permitidos

### Base de Datos

Por defecto, el proyecto usa SQLite3. Para cambiar a otra base de datos, modifica la configuración en `base_project/settings.py`.

## 📖 Uso

### Navegación

- **Inicio**: `http://127.0.0.1:8000/` - Página principal
- **Acerca de**: `http://127.0.0.1:8000/about/` - Información del proyecto

### Personalización

Para personalizar el contenido:

1. Edita las plantillas en `templates/`
2. Modifica las vistas en `pages/views.py`
3. Actualiza los estilos en las plantillas HTML

## 📁 Estructura del Proyecto

```
home_about/
├── base_project/          # Configuración principal de Django
│   ├── __init__.py
│   ├── asgi.py
│   ├── settings.py       # Configuraciones del proyecto
│   ├── urls.py           # URLs principales
│   └── wsgi.py
├── pages/                 # Aplicación de páginas
│   ├── __init__.py
│   ├── admin.py
│   ├── apps.py
│   ├── models.py         # Modelos de datos (vacío por ahora)
│   ├── tests.py
│   ├── urls.py           # URLs de la aplicación
│   ├── views.py          # Vistas de las páginas
│   └── migrations/       # Migraciones de base de datos
├── templates/             # Plantillas HTML
│   ├── _base.html        # Plantilla base
│   ├── home.html         # Página de inicio
│   └── about.html        # Página acerca de
├── db.sqlite3             # Base de datos SQLite
├── manage.py              # Script de gestión de Django
├── requirements.txt       # Dependencias del proyecto
└── README.md              # Este archivo
```

## 💻 Desarrollo

### Comandos Útiles

```bash
# Crear una nueva aplicación
python manage.py startapp nueva_app

# Crear migraciones
python manage.py makemigrations

# Ejecutar pruebas
python manage.py test

# Crear superusuario
python manage.py createsuperuser
```

### Extensión del Proyecto

Para agregar nuevas páginas:

1. Crea una nueva vista en `pages/views.py`
2. Agrega la URL en `pages/urls.py`
3. Crea la plantilla correspondiente en `templates/`

## 🌐 Despliegue

Para desplegar en producción:

1. Configura un servidor web (Apache, Nginx)
2. Usa un servidor WSGI (Gunicorn, uWSGI)
3. Configura variables de entorno seguras
4. Ejecuta migraciones en el servidor
5. Recopila archivos estáticos: `python manage.py collectstatic`

## 🤝 Contribución

¡Las contribuciones son bienvenidas! Para contribuir:

1. Haz un fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/AmazingFeature`)
3. Commit tus cambios (`git commit -m 'Add some AmazingFeature'`)
4. Push a la rama (`git push origin feature/AmazingFeature`)
5. Abre un Pull Request

### Guías de Contribución

- Sigue las convenciones de código de Django
- Escribe pruebas para nuevas funcionalidades
- Actualiza la documentación según sea necesario

## 📄 Licencia

Este proyecto está bajo la Licencia MIT. Ver el archivo `LICENSE` para más detalles.

## 📞 Contacto

- **Autor**: Tu Nombre
- **Email**: tu.email@ejemplo.com
- **GitHub**: [tu-usuario](https://github.com/tu-usuario)
- **LinkedIn**: [Tu Perfil](https://linkedin.com/in/tu-perfil)

---

⭐ Si te gusta este proyecto, ¡dale una estrella en GitHub!

*Última actualización: Mayo 2026*</content>
<parameter name="filePath">c:\home_about\README.md