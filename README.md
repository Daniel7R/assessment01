# Assessment
Este es el preview de las herramientas usadas en el stack de desarrollo, de manera local se hace uso de docker compose con todas la configuraciones necesarias para trabajar de manera local, las cuales, se listan algunas de ellas y ya la herramienta donde se despliega.

## RabbitMQ/LAVINMQ
Para el tema del broker de mensajeria se usa la plataforma [CloudAMQP](https://api.cloudamqp.com/console/d248565a-bcac-410f-8658-6c644aea6dad/details), que usa LAVINMQ, una alternativa a RabbitMQ, para acceder a la herramienta se hace por medio del siguiente enlace: [LavinMQ](https://campbell.lmq.cloudamqp.com/), por defecto al ser una herramienta gratuita, se limita la creacion de Host Virtuales, asi que se crea un virtual host que es a su vez el mismo nombre de usuario de conexion


## Neon(PostgreSQL)
Para las bases de datos, se hace uso de la plataforma [Neon](https://neon.tech/), la cual permite el aprovisionamiento de hasta 10 proyectos/bases de datos Postgres gratuitas, con el fin de tener la persistencia de datos requerida dentro de la solucion.

## Redis
Para cacheo de cierta informacion se hace uso de Redis de manera gratuita, dentro de la plataforma [UpStash](https://upstash.com/) que tiene una capa gratuita de la cual se puede hace uso con ciertas limitaciones, como lo son comandos ejecutados al mes, que son alrededor de 500k, un ancho de banda de 50GB, 100 conexiones y almacenamiento de 250MB, [platafoma](https://console.upstash.com/redis/15be349d-26a3-4db1-8435-84f3686cdfde?teamid=0)

## GitHub Actions
Se hace uso de GitHub Actions como alternativa gratuita de solucion DevOps, para poder desplegar las soluciones de los diferentes microservicios que fueron realizados en este proyecto, a modo de inicio, la idea seria desplegar los ms de acuerdo al Dockerfile de las solucion hacia [Render](https://render.com/), antes de desplegar las imagenes, se hacen los respectivos tests, una vez sean exitosos se hace el push de los cambios para que render haga la construccion de la imagen.




REFERENCIA: [GitHub Actions CI/CD Pipeline for Deploying .NET Web API to Amazon ECS](https://codewithmukesh.com/blog/github-actions-deploy-dotnet-webapi-to-amazon-ecs/)
