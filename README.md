# Desplegando la aplicación del cine

<p>1. Lo primero que tenemos que hacer es tener docker dekstop instalado y funcionando</p>
<p>2. Creamos un contenedor de nginx con el siguiente comando:</p>

```bash
docker run -d -p 8080:80 nginx
```
Si el puerto te da problemas en vez de 8080:80 puedes poner por ejemplo 8081:80 

<p>3. Una vez creado el contenedor lo abrimos en terminal dandole a los 3 puntos y open in terminal</p>
<p>4. Dentro de la terminal nos movemos a la carpeta donde deberemos guardar nuestro html, aqui te dejo la ruta</p>

```bash
cd usr/share/nginx/
```
aqui dentro hacemos 

```bash
rm -r html
```
para borrar el html que tiene por defecto
<p>5. Con ese html ya borrado para poder meter nuestra pagina primero tendremos que asegurarnos de que la propia carpeta del proyecto se llama html y que tenemos un index.html para que lo encuentre de forma automatica</p>

<p>6. Si lo tenemos el siguiente paso seria, en el contenedor del nginx iniciado le damos a files y seguimos la ruta antes mencionada hasta la carpeta nginx donde le damos click derecho y le damos a import, nos saldra nuestro ordenador, seleccionamos nuestro proyecto y listo</p>

<p>7. Comprobamos que funciona dandole a los 3 puntos y dandole a open with browser y si todo ha salido bien deberiamos ver nuestra pagina web funcionando</p>
