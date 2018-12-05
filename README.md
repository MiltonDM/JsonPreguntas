# JsonPreguntas
Realización de varias preguntas realizadas en un JSON para poderla jalar desde un servidor para poder mostrarlas en una aplicación Android donde debemos responderlas y después mandarlas a un correo donde muestre las respuestas del Test

***Integrantes Colaboradores***
>Creado por: Milton Alexis Durán Moreno.<br />
>Creado por: Diego Salvador Suarez Quijaz.<br />
>Creado por: Marco Antonio Moreno Cortes.<br />

***Correo de los contactos***
>Contacto: duran.milton.92@hotmail.com<br />
>Contacto: d.salvador0604a@gmail.com <br />
>Contacto: <br />

Desarrollar un aplicación que realize un Test (Tema libre), que se desplieguen de forma individual para que el usuario tenga una mejor vista y se pueda contestar el forma libre, plasmar un botón(JButton) que de acceso a la siguiente pregunta o poder regresar a la anterior. 
Al termino de las preguntas se debe de adjuntar las respuestas en el orden que se fueron mostrando en la interfaz, para así poder enviarlas de forma mas clara y organizada por medio de un correo electrónico y así evaluar las respuesta más fácil.
Cada pregunta de opción múltiple que se vea reflejada, solo se podrá seleccionar una opción para una mejor puntuación.
Todas la respuestas que se estén ingresando al formulario deberán estar almacenadas en un JSON en el orden que este los almacena. (Atributos, arreglos).

Descripción.
-	Presentar test tema libre.
-  crear base de datos con php.
-  donde arrojara los datos en formato de JSON.
-	Hacer uso de todos los dispositivos necesarios para una mejor vista para el usuario (JButton, EditText, RadioGroup, RadioButton, etc).
-	Cada pregunta que sea de opción múltiple, deberá de solo responder 1 respuesta de las opciones que se especifiquen.
-	Presentar dos botones que tengan la función de siguiente pregunta o pregunta anterior.
-	Adjuntar las respuestas y enviarlas por automático por correo electrónico en texto plano.
-	Poder ver el correo con las respuestas que el Usuario ingreso.

# Base de datos
```
Base de datos.
CREATE TABLE IF NOT EXISTS quiz_questions(
id bigint(20) NOT NULL AUTO_INCREMENT,
question varchar(300) NOT NULL,
possible_answers varchar(300) NOT NULL,
correct_answer int(5) NOT NULL,
PRIMARY KEY (id),
UNIQUE KEY question (question)
) ENGINE=InnoDB DEFAULT CHARSET=latin1 AUTO_INCREMENT=1 ;
```

Json
-----
```
{
   "quiz_questions":[
      {
         "id":"1",
         "question":"Que dos protocolos se utilizan para proporcionar autenticacion AAA basada en servidor",
         "possible_answers":"SSH, TACAS, SNMP, Ninguno",
         "correct_answer":"2"
      },
      {
         "id":"2",
         "question":"Cuales son las tres tecnicas para mitigar los ataques VLAN",
         "possible_answers":"deshabilitar DTP, Use VLAN privadas, Habilitar BPDU guardia, Ninguno",
         "correct_answer":"1"
      },
      {
         "id":"3",
         "question":"Cuales son tres tecnicas de mitigacion de ataques de VLAN",
         "possible_answers":"Desactiva el DTP, Usar VLAN privadas, Habilitar la proteccion de origen, Ninguno",
         "correct_answer":"1"
      },
      {
         "id":"4",
         "question":"Que version de SNMP utiliza el control de acceso basado en cadenas de comunidad debiles y adminte la recuperacion a granel",
         "possible_answers":"SNMPv3, SNMPv2c, SNMPv1, Ninguno",
         "correct_answer":"2"
      },
      {
         "id":"5",
         "question":"Que ataque a la red intenta crear un Dos para los clientes al evitar que obtenga arrendamiento de DHCP",
         "possible_answers":"Ataque de tabla CAM, Inanicion DHCP, Suplantacion de direccion, Ninguno",
         "correct_answer":"2"
      },
      {
         "id":"6",
         "question":"Cual es el campo disponible en los encabezados IPv4 e IPv6 para marcar los ataques para QoS ",
         "possible_answers":"Prioridad, ID de VLAN, Tipo de servicio, Ninguno",
         "correct_answer":"3"
      },
      {
         "id":"7",
         "question":"Que algoritmo de formacion de colas tiene una sola cola y trata a todos los paquetes por igual",
         "possible_answers":"FIFO, LLQ, WFQ, Ninguno",
         "correct_answer":"1"
      }
   ]
}
```
## Limpia de construcción
<table>
<tr>
<td><img src=https://github.com/MiltonDM/JsonPreguntas/blob/master/Clear/Sin_Limpiar.png width="225" height="270"></td>
<td><img src=https://github.com/MiltonDM/JsonPreguntas/blob/master/Clear/Clear.png width="225" height="270"></td>
<td><img src=https://github.com/MiltonDM/JsonPreguntas/blob/master/Clear/.png width="225" height="270"></td>
 
</tr>
</table>

AndroidManifest: para dar permiso de guardar y de escribir en el archivo.

    >Clase: AndroidManifest
    > 


* * *
## Referencias
**link:** https://mex.000webhost.com/<br />
**link:** https://jsonformatter.curiousconcept.com//<br />
