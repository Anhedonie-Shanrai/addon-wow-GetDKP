#####################################################
# GetDKP Plus
# Autores: Charla, Corgan, WalleniuM, Sylna
# $Cambiado por �ltima vez: 2009-03-09 17:16:25 +0100 (lun, 09 mar 2009) $
# $�ltimo cambio por: sylna $
#####################################################

Foro de soporte: http://www.eqdkp-plus.com/e107_plugins/forum/forum_viewforum.php?12

---------------------

-> Espa�ol <- 
Description:
===============

Hacer que la informaci�n de los DKP est� en el juego ya no ser� un problema.
El addon muestra los puntos DKP de todos los jugadores que est�n en tu EQDKP. Puede buscar jugadores, clases o armaduras.
Si tu, por ejemplo, haces click en un objeto que aparece en el chat ver�s un tooltip mostrando qui�n ha recibido ya este objeto.

Hay un m�dulo de subasta llamado "Bet and Win" para distribuir el bot�n en tu banda a trav�s de subastas. Hay 3 reglas diferentes para subastas por el momento. Tambi�n puedes anunciar el ganador en el chat de la banda

Con LiveDKP puedes modificar los DKP de los jugadores dentro del juego durante la banda para tener la lista siempre actualizada.

Hay un men� de configuraci�n para que puedas ajustarlo a tus necesidades.

Caracter�sticas:
- soporte para MultiDKP
- soporte para personajes especiales
- �susurra a alguien que tenga el addon y obt�n tus DKP!
- muestra todos los objetos que han sido introducidos en EQDKP
- al hacer click en un objeto que se haya puesto en el chat y haya sido introducido en el EQDKP, aparecer� un tooltip. Mostrar� qui�n ha recibido este objeto y por cuantos puntos. Tambi�n ver�s quien necesita este objeto a�n.
Esta informaci�n se puede poenr en los canales de banda/grupo/hermandad.
- muestra todos los objetos y sus precios en DKP que est�n en tu EQDKP. 
- b�squeda por nombre de objetos
- b�squeda por objetos de jugadores
- muestra la posibilidad de obtener un conjunto de objetos
- muestra detallada de los precios de objetos. Para sistemas DKP con distintos precios de objetos, se mostrar�n min/max/media de los precios
- susurro de clase/armadura
- Opci�n para mostrar s�lo los jugadores en Banda
- Ocultar los susurros realizados
- Mostrar jugador de tu banda en el Tooltip de un Objeto incluso si no tienen DKP (si tienes invitados en la banda)
- Peticiones de susurros para jugadores y objetos est�n desactivadas cuando est�s en un combate
- Puedes establecer un l�mite de cuantos jugadores deber�an mostrarse en el Tooltip.
- �Todas las opciones se pueden poner en TitanPanel!
- A�adir o quitar puntos DKP a un jugador


Instalaci�n
===============

Descarga y copia la carpeta de GetDKP en tu carpeta xxx\World of Warcraft\Interface\AddOns\ . 

Teniendo en cuenta que WoW no permite ning�n acceso de los archivos a Internet o a archivos de tu disco duro, tienes que actualizar los puntos una vez antes de una banda. Esto funciona usando el archivo incluido. Debes introducir las rutas en tu instalaci�n primero.

1. Descomprime GetDKP.zip y copia la carpeta GetDKP en tu carpeta /Interface/Addon . 
2. Usa el DKP.EXE (dentro de la carpeta GetDKP) para descargar la informaci�n de los DKP. Tienes que modificar la ruta para que enlace con el archivo getdkp.php y tu carpeta de WoW.
3. Inicia el juego

- Tras el primer inicio de sesi�n tendr�s que abrir el men� de configuraci�n "/gdc" e introducir tus ajustes. Antes de cada banda deber�as revisar si se ha seleccionado la cuenta correcta cuando se use MultiDKP. Si tus cuentas est�n nombradas como las bandas que est�s haciendo, la cuenta ser� autom�ticamente cambiada al entrar en la estancia.

Abrir Ventana :
===============
/gdc abre el men� de configuraci�n
/gdl abre la ventana de GetDKPList
/gdb abre el m�dulo de Bet and Win
  
Comandos dentro del juego:
===============
/gdc status									-> muestra la configuraci�n
/gdc info [chat/guild/raid/group]  			-> muestra la informaci�n de EQDKP en el canal respectivo
/gdc help									-> muestra esta tabla
/gdc whisperdkp	[on/off]					-> desactiva/activa la funci�n de susurro de los puntos DKP
/gdc whisperitems [on/off]					-> desactiva/activa la funci�n de susurro de los objetos
/gdc whisperhide [on/off] 					-> Oculta los susurros salientes cuando alguien solicita informaci�n de DKP o de Objetos
/gdc buyerslimit xx 						-> Muestra s�lo XX compradores de un objeto. XX puede ser un n�mero entre 1 y 40. 0 = todos
/gdc needlimit xx 							-> Muestra s�lo XX jugadores con NECESIDAD de ese objeto. XX puede ser un n�mero entre 1 y 40. 0 = todos
/gdc reset  								-> Esto restaurar� la configuraci�n de EQDKP (��No los datos de EQDKP!!)
/gdco [guild/group/chat/raid/officer] 		-> establece el canal donde se pondr�n los reportes de /dkp


LiveDKP
===============
/dkp+ [Spielername / Raid ] [DKP] [Kontoname]		-> F�gt dem Spieler (oder allen Spielern im Raid) xx Punkte hinzu
/dkp- [Spielername / Raid ] [DKP] [Kontoname]		-> Zieht dem Spieler (oder allen Spielern im Raid) xx Punkte ab

Ejemplo:
/dkp+ Belelros 100 DKP1 - A�ade 100 puntos DKP a Belelros en la cuenta DKP1
/dkp- Belelros 100 DKP1 - Resta 100 DKP de los puntos de Belelros en la cuenta DKP1
/dkp+ Raid 100 DKP1 - A�ade 100 puntos DKP a todos los jugadores en la banda en la cuenta DKP1

Susurros:
===============

dkp	[account]	-> Puntos DKP

Ejemplo:
El jugador Belelros tiene GetDKP instalado y quieres que te diga cuantos DKP tienes. /w Belelros dkp[nombre de cuenta]
============================================================================================
