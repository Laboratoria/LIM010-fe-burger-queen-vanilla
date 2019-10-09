# Burger Queen

## Preámbulo

La tecnologia poco a poco ha invadido nuestras vidas desde la forma en la que nos comunicamos con nuestro entorno hasta sectores como la medicina, educacion, comida, etc... Asi que la era digital ha llegado para quedarse y los negocios no quieren quedarse fuera de esta tranformacion.

Hoy en dia se emplea la tecnologia para desarrollar software que ayude a automatizar y agilizar procesos para mejorar la experiencia de sus usuarios, este el caso de Burger Queen un negocio de comida rapida que desea mejorar el proceso de realizar pedidos de sus clientes para brindar una mejor experiencia tanto a sus colaboradores como a sus clientes.

## Resumen del proyecto

Esta vez tenemos un proyecto 100% por encargo. Si bien siempre puedes (y debes)
hacer sugerencias de mejoras y/o cambios, muchas veces trabajarás en proyectos
en los que primero hay que asegurarse de cumplir con lo requerido.

Un pequeño restaurante de hamburguesas, que está creciendo, necesita una
interfaz en la que puedan tomar pedidos usando una _tablet_, y enviarlos
a la cocina para que se preparen ordenada y eficientemente (a través de un
  _backend_ del que nos darán detalles más adelante).

