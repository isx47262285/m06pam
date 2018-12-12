# m06pam
examen pam roberto 

# ordenes a ejecutar con el host
docker run --name examen_host -h host --network ldapnet --privileged -it m06pam:latest 


#ordenes a ejecutar con el server
# imagen local basada en ldapserver:18group 

 docker run --rm --name ldap -h ldap --network ldapnet --privileged -d ldapserver_18roberto

# utilizamos la network creada para que haya conexion entre el server y el cliente 
