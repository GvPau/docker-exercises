# Ejercicio 1

Para definir un comando al ejecutar cuando se inicie un contenedor tenemos
dos instrucciones CMD y ENTRYPOINT.
Si utilizamos el comando CMD entonces Docker ejecutará como primer comando
el comando entrypoint por defecto, que es /bin/sh -c.
Si utilizamos el comando ENTRYPOINT estamos especificando el primer ejecutable
al inicial el contenedor.

- Por ejemplo, si tenemos:
FROM nginx
CMD["/bin/date"]
Se ejecutará al inicial el contenedor:
/bin/sh -c y luego /bin/date
Y el output será:
Data actual
- Si por otra parte tenemos:
FROM nginx
ENTRYPOINT ["bin/echo"]
CDM ["Hello"]
Se ejecuta al inicial el contenedor
/bin/echo y leuego Hello
Y el output será:
Hello

