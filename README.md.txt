# Mini Compilador en Python

Este proyecto implementa un compilador simplificado que procesa un lenguaje básico con soporte para variables, expresiones aritméticas y estructuras condicionales. El compilador sigue las fases clásicas:

1. Análisis Léxico: convierte el código fuente en tokens.
2. Análisis Sintáctico: valida la estructura y construye un AST.
3. Análisis Semántico: verifica tipos y uso de variables mediante una tabla de símbolos.
4. Generación de Código Intermedio: produce código de tres direcciones.

El lenguaje soporta:

* Declaración de variables (int)
* Asignaciones
* Operaciones aritméticas (+, -, *, /)
* Condicionales (if / else)
* Impresión (print)

Ejemplo de entrada:

```
int a = 5;
int b = 3;
int c;

c = a + b * 2;

if (c > 10) {
    print(c);
}
```

Salida (código intermedio):

```
t1 = b * 2
t2 = a + t1
c = t2
if c > 10 goto L1
goto L2
L1: print c
L2:
```

Este proyecto demuestra el flujo completo de un compilador educativo.
