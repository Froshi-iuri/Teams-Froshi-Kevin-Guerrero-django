# Teams-Froshi-Kevin-Guerrero-django

### control equipos e inventarios


Hecho por: Kevin Guerrero, tambien conocido como froshi :b

## Requisitos e Instalación

Para ejecutar este proyecto de forma local, se puede seguir estos pasos

### 1. Clonar el proyecto y activar el entorno
```git clone https://github.com/Froshi-iuri/Teams-Froshi-Kevin-Guerrero-django.git
cd Teams-Froshi-Kevin-Guerrero-django
python -m venv envs/teams
source envs/teams/bin/activate

```
### 2. Instalar las dependencias necesarias, estan almacenadas en un archivo txt
```empty
pip install -r requirements.txt

```
### 3. Ejecutar las migraciones y crear el administrador
### el administrador se crea si o si porque no podrás tener acceso a el get ni post ni nada
```empty
python manage.py makemigrations
python manage.py migrate
python manage.py createsuperuser

```
### 4. Iniciar el servidor
```empty
python manage.py runserver

```
## Rutas del Sistema
Cuando el servidor esté corriendo, puedes acceder a:
 * **Swagger** http://127.0.0.1:8000/swagger/
 * **Login del superusuario** http://localhost:8000/api-auth/login/
*Nota: La API implementa la seguridad IsAuthenticatedOrReadOnly. Cualquiera puede ver los equipos (GET), pero necesitas iniciar sesión como superusuario para crear, editar o borrar registros (POST, PATCH, DELETE).*
*El sistema no cuenta con unos apartados funcionales como el admin*
*dado que no se necesitaba estrictamente, no fué implementada*
**dado que el sistema no cuenta con ese apartado, una vez logueado saldrá error**
**esto sucede porque no hay apartado, pero aún asi, se habrá logueado, ahora sí podrá acceder a http://127.0.0.1:8000/swagger/**
```
