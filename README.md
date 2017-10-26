# Asociar-subdominio-a-proyecto-hecho-en-glassfish

Primeramente habrá que crear un subdominio o carpeta raiz que apunte a tu servidor de QA o producción según sea el caso.
quedando de la siguiente manera en el firewall por ejemplo:

![dominio mmfd sems gob mx](https://user-images.githubusercontent.com/11967028/32068136-01db1664-ba4b-11e7-8212-10e30c13f243.png)

Para poder *vincular* tu proyecto montado en glassfish, y apunte a un subdominio, es necesario modificar tu virtual server de glassfish
A continuación se enmarca en color naranja la ruta en la que se desplega tu aplicación generada por el .war 

![virtual server](https://user-images.githubusercontent.com/11967028/32068449-ffe9cf2a-ba4b-11e7-97ed-08e6aa9f6e4c.png)

Al ser el puerto 80 el que escucha por defecto, se enviaría esa información directamente al dominio:

**Nota** Para que lo anterior suceda, será necesario cambiar el puerto que viene por defecto de publicación(8080) por solamente 80





