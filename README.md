# pwcMonitoringApp

Para correr el proyecto, se debe correar el archivo .workspace que está dentro de la carpeta example, cabe recordar que toca tener instalado el IDE de xcode para por correr la aplicación

EL proyecto tiene:
 - Es una proyecto tipo cocoa pods, realizado con el lenguaje de programación swift
 - El proyecto está como librería, eso quiere decir que se puede exportar en otros proyectos para reutilizar la funcionalidad de monitoreo en cualquier aplicación donde la requiera
 - El proyecto tiene un target de example, que es la aplicación como tal y se puede correr sin problema y hace uso de la funcionalidad que se encuentra en la librería
 - El proyecto en del target de aplicación utilizo una arquitectura de diseño llamada MVP, donde las capas todas son desacopladas y se comunican por medio de interfaces
  - El proyecto tiene pruebas unitarias de la librería
  - EL proyecto está consumiendo un servicio Rest que se encuentra alojado en un dominio, este servicio es un mockserver, donde se obtiene la lista de productos y devuelve un json
    - URL rest: https://run.mocky.io/v3/d729222c-64d1-449a-9bc5-04bc6ba29af9
    - JSON de ejemplo:
      {
         "ctaahorro":"Cuenta ahorros",
         "ctacorriente":"Cuenta corriente",
         "tc":"Tarjeta crÃ©dito",
         "cred":"Creditos"
     }
  - La revisión de las comunicaciones se está haciendo cada 30 segundos.
   - Se puede probar la app, quitando el internet y colocandolo de nuevo
   
  # Imagenes de la aplicación
| Sin comunicación      | Con productos y comunicación      |
|------------|-------------|
| <img src="https://github.com/elkinsalcedo/pwcMonitoringApp/blob/feature/monitoring/Screen%20Shot%202020-12-16%20at%2012.15.23%20AM.png" width="250"> | <img src="https://github.com/elkinsalcedo/pwcMonitoringApp/blob/feature/monitoring/Screen%20Shot%202020-12-16%20at%201.41.08%20AM.png" width="250"> |
