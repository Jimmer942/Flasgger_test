# Heippi Hospital RESTFUL API
<p align="center"> <img src="Logo_Heippi_Hospital.png"/> </p>
This repository is cretae to Heippi Backend Developer - Prueba técnica

**Reto**: Desarrollo de servicio web (API REST) que sirva endpoints para un sistema de gestión de
historia clínica centralizada.

**NOTA**: Este es un proyecto que evaluaremos como si fuera real aunque sea ficticio, no es necesario
enviar proyecto. Solo requerimos llamada virtual para recibir indicaciones de lo realizado.

**Requerimientos**:
	1. Permitir registro de usuarios con Identificación, Email, Teléfono y
	contraseña.
		**Condiciones**: Los tipos de usuario permitidos en registro son Hospital y Paciente.
	**Solución**:

	 **Signin pacients**
	 route: "/new-pacient/add"
	 methods allowed: POST
	 parameters: usr_cc, usr_email, usr_phone, usr_password, [usr_name], [usr_addr], [usr_birth_date]
	 Curl Example:
	 curl -d "usr_cc=00001&usr_email=jodmunozol@unal.edu.co&usr_phone=1234&usr_password=123456" -X POST http://localhost:3000/new-pacient/add

	 **Signin hospitals**
	 route: "/new-hospital/add"
	 methods allowed: POST
	 parameters: hosp_cc, hosp_email, hosp_phone, [hosp_services], [hosp_name], [hosp_addr]
	 Curl Example:
	 curl -d "hosp_cc=00002&hosp_email=834@holbertonschool.com&hosp_phone=1234&hosp_password=123456" -X POST http://localhost:3000/new-hospital/add
