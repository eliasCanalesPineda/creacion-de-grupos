# software-libre
tarea de software libre
Para iniciar la creación de usuarios ingresaremos el comando "useradd" seguido del nombre que le asignaremos, en mi caso useradd Elías.
También podemos ingresarle una contraseña al usuario con el comando passwd y el nombre de usuario que en mi caso es passwd Canales.
luego hacemos los mismos pasos con la creación de un segundo usuario que en mi caso será el nombre de mi madre, utilizando el mismo comando. useradd Armida.
Luego de ingresar el comando anterior podremos asignarle una contraseña y nos pedirá que la ingresemos nuevamente para confirmar. 
En este punto ya tendremos nuestro usuario creado.
Para verificar la existencia del usuario en el sistema ingresaremos el comando "nano /et/passwd".
Si queremos verificar la información relativa de los usuarios ingresamos el comando "nano /etc/shadow".
A continuación, la maquina nos mostrará la información correspondiente a cada uno de los usuarios existentes.
Para crear un grupo ingresaremos el comando groupadd y el nombre a asignar al grupo, por ejemplo groupadd Familia.
Si deseamos agregar usuarios a un grupo podemos realizarlo con el comando adduser nombre del usuario a agregar + nombre del grupo, adduser familia de Elias.
Luego de ejecutar el comando anterior nos mostrará un texto que indica que el usuario Elias ha sido agregado al grupo Familia.
Para verificar que los usuarios se asignaron correctamente en el grupo lo hacemos con el comando getent group + el nombre del grupo getent group Familia.
A continuación la máquina nos mostrará los nombres de los usuarios que pertenecen al grupo Familia. 
Si queremos cambiar el nombre de nuestro grupo ingresamos el comando "groupmod -n" + nombre nuevo + nombre del grupo, groupmod -n casa Familia.
Verificamos con el comando "cat /etc/group" y podemos comprobar que el nombre del grupo cambió a "casa".
