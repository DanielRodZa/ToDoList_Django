# Lista de Tareas con Django

Este proyecto es una aplicación web de lista de tareas desarrollada con Python y el framework Django. Permite crear, leer, actualizar y eliminar tareas (CRUD).

## Características

* Creación de tareas con título y descripción.
* Marcado de tareas como completadas.
* Edición y eliminación de tareas.
* Interfaz de usuario sencilla y fácil de usar.

## Requisitos

* Python 3.x
* Django

## Instalación

1.  Clona el repositorio:

    ```bash
    git clone https://github.com/DanielRodZa/ToDoList_Django.git
    cd <nombre_del_proyecto>
    ```

2.  Crea un entorno virtual (recomendado):

    ```bash
    python -m venv venv
    source venv/bin/activate  # En Linux/macOS
    venv\Scripts\activate  # En Windows
    ```

3.  Instala las dependencias:

    ```bash
    pip install -r requirements.txt
    ```

4.  Aplica las migraciones:

    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5.  Ejecuta el servidor de desarrollo:

    ```bash
    python manage.py runserver
    ```

6.  Abre tu navegador y navega a `http://127.0.0.1:8000/tasks/`

## Estructura del Proyecto

```
todo_project/
├── manage.py
├── tasks/
│   ├── init.py
│   ├── models.py     
│   ├── views.py       
│   ├── urls.py        
│   ├── forms.py       
│   ├── templates/     
│   │   └── tasks/
│   │       ├── task_list.html
│   │       ├── task_form.html
│   │       └── task_confirm_delete.html
│   └── static/        
│       └── css/
│           ├── styles.css
│           └── normalize.css
├── todo_project/
├── init.py
├── settings.py    
├── urls.py        
├── wsgi.py
├── requirements.txt  
└── README.md         
```
## Uso

* Accede a `http://127.0.0.1:8000/tasks/` para ver la lista de tareas.
* Utiliza los enlaces para crear, editar y eliminar tareas.