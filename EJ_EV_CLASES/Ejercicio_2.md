## Problema

Una forma de poder enviar mensajes de manera secreta es encriptandolos. Existen varias maneras de hacerlo y una de ellas es por desplazamientos. En este caso lo que se hace es cambiar las letras del mensajes por las que están ciertas posiciones más adelante o atrás en el abecedario.

Se le solicita crear un programa que decifre mensajes. Los mensajes que se le ingresarán están encriptados de la siguiente forma: la primera letra del mensaje se cambió por la que está una posición a la derecha en el abecedario, la segunda letra se cambió por la que está dos posiciones a la derecha, la tercera letra por la que se encuentra tres posiciones y así sucesivamente. En caso de que los movimientos sobrepasen la cantidad de letras del abecedario, se vuelve a comenzar por el otro extremo del abecedario, por lo que después de la letra Z se vuelve a comenzar con la A, B, C... y, en el caso contrario, antes de la letra A esta la Z y luego la Y, etc.

Por ejemplo, para el mensaje `IQÑE` cada letra se desplazó una cantidad de posiciones en el abecedario hacia la derecha (avanzando en el abecedario), la cantidad de posiciones desplazadas depende de la cantidad de letras que han sido trabajadas en la palabra hasta ese punto:

I primera letra, por lo que se desplazó una posición
Q segunda letra, por lo que se desplazó dos posiciones
Ñ tercera letra, por lo que se desplazó tres posiciones
E cuarta letra, por lo que se desplazó cuatro posiciones

Por lo que para descrintarlo se debe realizar el proceso inverso. Para obtener el valor original se debe cambiar la I por la letra que está una posición a la izquierda, para el caso de la Q se debe cambiar por la que está dos posiciones a la izquierda, para la Ñ son 3 posiciones a la izquierda y la E por la que está 4 posiciones a la izquierda.

Abecedario: `ABCDEFGHIJKLMNÑOPQRSTUVWXYZ`
```
I => H (ya que la H esta 1 posición a la izquierda de la I en el abecedario)

Q => O (ya que la O esta 2 posiciones a la izquierda de la Q en el abecedario)

Ñ => L (ya que la L esta 3 posiciones a la izquierda de la Ñ en el abecedario)

E => A (ya que la A esta 4 posiciones a la izquierda de la E en el abecedario)
```
Por lo que si el mensaje de entrada es `IQÑE`, el mensaje desencriptado es `HOLA`.

Si el mensaje de entrada es `IQÑE! HNHW!` el mensaje desencriptado es `HOLA! CHAO!`. Note que para desencriptar la letra `H` del mensaje de entrada solo se desplazo 5 posiciones a la izquierda y no 7, ya que la letra `H` es la quienta letra del mensaje, no contando el signo de exclamación de cierre y el espacio que están justo antes.


## Entrada

La entrada es un único texto, con letras mayúsculas, números y símbolos.

## Salida

Debe mostrar el mensaje desencriptado. Solo se deben cambiar las letras. Los números y símbolos se deben mantener sin cambios.


###Ejemplo 1
Entrada:
```
ÑCGE JY CMANLO. GCRE UKMÁ JYNIFRHDP.
```

Salida:
```
NADA ES VERDAD. TODO ESTÁ PERMITIDO.
```

### Ejemplo 2
Entrada:
```
QQUUZK, MPVKVXQAIT, ¿HMW XN ZH ENLBSG HQ PG TICECMXRÑP? DRVT MZONCBTP CÑ MRLOUQDZ, FBQD HUKIXWOL X JZ NBFD, IXZH MV VOOUC SCKJW EU IWAY X EM VRHT, VLZX RXQUAWJQDWGÑZ WICIAEQ GI HUSXAÑXOQF OBRGL XROÑBKÑS, JOFEUGG LN FOD XÑ BPTR VX XKJAC GA TKGS XGJIMY J PX VBUYEANJ ZJ ÑSD SF JDOPG ZCURÑA.
```

Salida:
```
PORQUE, FINALMENTE, ¿QUE ES EL HOMBRE EN LA NATURALEZA? NADA RESPECTO AL INFINITO, TODO RESPECTO A LA NADA, ESTA EN MEDIO ENTRE LA NADA Y EL TODO, PERO INFINITAMENTE ALEJADO DE COMPRENDER AMBOS EXTREMOS, INCAPAZ DE VER LA NADA DE DONDE HA SIDO SACADO Y EL INFINITO EN QUE SE HALLA SUMIDO.
```

### Ejemplo 3
Entrada:
```
MC HBHKRMVMSM ZC SI QJMX, YÑ MRPÑ HBDLXT. YVTXC VA DIS WQTWFJÑ QKY X OUTD ZJF.
```

Salida:
```
LA EXCELENCIA NO ES ARTE, ES PURO HABITO. SOMOS LO QUE HACEMOS UNA Y OTRA VEZ.
```
