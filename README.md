# BackupDB-PHPMailer
Script de Backup DB MySQL y PHPmailer

##Requerimientos:
Este script usa PHPmailer de manera individual para evitar fallas.
https://github.com/PHPMailer/PHPMailer

El script debe debe ser asignado a un cron job.

##Funcionalidad:
Tenemos que dar de alta los datos de la DB y los parametros SMTP de una cuenta de correo. (En caso de usar gmail, checar la opcion de aceptar aplicaciones no seguras)
https://support.google.com/accounts/answer/6010255?hl=es

Una vez puesto el cron job cada que quieran correr el script este sacara un respaldo de la db y lo enviara con la fecha de un dia antes(Esto pensado en que el cron se debe de correr muy temprano cuando no se este usando el sistema)