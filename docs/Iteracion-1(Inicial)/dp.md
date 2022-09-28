# Trabajo en equipo
El lider de la primera iteracion sera: Matias Fernandez

La division de las Historias de Usuario sera la siguiente:
- Crear un nuevo usuario
    - Encargados: Marcela Stigelmeier y Matias Fernandez

- Ingresar usuario
    - Encargados: Emiliano Blazco y Ariel Cristaldo

- Registrar propiedad
    - Encargados: Marcela Stigelmeier, Matias Fernandez, Emiliano Blazco, Ariel Cristaldo, Guillermo Quintana, Marcelo Kachuk 

- Modificar propiedad
    - Encargados: Guillermo Quintana, Marcelo Kachuk 

# Diseño OO

# Wireframe y caso de uso

Wireframe Registrar Usuario

![](https://github.com/guille1093/SpringWebApp-POO2/raw/master/src/main/webapp/static/img/md/scrshot1.png) 

<br><br>
**Caso de Uso**: Registar Usuario <br>
**Descripción**:  El usuario quiere crear un nombre de usuario y contraseña para poder ingresar al sistema, se <br> dirige a la sección  “Iniciar sesión” luego a la parte inferior en “cree una cuenta” donde deberá completar los <br> campos requeridos (E-Mail, DNI, Nombre, Apellido, Contraseña) de esta manera podrá generar su usuario y contraseña. <br>
**Precondición**:Disponer de un E-Mail válido <br>
**Postcondición**:--- <br>


**Flujo Típico de eventos**:
<table>
  <tr>
    <th>Actor</th>
    <th>Sistema</th>
  </tr>
  <tr>
    <td><b>1</b>.Este caso de uso comienza cuando el usuario <br> se dirije al apartado "Cree una cuenta" </td>
      <td></td>
  </tr>
  <tr>
    <td></td>
      <td><b>2</b>.El sistema despliega un formulario de <br> Identificación con seis campos:
    <br>Campo-1: E-mail
    <br>Campo-2: DNI
    <br>Campo-3: Nombre
    <br>Campo-4: Apellido
    <br>Campo-5: Contraseña
    <br>Campo-6: Confirme su cotraseña</td>
  </tr>
  <tr>
    <td><b>3</b>. El usuario selecciona el campo con la etiqueta <br> asociada “E-mail” y lo completa</td>
    <td></td>
  </tr>
  <tr> 
    <td><b>4</b>. El usuario selecciona el campo con la etiqueta <br>asociada “DNI” y lo <br>completa</td>
    <td></td>
  <tr>
       <td><b>5</b>. El usuario selecciona el campo con la etiqueta<br> asociada “Nombre” y lo <br>completa</td>
    <td></td>
  <tr>
       <td><b>6</b>. El usuario selecciona el campo con la etiqueta <br>asociada “Apellido”  y lo <br>completa</td>
    <td></td>
  <tr>
       <td><b>7</b>. El usuario selecciona el campo con la etiqueta <br> asociada “Contraseña” y lo <br>completa</td>
    <td></td>
  <tr>
       <td><b>8</b>. El usuario selecciona el campo con la etiqueta <br> asociada “Confirme su contraseña” y lo completa</td>
    <td></td>
  <tr>
    <td><b>9</b>. El usuario presiona sobre el botón con la <br> etiqueta “REGISTRARME”</td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td><b>10</b>. El sistema valida los campos cargados <br>y muestra el mensaje <br> "Registro exitoso" el cual contiene un boton <br> con la etiqueta "OK"</td>
  <tr>
    <td><b>11</b>. El usuario presiona sobre el botón con <br> la etiqueta “OK”</td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td><b>12</b>. El sistema redirecciona al usuario a la pantalla <br> del apartado “Iniciar sesión” (Al login)
</td>
 </tr>
</table>

**Flujo Alternativo de Eventos**.  

**Paso 8**:  El sistema detecta que la contraseña ingresada en el campo “Confirme su contraseña”no coincide con la del <br> campo “Contraseña”. Muestra un mensaje de error y remarca con color rojo el cuadro con la contraseña errónea.

Wireframe Ingresar Usuario

![](https://github.com/guille1093/SpringWebApp-POO2/raw/master/src/main/webapp/static/img/md/scrshot1.png)  

<br><br>
**Caso de uso**: Ingresar Usuario  
**Descripción**: El usuario quiere ingresar a su cuenta ya creada en la plataforma, se dirige al apartado de Inicio de Sesión e ingresa los datos de su cuenta.  
**Precondición**:Tener una cuenta registrada   
**Postcondición**:---  

**Flujo Típico de eventos**:
<table>
  <tr>
    <th>Actor</th>
    <th>Sistema</th>
  </tr>
  <tr>
    <td><b>1</b>. Este caso de uso comienza cuando <br>el usuario se dirige al apartado de <br>“Inicio de  Sesion”</td>
    <td></td>
  </tr>
  <tr>
    <td></td>
    <td><b>2</b>. El sistema despliega un formulario de <br>Identificación con dos campos los <br>cuales tienen asociado la etiqueta de
    <br>Campo-1: Usuario o E-mail
    <br>Campo-2: Contraseña</td>
  </tr>
  <tr>
    <td><b>3</b>. El usuario selecciona el campo con la etiqueta asociada “Usuario o E-mail” <br>y lo completa</td>
    <td></td>
  </tr>
  <tr>
    <td><b>4</b>. El usuario selecciona el campo con la <br>etiqueta asociada “Contraseña” y lo <br>completa</td>
    <td></td>
  <tr>
    <td><b>5</b>. El usuario presiona sobre el botón con la etiqueta “Iniciar Sesión”</td>
    <td></td>
    
  </tr>
  <tr>
    <td></td>
    <td><b>6</b>. El sistema valida los campos cargados <br>y redirecciona al usuario a la pantalla principal con su cuenta cargada</td>
 </tr>
</table>

**Flujo Alternativo de Eventos**.  

**Paso 2**: El sistema no logra cargar los campos. Se reinicia la interfaz  
**Paso 4.1**: El sistema detecta que se cargó un usuario erróneo en el campo “Usuario o E-mail”. Muestra un mensaje de error y remarca con color rojo el cuadro con el usuario erróneo  
**Paso 4.2**: El sistema detecta que la contraseña ingresada no coincide con el usuario . Muestra un mensaje de error y remarca con color rojo el cuadro con la contraseña errónea



# Backlog de iteraciones
**Iteracion 1**
- Crear un nuevo usuario
- Ingresar usuario
- Registrar propiedad
- Modificar propiedad


# Tareas
**Tareas para Ingresar usuario**

**Como** Inquilino/Propietario/Administrador  
**Quiero** poder ingresar mi nombre de usuario y contraseña  
**Para** poder hacer uso de las funcionalidades del sistema e ingresar a las características relacionadas a mi cuenta

<u>Criterios de aceptación</u>

- El nombre de usuario debe existir dentro de la base de datos  
- Cuando el ingreso del usuario y contraseña son correctos, entonces el sistema permitirá el ingreso  
- Si el usuario ingresa una contraseña incorrecta, el sistema mostrara la opcion de restablecer contraseña

<u>Las siguientes tareas comprenderán el desarrollo de la Historia de Usuario:</u>

- Creación de wireframe
    - Creación del formulario donde contendrán los siguientes elementos
        - Posicionamiento de campo de texto para completar “Usuario”
        - Posicionamiento de campo de texto para completar “Contraseña”
        - Boton de accion de “Iniciar Sesión” para enviar el formulario
- Descripción del Uso del wireframe (Caso de Uso real)
- Creación del modelo de datos(Entidad/es de Base de datos)
- Establecer funcion de envio de formulario 
- Validación de campos con sus respectivas alertas

**Tareas para Registrar usuario**

**Como** Inquilino/Propietario/Administrador  
**Quiero** poder crear una nueva cuenta  
**Para** poder hacer uso de las funcionalidades del sistema

<u>Criterios de aceptación</u>

 - Cuando el usuario intente ingresar a una URL o pantalla en la que no tenga permiso, entonces el sistema <br> se direccionará a la pantalla de registro del sistema.
 - La contraseña del usuario debe tener como mínimo 8 dígitos y como máximo 16
 - El nombre de usuario no debe contener caracteres especiales


<u>Las siguientes tareas comprenderán el desarrollo de la Historia de Usuario:</u>

- Creación de wireframe
    - Creación del formulario donde contendrán los siguientes elementos
        - Posicionamiento de campo de texto para completar “E-Mail”
        - Posicionamiento de campo de texto para completar “DNI"
        - Posicionamiento de campo de texto para completar “Nombre”
        - Posicionamiento de campo de texto para completar “Apellido”
        - Posicionamiento de campo de texto para completar “contraseña”
        - Posicionamiento de campo de texto para completar “Confirmar contraseña”
        -  Boton de accion de “Registrarme” para enviar el formulario
- Descripción del Uso del wireframe (Caso de Uso real)
- Creación del modelo de datos(Entidad/es de Base de datos)
- Establecer funcion de envio de formulario 
- Validación de campos con sus respectivas alertas

# Retrospectiva


