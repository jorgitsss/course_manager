# Proyect on Ruby on Rails -- Course Manager 
## What is REST (Representational state Transfer) ?

* It is a software architecture form managing networked applications.
 
HEAD
CONNECT
OPTIONS
TRACE

GET	  obtener indormacion
POST    añadir o crear nueva informacion
PUT	  modificar actualizacion dato existente
PATCH   modificar actualizacion parcial
DELETE  eliminar dato

***
simple 7 Controller on Ruby on Rails 

```rails
class EntryController < AuthenticatedController

def index # traer informacion
end

def show  # mostrar datos de un elemento
end

def edit # renderizar un formulario
end

def update
end

def new  # renderizar un nuevo formulario 
end

def create # crear un nuevo registro
end

def destroy  # elimina elemento simple
end

end
```
_________________________________________________________________
<dl>
  <dt>App requirements</dt>
  <dd>Build a simple app on ruby on rails to manage courses, lessons and questions.</dd>
  <dd>Courses will have 1 or more lessons, lessons will have 1 or more questions.</dd>
  <dd>We will have students and teachers, all teachers can create questions in lessons.</dd>
  <dd>We will need a homepage that will show the available courses and from there users (studenst and teachers).</dd>
  <dd>Will be able to look at the course contents and sign up.</dd>
</dl>

<dl>
## Models

* Course
	* Title
	* Description

* Lessons
	* Course_id
	* Title
	* Content

* Question
	* Lesson_id
	* Content

* Users
	* Teachers
		* First_name
		* Last_name

	* Students
		* First_name
		* Last_name
</dl>
___________________________________________________________________

## Metas y progreso de este proyecto /  Goals and progrees about this proyect 

- [x] The app used postgresql db and we used scaffold to made MVC 
- [x] models on single
- [x] controller on plural


1. - [x] Crear una nueva aplicación de Rails con el comando
```rails
rails new course_manager -d=postgresql
```
2. - [x] Generar los modelos Course, Lesson, Question, Teacher y Student con los atributos correspondientes.
3. - [ ] Agregar las relaciones entre los modelos Course, Lesson, Question, Teacher y Student.
4. - [ ] Ejecutar las migraciones con el comando rails db:migrate.
5. - [ ] Agregar datos de prueba en la base de datos para verificar que todo funciona correctamente.
6. - [ ] Crear controladores y vistas para mostrar los cursos, las lecciones, las preguntas, los profesores y los estudiantes.
7. - [ ] Agregar una página de inicio que muestre los cursos disponibles y permita a los usuarios ver los contenidos y registrarse.
8. - [ ] Agregar la funcionalidad para que los profesores puedan crear preguntas en las lecciones.
