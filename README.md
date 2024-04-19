Diferencias entre ref y reactive:
ref:
ref se utiliza para envolver un valor simple, como un número, una cadena o un objeto. Esto hace que ref sea más polivalente que reactive.
Devuelve un objeto con una propiedad .value que contiene el valor envuelto.
Es útil cuando se necesita mutar directamente un valor simple de manera reactiva.


reactive:
reactive se utiliza para envolver un objeto y hacer que todas sus propiedades sean reactivas. NO puedes usar reactive con valores primitivos.
Devuelve un objeto proxy, donde todas las propiedades del objeto original se pueden acceder y mutar directamente.
Es útil cuando se necesita reactividad en un objeto completo.
