https://learn.microsoft.com/es-mx/training/modules/enterprise-governance/1-introduction

Exploración: realice estos ejercicios

Use su propia suscripción de Azure para realizar estos ejercicios de gobernanza empresarial.

## Tarea 1: Navegación por Azure

En esta tarea, aprenderá a acceder a Azure Portal y usarlo.

### UBICACION DE AZURE PORTAL

En esta tarea, accederá al entorno de laboratorio y a Azure Portal.

1. Pregunte a su instructor cómo acceder al entorno de laboratorio.

2. Después de acceder al entorno de laboratorio, vaya a Azure Portal.

3. Agregue un marcador a esta página. Usará el portal a lo largo de los laboratorios y demostraciones del curso.

4. En la esquina superior derecha del portal, seleccione su cuenta de usuario.

5. Observe que puede ver la cuenta y cambiar el directorio.

![image](https://user-images.githubusercontent.com/110675810/191337027-20e88800-6531-4683-a58c-a4555450d235.png)

6. La opción Cambiar directorio le permite acceder a las opciones Mis permisos y Ver mi factura.

7. Seleccione el icono Configuración (barra de menús superior derecha: icono de engranaje).

![image](https://user-images.githubusercontent.com/110675810/191337386-d5d2dcc2-ee9c-4261-bcae-a48d5f26d4ef.png)

8. Revise la Configuración del portal, incluida la configuración general y la configuración de idioma & región.

![image](https://user-images.githubusercontent.com/110675810/191337492-c87d3489-4005-4736-8197-91eb080b0318.png)

9. Use el cuadro de texto Buscar recursos, servicios y documentos para buscar máquinas virtuales.

![image](https://user-images.githubusercontent.com/110675810/191337665-16a096af-81d7-4956-bc09-abb0ccac8857.png)

10. Puede buscar no solo recursos generales de Azure, sino también recursos con nombre específicos.

11. Seleccione el uso del menú del portal (icono de tres barras de la esquina izquierda).

12. Observe que puede Crear un recurso, ver Todos los servicios y ver Todos los recursos.

![image](https://user-images.githubusercontent.com/110675810/191337880-eb8047bc-946d-4f31-a11a-9c0a78a47e70.png)

13. Tómese un tiempo para examinar la interfaz, buscar y explorar distintas áreas.

14. Inicie el Cloud Shell (primer icono de la barra de menú superior).

15 Observe la lista desplegable de PowerShell o Bash.

![image](https://user-images.githubusercontent.com/110675810/191338331-0f64b20f-0a82-435a-abcb-959915ec136c.png)


## Tarea 2: Asignaciones de roles de RBAC de Azure
En esta tarea, conoceremos las asignaciones de roles.

### UBICACION DE LA HOJA DE CONTROL DE ACCESO

1. Acceda a Azure Portal y seleccione un grupo de recursos. Tome nota del grupo de recursos que usa.

![image](https://user-images.githubusercontent.com/110675810/191339716-2939b062-9b79-4681-8be7-dd1efd87356f.png)

2. Seleccione la hoja Control de acceso (IAM).

![image](https://user-images.githubusercontent.com/110675810/191339816-dea9417f-f78b-4cf2-90dd-87b8a4d697a3.png)

3. Esta hoja estará disponible para muchos recursos diferentes para que pueda controlar el acceso.

### REVISION DE PERMISOS DEL ROL

1. Haga clic en la pestaña Roles (parte superior).

![image](https://user-images.githubusercontent.com/110675810/191340059-ee3fc821-55c8-4b37-8b3b-300e355fc607.png)

2. Seleccione el rol que quiera de la lista haciendo clic en el cuadro asociado situado junto al nombre del rol.

![image](https://user-images.githubusercontent.com/110675810/191340303-cdc5b274-f1f8-4bf0-964f-fd46d359c61a.png)

3. Haga clic en el vínculo Ver debajo de la columna Detalles en el extremo derecho de la página.

![image](https://user-images.githubusercontent.com/110675810/191340425-4c82fcd6-a03c-4c4f-9f5f-f31c8b62df7e.png)

4. Se muestra la vista Permisos, incluidas tres columnas, que muestran, de izquierda a derecha Tipo (por ejemplo, Otros, Lectura, Escritura y Eliminación), Permisos y Descripción.

![image](https://user-images.githubusercontent.com/110675810/191340610-03b379ee-ac8b-4212-bfad-63c53afc56d2.png)

5. Cierre la hoja Control de acceso (IAM).


## Tarea 3: Administración de bloqueos de recursos
Nota: Esta tarea requiere un grupo de recursos.

En esta tarea, crearemos bloqueos de recursos.

1. En el Portal, vaya al grupo de recursos.

2. En la sección Configuración, haga clic en Bloqueos y, a continuación, haga clic en + Agregar.

![image](https://user-images.githubusercontent.com/110675810/191341345-86edb861-4d02-4c7e-b044-b6960f54d71f.png)

3. Analice los distintos tipos de bloqueos y aplique los bloqueos en distintos niveles.

4. Cree un nuevo bloqueo con un Tipo de bloqueo de Eliminar.

![image](https://user-images.githubusercontent.com/110675810/191341612-0218cd58-86af-4792-b72e-5f030f760b02.png)

5. En la hoja Información general, haga clic en Eliminar grupo de recursos. Escriba el nombre del grupo de recursos y haga clic en Aceptar.

![image](https://user-images.githubusercontent.com/110675810/191342256-2adb0c81-ea67-489f-aeeb-69dfbba1e9d6.png)

6. Debería recibir un mensaje de error que indica que el grupo de recursos está bloqueado y no se puede eliminar.

![image](https://user-images.githubusercontent.com/110675810/191342401-84950fcd-d269-4224-a349-6a270b0bd5cb.png)

7. Agregue una cuenta de almacenamiento al grupo de recursos.

![image](https://user-images.githubusercontent.com/110675810/191343302-82423980-3992-411d-aa2f-ebbadfc2e58a.png)

8. Una vez creada la cuenta de almacenamiento, intente eliminarla.

![image](https://user-images.githubusercontent.com/110675810/191343447-60143f40-29db-4dde-8e96-c42c0ef93cd4.png)

9. Recibirá un mensaje de error que indica que el recurso o su elemento primario tiene un bloqueo de eliminación.

![image](https://user-images.githubusercontent.com/110675810/191343522-34a36594-2485-4774-8706-21dc3ff12668.png)

10. Revisa cómo hereda la cuenta de almacenamiento el bloqueo del elemento primario y no se puede eliminar.

11. Vuelva a la hoja del grupo de recursos y, en la Configuración, haga clic en Bloqueos.

![image](https://user-images.githubusercontent.com/110675810/191343708-3b6aa107-6c15-48a2-85d4-660d3e5f478c.png)

12. Desplácese hasta la derecha y haga clic en el vínculo Eliminar situado a la derecha del bloqueo.

![image](https://user-images.githubusercontent.com/110675810/191343849-ab4ce470-237a-4973-8f26-9504a5568161.png)

![image](https://user-images.githubusercontent.com/110675810/191343924-d6b0001a-a9e7-40f4-b8b9-e0882f79283b.png)

13. Vuelva a la cuenta de almacenamiento y confirme que ahora puede eliminar el recurso.

![image](https://user-images.githubusercontent.com/110675810/191344051-1c6c9353-e161-4606-ade9-80f2dfe06efc.png)

![image](https://user-images.githubusercontent.com/110675810/191344161-6e7d56f5-8033-4914-912a-59924abfbb02.png)


Contenidos
Características y licencias de Azure AD Multi-Factor Authentication
https://learn.microsoft.com/es-mx/azure/active-directory/authentication/concept-mfa-licensing

Extras
Examen de prueba - Kahoot!
Examen del módulo 1
https://kahoot.it/challenge/17c998c7-d2ca-4aad-8555-25d087dca7da_1662227486074