![burger-queen](https://user-images.githubusercontent.com/110297/42118136-996b4a52-7bc6-11e8-8a03-ada078754715.jpg)

Esta es la información que tenemos del cliente:

> Somos **Burguer Queen**, una cadena de comida 24hrs.
>
> Nuestra propuesta de servicio 24hrs ha tenido muy buena acogida y, para
> seguir creciendo, necesitamos un sistema que nos ayude a tomar los pedidos de
> nuestros clientes.
>
> Tenemos 2 menús: uno muy sencillo para el desayuno:
>
> | Ítem                      |Precio $|
> |---------------------------|------|
> | Café americano            |    5 |
> | Café con leche            |    7 |
> | Sandwich de jamón y queso |   10 |
> | Jugo de frutas natural    |    7 |
>
> Y otro menú para el resto del día:
>
> | Ítem                      |Precio|
> |---------------------------|------|
> |**Hamburguesas**           |   **$**   |
> |Hamburguesa simple         |    10|
> |Hamburguesa doble          |    15|
> |**Acompañamientos**        |   **$**   |
> |Papas fritas               |     5|
> |Aros de cebolla            |     5|
> |**Para tomar**             |   **$**   |
> |Agua 500ml                 |     5|
> |Agua 750ml                 |     7|
> |Bebida/gaseosa 500ml       |     7|
> |Bebida/gaseosa 750ml       |     10|
>
> **Importante:** Lxs clientes pueden escoger entre hamburguesas de res,
> de pollo, o vegetariana. Además, por $ 1 adicional, pueden agregarle queso
> o huevo.
>
> Nuestros clientes son bastante indecisos, por lo que es muy común que cambien
> el pedido varias veces antes de finalizarlo.

La interfaz debe mostrar los dos menús (desayuno y resto del día), cada uno
con todos sus _productos_. El usuario debe poder ir eligiendo qué _productos_
agregar y la interfaz debe ir mostrando el _resumen del pedido_ con el
costo total.

![out](https://user-images.githubusercontent.com/110297/45984241-b8b51c00-c025-11e8-8fa4-a390016bee9d.gif)

## Objetivos de aprendizaje

El objetivo de este proyecto es construir una Single-Page Application [SPA](https://dzone.com/articles/how-single-page-web-applications-actually-work) ([versión traducida](https://dzone.com/articles/how-single-page-web-applications-actually-work)), responsiva en la que podamos escribir, leer, actualizar y eliminar datos.

Para ello deberás poner en juego tu creatividad para generar ideas que lleven a una solución original y valiosa del problema, trabajando en equipo buscando feedback constante.

En otras palabras, seguirás afianzando todo lo aprendido hasta el momento, pero en particular verás:

### HTML y CSS
- [ ] HTML semántico
- [ ] CSS `flexbox`
- [ ] Sass
- [ ] Maquetación

### Frontend Development

- [ ] Componentes
- [ ] Manejo del estado

### DOM y Web APIs
- [ ] Manipulación dinámica del DOM
- [ ] Data attributes
- [ ] History API

### Javascript
- [ ] Uso de callbacks
- [ ] Consumo de Promesas
- [ ] ES modules

### Firebase
- [ ] Firestore
- [ ] Firebase Auth
- [ ] Observables
- [ ] Firebase security rules

### Testing
- [ ] Testeo de tus funciones
- [ ] Testeo asíncrono
- [ ] Mocking

### Colaboración en Github

- [ ] Branches
- [ ] Pull Requests
- [ ] Tags

### Organización en Github

- [ ] Projects
- [ ] Issues
- [ ] Labels
- [ ] Milestones

### Buenas prácticas de desarrollo
- [ ] Modularización
- [ ] Nomenclatura / Semántica
- [ ] Linting

***

## Consideraciones

Este proyecto se debe "resolver" en tríos.

Trabaja en una historia hasta terminarla antes de pasar a la siguiente. Trabaja
hasta la historia que puedas en el tiempo especificado.

La lógica del proyecto debe estar implementada completamente en JavaScript
(ES6+), HTML y CSS.

La aplicación debe ser un _Single Page App_, por lo cual deberas de implementar un sistema de rutas.
Los pedidos los tomaremos desde una
_tablet_, pero **no queremos una app nativa**, sino una web app que sea
**responsive**, por lo cual te recomendamos utilizar [`flexbox`](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
para posicionar tus elementos.

Necesitamos pensar bien en el aspecto UX de de quienes van a tomar los pedidos,
 el tamaño y aspecto de los botones, la visibilidad del estado actual del
 pedido, etc.

Deberas de guardar la información de los pedidos realizados por
lo cual te reocmendamos utilizar [Firebase](https://firebase.google.com/).

Los tests unitarios deben cubrir un mínimo del 90% de _statements_, _functions_,
_lines_ y _branches_.

Por otro lado, deberás definir la estructura de carpetas y archivos que consideres
necesaria. Por ende,
los _tests_ y el _setup_ necesario para ejecutarlos, serán hechos por ti.

## Criterios de aceptación del proyecto

### Definición del producto

El [_Product Owner_](https://www.youtube.com/watch?v=r2hU7MVIzxs&t=202s) nos presenta este _backlog_ que es el resultado de su trabajo con el cliente hasta hoy.

---------------------
#### [Historia de usuario 1] Mesero/a debe poder tomar pedido de cliente
Yo como meserx quiero tomar el pedido de un cliente para no depender de mi mala
memoria, para saber cuánto cobrar, y enviarlo a la cocina para evitar errores y
que se puedan ir preparando en orden.

##### Criterios de aceptación
Lo que debe ocurrir para que se satisfagan las necesidades del usuario)
  * Anotar nombre de cliente.
  * Agregar productos al pedido.
  * Eliminar productos.
  * Ver resumen y el total de la compra.
  * Enviar pedido a cocina (guardar en alguna base de datos).
  * Se ve y funciona bien en una _tablet_

##### Definición de terminado
Lo acordado que debe ocurrir para decir que la historia está terminada.
  * Debes haber recibido _code review_ de al menos una compañera.
  * Haces _test_ unitarios y, además, has testeado tu producto manualmente.
  * Hiciste _tests_ de usabilidad e incorporaste el _feedback_ del usuario.
  * Desplegaste tu aplicación y has etiquetado tu versión (git tag).


---------------------

#### [Historia de usuario 2] Jefe de cocina debe ver los pedidos
Yo como jefx de cocina quiero ver los pedidos de los clientes en orden y
marcar cuáles están listos para saber qué se debe cocinar y avisar a lxs meserxs
que un pedido está listo para servirlo a un cliente.

##### Criterios de aceptación
  * Ver los pedidos ordenados según se van haciendo.
  * Marcar los pedidos que se han preparado y están listos para servirse (actualizar estado en la base de datos).
  * Ver el tiempo que tomó prepara el pedido desde que llegó hasta que se
  marcó como completado.

##### Definición de terminado
  * Debes haber recibido _code review_ de al menos una compañera.
  * Haces _test_ unitarios y, además, has testeado tu producto manualmente.
  * Hiciste _tests_ de usabilidad e incorporaste el _feedback_ del usuario.
  * Desplegaste tu aplicación y has etiquetado tu versión (git tag).

---------------------

#### [Historia de usuario 3] Meserx debe ver pedidos listos para servir
Yo como meserx quiero ver los pedidos que están preparados para entregarlos
rápidamente a los clientes que las hicieron.

##### Criterios de aceptación
  * Ver listado de pedido listos para servir (actualizar estado en la base de datos).
  * Marcar pedidos que han sido entregados.

##### Definición de terminado
  * Debes haber recibido _code review_ de al menos una compañera.
  * Haces _test_ unitarios y, además, has testeado tu producto manualmente.
  * Hiciste _tests_ de usabilidad e incorporaste el _feedback_ del usuario.
  * Desplegaste tu aplicación y has etiquetado tu versión (git tag).
  * Los datos se deben mantener íntegros, incluso después de que un pedido ha
  terminado. Todo esto para poder tener estadísticas en el futuro.

---------------------
#### [Historia de usuario 4] Mesero/a debe poder ingresar al sistema, si el admin ya le ha asignado credenciales
Yo como meserx quiero poder ingresar al sistema de pedidos.

##### Criterios de aceptación
Lo que debe ocurrir para que se satisfagan las necesidades del usuario.
  * Acceder a una pantalla de login.
  * Ingresar email y contraseña.
  * Recibir mensajes de error comprensibles, dependiendo de cuál es el error con la información ingresada.
  * Ingresar al sistema de pedidos si las crendenciales son correctas.

##### Definición de terminado
Lo acordado que debe ocurrir para decir que la historia está terminada.
  * Debes haber recibido _code review_ de al menos una compañera.
  * Haces _test_ unitarios y, además, has testeado tu producto manualmente.
  * Hiciste _tests_ de usabilidad e incorporaste el _feedback_ del usuario.
  * Desplegaste tu aplicación y has etiquetado tu versión (git tag).

---------------------

#### [Historia de usuario 5] Administrador(a) de tienda debe administrar a sus trabajadorxs
Yo como administrador(a) de tienda quiero gestionar a los usuarios de 
la plataforma para mantener actualizado la informacion de mis trabajadorxs.

##### Criterios de aceptación
  * Ver listado de trabajadorxs.
  * Agregar trabajadorxs.
  * Eliminar trabajadoxs.
  * Actualizar datos de trabajadorxs.

##### Definición de terminado
  * Debes haber recibido _code review_ de al menos una compañera.
  * Haces _test_ unitarios y, además, has testeado tu producto manualmente.
  * Hiciste _tests_ de usabilidad e incorporaste el _feedback_ del usuario.
  * Desplegaste tu aplicación y has etiquetado tu versión (git tag).
  * Los datos se deben mantener íntegros, incluso después de que un pedido ha
  terminado. Todo esto para poder tener estadísticas en el futuro.

***

## Pistas / Tips

* [Firestore](https://firebase.google.com/docs/firestore)
* [`flexbox`](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
* [*sass*](https://sass-lang.com/)
* [Modulos: Export](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Sentencias/export)
* [Modulos: Import](https://developer.mozilla.org/es/docs/Web/JavaScript/Referencia/Sentencias/import)
* [Testing Firebase con mock - video](https://www.youtube.com/watch?v=06myVn41OTY&t=1s)
* [Testing Firebase con mock - repositorio](https://github.com/Danielalab/2018-2-Testing)
* [Pill SPA - video](https://www.loom.com/share/fa63a8ad0e9a43428222c15b6f6613d3)
* [Pill SPA - repositorio](https://github.com/betsyvies/bootcamp-spa)
* [Pill MVC - repositorio](https://github.com/merunga/todomvc-vanillajs)
* [Diseño web, responsive design y la importancia del mobile first - Media Click](https://www.mediaclick.es/blog/diseno-web-responsive-design-y-la-importancia-del-mobile-first/)
* [Mobile First: el enfoque actual del diseño web móvil - 1and1](https://www.1and1.es/digitalguide/paginas-web/diseno-web/mobile-first-la-nueva-tendencia-del-diseno-web/)
* [Mobile First - desarrolloweb.com](https://desarrolloweb.com/articulos/mobile-first-responsive.html)
* [Mobile First - ZURB](https://zurb.com/word/mobile-first)
* [Mobile First Is NOT Mobile Only - Nielsen Norman Group](https://www.nngroup.com/articles/mobile-first-not-mobile-only/)
