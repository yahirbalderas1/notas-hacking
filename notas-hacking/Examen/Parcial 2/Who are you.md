# Solucion

Paso 1:
Meternos a inspeccionar la pagina, despues en network y eliges el primer GET
Paso 2:
Cambias los headers conforme te los vaya pidiendo en las pistas en mi caso fueron:
	"### Only people who use the official PicoBrowser are allowed on this site!"
		En este caso, se cambia el User-Agent a PicoBrowser
	"I dont trust people who can be tracked"
		Aqui se agrega una etiqueta llamada DNT "Do Not Track" y le ponemos valor 1 que es igual a verdadero
Como resultado nos da la bandera
```
**picoCTF{http_h34d3rs_v3ry_c0Ol_much_w0w_0da16bb2}**
```
