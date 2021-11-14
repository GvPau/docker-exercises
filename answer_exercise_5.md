# Ejercicio 5


He rellenado el fichero de docker-compose-yml con la siguiente configuración.

![title](images/hw5/dockercomposeyml.png)

Despues utilitzo el comando **docker compose up -d** para lanzar el docker-compose.yml
![title](images/hw5/creating-docker-compose.png)

Me crea la network, se baja las imagenes de elasticsearch y kibana, y crea los dos contendores.

Si ahora accedemos a http://localhost:5601 tenemos lo siguiente:
![title](images/hw5/welcome-elastic.png)

![title](images/hw5/add-data-view-data.png)
Le doy a add data y luego a view data con dashboard:

![title](images/hw5/dashboard.png)

