# course_manager
Proyect on Ruby on Rails -- Course Manager
 What is REST (Representational state Transfer)

* It is a software architecture form managing networked applications.
* 
HEAD
CONNECT
OPTIONS
TRACE

GET	  obtener indormacion
POST    añadir o crear nueva informacion
PUT	  modificar actualizacion dato existente
PATCH   modificar actualizacion parcial
DELETE  eliminar dato

_________________________________________________________________

Controlador sencillo en rails, con 7 acciones
Ventajas por trabajo en equipo por convenciones 

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
_________________________________________________________________

build a simple app on ruby on rails 
an aplication to manage courses.
Courses will have 1 or more lessons, lessons will have 1 or more questions.
we will have students and teachers.
teachers can create questions in lessons
we will need a homepage that will show the available courses and from there users will be able to llok at the course contents and sign up.
__________________________________________________________________

Models
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
___________________________________________________________________

 aplicacion se conecta a postgres
Iniciamos con scaffold MVC
modelos en singular
controladores en plural
