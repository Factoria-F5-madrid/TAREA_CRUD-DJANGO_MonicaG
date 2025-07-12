Parte 1: Aplicación CRUD y Django

1. ¿Qué es un CRUD y cuál es su propósito en el desarrollo de aplicaciones web?

CRUD es un acronimo que significa Create, Read, Update y Delete. (Crear, leer, Actualizar y Eliminar).
Su proposito en el desarrollo web:
- Proveer a los usuarios una forma de gestionar informacion.
- Facilitar la interaccion entre la interfaz de usuario y la base de datos.
- Constituir la base de la funcionalidad de la mayoria de las aplicaciones web.

2. ¿Qué son los patrones de arquitectura en desarrollo de software?
Son como planos o recetas que te dicen como dividir tu programa en partes y como esas partes se comunican entre si.

¿Qué es el patrón MVC (Modelo–Vista–Controlador)?
Divide el trabajo para que funcione mejor, tu eres el controlador.

¿Qué es el patrón MVT (Modelo–Vista–Template)?
Es como un equipo que trabaja en orden para mostrarte la informacion de una forma linda y organizada.

Diferencias entre MVC y MVT.

| Parte              | MVC (Modelo–Vista–Controlador)     | MVT (Modelo–Vista–Template - usado en Django)   |
| ------------------ | ---------------------------------- | ----------------------------------------------- |
| 🧠 **Modelo**      | Maneja los datos                   | Igual, maneja los datos                         |
| 🎮 **Controlador** | Controla la lógica y conecta todo  | Django lo maneja por vos (lo hace internamente) |
| 🖼️ **Vista**      | Lo que el usuario ve (la interfaz) | Recibe los datos y los manda al template        |
| 📄 **Template**    | No existe (la Vista ya muestra)    | Es la parte visual que ve el usuario (HTML)     |

¿Cuál de estos dos patrones se usa en Django?
En Django se usa el patrón MVT (Modelo – Vista – Template).

3. ¿Cómo se estructura un proyecto en Django? Explicar brevemente el rol de los modelos, vistas, templates y URLs.
Cuando haces una página con Django, todo se divide en partes para que sea fácil de manejar. Estas partes principales son:

    1. Modelos (models.py)
    Es donde se guardan los datos.
    Por ejemplo: si tu página es una tienda, aquí guardás los productos, sus precios, y detalles.

    2. Vistas (views.py)
    Es lo que recibe lo que pedís en la página (como hacer clic en un botón).
    Decide qué datos mostrar y cómo mandarlos para que los veas.

    3. Templates (plantillas HTML)
    Son las páginas que realmente ves en tu navegador.
    Aquí se pone el diseño, colores, textos y todo lo que el usuario ve.

    4. URLs (urls.py)
    Son las direcciones de la página web.
    Por ejemplo: cuando entras a www.mipagina.com/productos, las URLs dicen qué vista tiene que trabajar para mostrar esa página.

¿Para qué se usa el signo “%%” en los templates?
Se usa para poner instrucciones o comandos.

4. ¿Cuál es el flujo de datos entre un formulario HTML y la base de datos en Django?
    Formulario → Django recibe y revisa → guarda en base de datos → muestra resultado

5. ¿Qué herramientas o comandos ofrece Django para facilitar el desarrollo de un CRUD, para qué es cada una? 
(Por ejemplo: startapp, makemigrations, migrate, runserver, ModelForm, admin, etc.)

| Herramienta/Comando | Para qué sirve                           |
| ------------------- | ---------------------------------------- |
| `startapp`          | Crear una nueva app                      |
| `makemigrations`    | Preparar cambios en la base de datos     |
| `migrate`           | Aplicar esos cambios en la base de datos |
| `runserver`         | Probar la app en el navegador            |
| `ModelForm`         | Crear formularios basados en modelos     |
| `admin`             | Manejar datos fácilmente desde una web   |

6. ¿Cómo funciona el Admin de Django?

- Hacés un modelo Producto con nombre y precio.

- Registrás Producto en admin.py.

- Creás un superusuario con python manage.py createsuperuser.

- Entrás a /admin en tu navegador, ponés usuario y contraseña.

- Ahí ves todos los productos, podés agregar, cambiar o borrar.

