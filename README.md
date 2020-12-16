# pwcMonitoringApp

Para correr el proyecto, se debe correar el archivo .workspace que está dentro de la carpeta example, cabe recordar que toca tener instalado el IDE de xcode para por correr la aplicación

EL proyecto tiene:
 - Es una proyecto tipo cocoa pods, realizado con el lenguaje de programación swift
 - El proyecto está como librería, eso quiere decir que se puede exportar en otros proyectos para reutilizar la funcionalidad de monitoreo en cualquier aplicación donde la requiera
 - El proyecto tiene un target de example, que es la aplicación como tal y se puede correr sin problema y hace uso de la funcionalidad que se encuentra en la librería
  - El poroyecto tiene pruebas unitarias de la librería
  - EL proyecto está consumiendo un servicio Rest que se encuentra alojado en un dominio, este servicio es un mockserver, donde se obtiene la lista de productos
    - URL rest: https://pwctestelkin-bancofuturo.free.beeceptor.com/api/getProducts
  - La revisión de las comunicaciones se está haciendo cada 30 segundos.
   - Se puede probar la app, quitando el internet y colocandolo de nuevo
   
  # Imagenes de la aplicación
| Sin comunicación      | Con productos y comunicación      |
|------------|-------------|
| <img src="https://github.com/elkinsalcedo/pwcMonitoringApp/blob/feature/monitoring/Screen%20Shot%202020-12-16%20at%2012.15.23%20AM.png" width="250"> | <img src="https://github.com/elkinsalcedo/pwcMonitoringApp/blob/feature/monitoring/Screen%20Shot%202020-12-16%20at%2012.17.09%20AM.png" width="250"> |
