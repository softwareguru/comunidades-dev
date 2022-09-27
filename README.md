# Directorio de comunidades tech en Latam

Sitio web que opera como directorio de comunidades tecnológicas en Latinoamérica.

Este repositorio contiene tiene los archivos necesarios para generar un sitio web estático con Hugo.

## Cómo contribuir

#### Contenido
Para agregar una comunidad, la forma ideal es [llenar en esta forma](https://airtable.com/shrHyiCxdnZX9oQqF) en Airtable. Es bastante sencillo, una vez que verifiquemos los datos (típicamente menos de 24 hrs), la información aparecerá en este sitio. 

#### Diseño
Si deseas contribuir al diseño o funcionamiento de este sitio, los pull requests son bienvenidos. El sitio se genera con [Hugo](https://gohugo.io/). 

1. Si tienes Hugo instalado, simplemente puedes clonar el repo, entrar al directorio raíz del repo y escribir `hugo server`, y debería obtener un mensaje de que ya puedes ver el sitio corriendo en tu localhost (típicamente en http://localhost:1313).

2. Estilo: En principio, el sitio usa Bootstrap 5 sin alteraciones. Si quieres seguir usando Bootstrap y simplemente redefinir/agregar estilos, entonces basta con que pongas estilos custom en `/themes/bootstrap-clean/assets/scss/styles.scss` . Por otro lado, si quieres reconfigurar Bootstrap con otras variables, también se puede pero requiere saber lo que haces. Y por último, si prefieres usar otro framework por completo, entonces puedes modificar `config.toml` donde se listan los archivos de CSS y Bootstrap que se están cargando, y poner los archivos del framework que quieras usar.

3. Layouts: Los layouts están bajo `themes/bootstrap-clean/layouts`. Las plantillas que tal vez te interese cambiar son:
  * `partials/header.html` - Header con título del sitio y menú de navegación
  * `partials/footer.html` - Footer
  * `comunidades/list.html` - Plantilla del listado de comunidades
  * `comunidades/single.html` - Plantilla para desplegar una comunidad
  * `index.html` - Homepage

## Atenerse a solo registrar comunidades abiertas 
Este directorio no es para promover empresas ni cursos otorgados por empresas de capacitación.

Nos reservamos el derecho de rechazar cualquier registro que consideremos que no cumple este lineamiento.
