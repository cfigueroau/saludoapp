¿Qué beneficios concretos viste al automatizar la construcción con Jenkins?
Automatizar con Jenkins trajo varios beneficios: consistencia en cada construcción, detección temprana de errores gracias a pruebas automáticas, y ahorro de tiempo al eliminar tareas manuales como compilar o empaquetar. Además, facilita la integración continua en equipos, ya que cada cambio puede ser validado automáticamente.

¿Qué parte del proceso crees que sería más crítica en un equipo grande?
La integración de cambios frecuentes. En equipos grandes, donde varios desarrolladores trabajan en paralelo, es fundamental contar con validaciones automáticas en cada push. La ejecución continua de pruebas y validaciones previene conflictos y asegura estabilidad del código compartido.

¿Cómo Jenkins asegura calidad antes de hacer despliegues?
Jenkins permite automatizar pruebas unitarias, análisis de código (como SonarQube) y validaciones de compilación. Si algo falla, el pipeline se detiene, evitando que código defectuoso llegue a producción. Además, puede integrarse con revisiones de calidad como pruebas funcionales o análisis estático.

¿Qué cambiarías en este pipeline para prepararlo para producción?
Incluiría:
Análisis estático de código con herramientas como SonarQube o Checkstyle
Escaneo de seguridad con OWASP Dependency-Check
Notificaciones (Slack o correo) tras cada ejecución
Separar entornos (dev, staging, prod) y agregar una etapa de aprobación manual antes de desplegar en producción
Paralelizar pruebas para mayor eficiencia

![image](https://github.com/user-attachments/assets/d6f3babd-1198-4dfe-96f9-0cea565c5e11)

¿Qué aprendimos? ¿Qué nos sorprendió más?
Aprendimos a montar todo el flujo de integración continua con Jenkins, desde subir el código a GitHub hasta que el pipeline se ejecute con cada cambio. Ver cómo se compila, prueba y empaqueta sin que uno tenga que hacer nada manual fue muy satisfactorio. Lo que más nos sorprendió fue lo fácil que es automatizar tareas repetitivas y lo útil que resulta para detectar errores rápido. También nos dimos cuenta de lo potente que es Jenkins cuando todo está bien configurado.
