SIMPLE GENERADOR DE CONTRASEÑAS

Genera contraseñas de la longitud que usted desea con caracteres tales como letras, numeros y caracteres especiales de forma combinada. Un simple codigo en python en pocas lineas.

CODIGO:

import random 

letras = "QWERTYUIOPASDFGHJKLZXCVBNM"
numeros = "1234567890"

conjunto = letras+numeros
longitud = 16

for _ in range(100):
    code = random.sample(conjunto, longitud)
    codigo= "".join(code)
    print(codigo)
