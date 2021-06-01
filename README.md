Kata de cuenta bancaria
=================

Piense en la experiencia de su cuenta bancaria personal
En caso de duda, opte por la solución más sencilla

Requisitos
------------

Depósito y retiro
Transferir
Estado de cuenta (fecha, monto, saldo)
Impresión de estados de cuenta
Filtros de estados de cuenta (solo depósitos, retiro, fecha)

Las normas
---------

1. Un nivel de sangría por método
2. No use la palabra clave ELSE
3. Envuelva todas las primitivas y cadenas
4. Colecciones de primera clase
5. Un punto por línea
6. No abrevie
7. Mantenga todas las entidades pequeñas (50 líneas)
8. No hay clases con más de dos variables de instancia.
9. Sin captadores / definidores / propiedades

#### Para más información:

- [Object Calistenia pdf] (http://www.cs.helsinki.fi/u/luontola/tdd-2009/ext/ObjectCalisthenics.pdf)
- Object Calisthenics (libro completo), Jeff Bay en: The ThoughtWorks Anthology.
Estantería pragmática 2008
- Idea original para el kata: ¿Qué tan orientado a objetos te sientes hoy? - Krzysztof Jelski (Sesión sobre la conferencia Software Craftsmanship UK 2011)


### Mi solución (* sin terminar *)

Comenzó con la definición de una prueba de aceptación:

> Dado que un cliente realiza un depósito de 1000 el 10-01-2012
Y un depósito de 2000 el 13-01-2012
Y una retirada de 500 el 14-01-2012
Cuando imprime su extracto bancario
Entonces ella vería
fecha || crédito || débito || equilibrio
14/01/2012 || || 500,00 || 2500,00
13/01/2012 || 2000,00 || || 3000,00
10/01/2012 || 1000,00 || || 1000,00

Hágalo usted mismo primero y luego compare las soluciones.

Los archivos para mirar:

[statement_printing.story] (https://github.com/sandromancuso/Bank-kata/blob/master/src/test/resources/org/craftedsw/acceptancetests/stories/statement_printing.story)
[StatementPrintingSteps.java] (https://github.com/sandromancuso/Bank-kata/blob/master/src/test/java/org/craftedsw/acceptancetests/steps/StatementPrintingSteps.java)
[Pruebas unitarias] (https://github.com/sandromancuso/Bank-kata/tree/master/src/test/java/org/craftedsw/domain/test)
[Clases de dominio] (https://github.com/sandromancuso/Bank-kata/tree/master/src/main/java/org/craftedsw/domain)