# colores.lat
Librería para imprimir a colores en Latino.
![terminal](https://github.com/lenguaje-latino/colores.lat/releases/download/img/jarriz.jarriz._020.png)

**Requiere**: Latino 

**NOTA**: si quieres restablecer el color usa el parámetro `reset` en lugar de poner el color

## Tipos de texto
```java
	bold // texto remarcado
	ligero // texto con color ligero
	italicas // texto conocido también erroneamente como "cursivas"
	subrayado // texto subrayado
	parpadea // parpadeará, pero solo en terminarles como xTerm
	marcado // color estilo marcatextos
	tachado // tacha el texto
 ```


## Colores de texto disponibles
```
	negro
	rojo
	verde
	amarillo
	azul
	purpura
	cyan
	blanco
	rosa
	naranja
 ```
 
## Remarcar el color
Uso: `r_COLOR`<br>
Ejemplo: `r_rojo`
 
## Colorear texto con formato
Tendrás que usar la letra que define cada uno de sus formatos: `b: bold, l: ligero, i: italicas, s: subrayado, p: parpadeante, m: marcado, t: tachado`.<br>
Uso: `simp("ARGUMENTOS.color")`<br>
Ejemplo:
```c
simp("bt.azul") // usé los parámetros 'b' para bold y 't' para tachado (ver arriba) y elegí el color azul
```
## Color personalizado
Imprime los colores con `colores()`<br>
Ahora nos saldrán cuadros de colores con el número de color, por ejemplo, vemos un cuadro rosa, tiene el número **162**<br>
Ahora ejecutamos el color con `color(162)`

## Ejemplo
```c
color = incluir("colores")
imprimir(color.verde.."hola"..color.reset) // imprimimos 'hola' en color verde y reseteamos el color.
imprimir(color.simp("im.azul").."hola"..color.reset) // imprimimos 'hola' con formato, eligiendo i: italicas y m: marcado
```

