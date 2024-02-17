

## **GitFlow for SobreCodigo**
creador de contenido:  [Gaston Ortega](https://www.instagram.com/sobrecodigo/ "Gaston Ortega")
[Ramas](https://imgur.com/uZ9KJnd)
[Main](https://imgur.com/Ns0pDJM)
[Hotfix](https://imgur.com/yXso3HN)
[Develop](https://imgur.com/DFkAkav)
[Feature](https://imgur.com/8oOjgBJ)
[Release](https://imgur.com/TYOD8if)





## Video explicativo por G. Mizael Mtz Hdz

Aprende a cómo trabajar con GitFlow en Gitlab. 
Curso 100% práctico de cómo realizar el manejo de ramas: main/develop/release/hotfix/feature/support/etc.

[GitFlow en Github](https://www.youtube.com/watch?v=LkYWop93S70 "GitFlow en Github")

Para practicar deben tener [Visual Code Studio ](https://code.visualstudio.com/ "Visual Code Studio ") y la extensión [Git Graph](https://marketplace.visualstudio.com/items?itemName=mhutchie.git-graph "Git Graph"). 
Los ejercicios son simples, orientados simplemente a como se debe gestionar las ramas en cada caso. Se simulara que somos cuatro programadores trabajando en un mismo proyecto de acuerdo a las siguientes condiciones: 


------------


#### **Cambio 1 **
**Objetivo:** Implementar inción de sesión de facebook.
**Rama de trabajo:** feature/login-con-facebook.
**Rama Origen: **develop
**Rama Destino: **develop

###### Pasos a seguir: 
indicamos en consola
-**git checkout -b develop ** para crear la rama
-**git push -u origin develop ** para traer la rama a entorno local. 
-**git checkout -b feature/login-con-facebook ** Para crear nuestra rama donde desarrollemos nuestro trabajo. 
-**touch login-con-facebook.txt **  Para crear un archivo cómo si fuera nuestro proyecto nuevo o modificado por el desarrollador. 
-**git add login-con-facebook.txt ** Agregamos los cambios realizados en el nuevo archivo. 
-**git commit -m "Se implementó nuevo inicio de sesión"** comprometemos el cambio y agregamos el comentario.
-**git push -u origin feature/login-con-facebook "**  Y subimos nuestro trabajo a la rama nueva. 

Debemos ingresar los cambios a la rama pertinente una vez este terminado nuestro desarrollo>
**repositorio>Pull request>New pull request**
**base: **develop
**compare:** feature/login-con-facebook

------------


#### **Cambio 2**
**Objetivo:** Exportar reporte de usuarios a Google drive. 
**Rama de trabajo:** feature/exportar-report-drive
**Rama Origen: **develop
**Rama Destino: **develop

###### Pasos a seguir: 
indicamos en consola
-**git checkout -b develop ** 
-**git push -u origin develop ** 
-**git checkout -b feature/exportar-report-drive**
-**touch exportar-report-drive.txt. ** 
-**git add exportar-report-drive.txt ** 
-**git commit -m "Soporte para reportes de usuarios a Google drive"** 
-**git push -u origin feature/exportar-report-drive"**  

Debemos ingresar los cambios a la rama pertinente>
**repositorio>Pull request>New pull request**
**base: **develop
**compare:** feature/exportar-report-drive





#### **Cambio 3**
**Objetivo:** Error de inicio de sesión con Linkedin (v1.1.0). 
**Rama de trabajo:** hotfix/login-linkeding
**Rama Origen: **master
**Rama Destino: **master y develop

indicamos en consola
-**git checkout -b main ** 
-**git push -u origin main ** 
-**git checkout -b feature/exportar-report-drive** 
-**touch exportar-report-drive.txt. **  
-**git add exportar-report-drive.txt **
-**git commit -m "Soporte para reportes de usuarios a Google drive"** 
-**git push -u origin feature/exportar-report-drive"**  

Debemos ingresar los cambios a la rama pertinente>
**repositorio>Pull request>New pull request**
**base: **develop
**compare:** feature/exportar-report-drive


#### **Cambio 4**
**Objetivo:** Liberar verision v1.2.0 
**Rama de trabajo:** release/v1.2.0
**Rama Origen: **develop
**Rama Destino: **master y develop
