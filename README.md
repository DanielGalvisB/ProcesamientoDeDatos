**Daniel Galvis Betancourth**  
**Institución:** Pontificia Universidad Javeriana 
**Curso:** Procesamiento de Datos a Gran Escala  
**Fecha:** Febrero 2026

Cuadernos a resolver:
01-Cadenas
02-Tuplas
03-Listas
04-Conjuntos
05-Diccionarios
06-Condiciones
07-Bucles
08-Funciones
09-Clases
10-Bono

**01 Cadenas**
¿Cual es el valor de la variable A después de ejecutar el siguiente código?
A = "1"
R = 1

¿Cual es el valor de la variable B después de ejecutar el siguiente código?
B = "2"
R = 2

¿Cual es el valor de la variable C después de ejecutar el siguiente código?
C = A + B
R = 12

En la variable D haz uso del slicing para imprimir solo los primeros tres elementos:
D = "ABCDEFG"
R = print(D[:3]) /// print(D[0:3])

Usa un valor de stride de 2 para imprimir cada segundo elemento de la cadena E:
E = 'clocrkr1e1c1t'
R = print(E[::2])

Imprime una barra invertida:
print("\\") /// print(r" \ ")

Convierte el mayúsculas el contenido de la variable F:
F = "You are wrong"
R = F.upper()

En la variable G, encuentra el primer índice de la sub-cadena snow:
G = "Mary had a little lamb Little lamb, little lamb Mary had a little lamb \
Its fleece was white as snow And everywhere that Mary went Mary went, Mary went \
Everywhere that Mary went The lamb was sure to go"
R = G.find("snow")

En la variable G, reemplaza la sub-cadena Mary con Bob:
R = G.replace("Mary", "Bob")

**02 Tuplas**
Considérese la siguiente tupla:
# Tupla de ejemplo
genres_tuple = ("pop", "rock", "soul", "hard rock", "soft rock", \
                "R&B", "progressive rock", "disco") 
genres_tuple
Encontrar la longitud de la tupla, genres_tuple:
R = len(genres_tuple)

Accede al elemento en el índice 3:
R = genres_tuple[3]

Utiliza el slicing para obtener los índices 3, 4 y 5:
R = genres_tuple[3:6]

Encuentra los primeros dos elementos de la tupla genres_tuple:
R = genres_tuple[0:2]

Encuentra el primer índice de "disco":
R = genres_tuple.index("disco")

Genera una lista ordenada desde la tupla C_tuple=(-5, 1, -3):
R = C_tuple = (-5, 1, -3) // C_list = sorted(C_tuple) // C_list

**03 Listas**
Crea una lista a_lit con los siguientes elementos 1, hello, [1,2,3] y True.

R = a_list = [1, 'hello', [1, 2, 3] , True] // a_list

Encuentra el valor almacenado en el índice 1 de a_list.
R = a_list[1]

Obtén el elemento almacenado en el índice 1, 2 y 3 de a_list.
R = a_list[1:4]

Concatena las siguientes listas A = [1, 'a'] y B = [2, 1, 'd']:
R = A = [1, 'a']  // B = [2, 1, 'd'] // A + B

**04 Conjuntos**
Transformar la lista ['rap','house','electronic music', 'rap'] en un conjunto:
R = set(['rap','house','electronic music','rap'])

Considera que la lista A = [1, 2, 2, 1] y el conjunto B = set([1, 2, 2, 1])suman sum(A) = sum(B)

R = A = [1, 2, 2, 1]  // B = set([1, 2, 2, 1]) // print("the sum of A is:", sum(A)) // print("the sum of B is:", sum(B))

**Bono**
#### MENOR DE DOS PARES
lesser_of_two_evens(2,4) --> 2
lesser_of_two_evens(2,5) --> 5 

def lesser_of_two_evens(a, b):
    if a % 2 == 0 and b % 2 == 0:
        return min(a, b)
    else:
        return max(a, b)
#### GALLETAS DE ANIMALES
    animal_crackers('Ciudad Calor') --> True
    animal_crackers('Lugar Frio') --> False
def animal_crackers(text):
    words = text.split()
    return words[0][0].lower() == words[1][0].lower
#### HACE VEINTE
    makes_twenty(20,10) --> True
    makes_twenty(12,8) --> True
    makes_twenty(2,3) --> False
    
  def makes_twenty(n1, n2):
    return n1 == 20 or n2 == 20 or (n1 + n2) == 20
#### NIVEL 1
#### MAYÚSCULAS: Escribir una función que haga mayúscula la primera y cuarta letra de una cadena de texto
     
    old_macdonald('macdonald') --> MacDonald
    
    def old_macdonald(name):
    return name[:3].capitalize() + name[3:].capitalize()

#### REVERSA: Dada una oración, retornar la misma oración pero en reversa

    master_yoda('I am home') --> 'home am I'
    master_yoda('We are ready') --> 'ready are We'
    
Note: Revisar método .join()

    >>> "--".join(['a','b','c'])
    >>> 'a--b--c'

Resultado de .join():

    >>> " ".join(['Hello','world'])
    >>> "Hello world"

def master_yoda(text):
    words = text.split()
    return " ".join(words[::-1])
#### NIVEL 2
#### PROBLEMA 33: 

Dada una lista de enteros, retornar True si el arreglo tinene un  3  seguido por un  3 .

    has_33([1, 3, 3]) → True
    has_33([1, 3, 1, 3]) → False
    has_33([3, 1, 3]) → False
    
  def has_33(nums):
    for i in range(len(nums) - 1):
        if nums[i] == 3 and nums[i+1] == 3:
            return True
    return False

#### REPLICADOR: Dada una cadena, devuelve una cadena donde por cada carácter en el original hay tres caracteres REPETIDOS
    paper_doll('Hello') --> 'HHHeeellllllooo'
    paper_doll('Mississippi') --> 'MMMiiissssssiiippppppiii'

  def paper_doll(text):
      result = ""
      for char in text:
          result += char * 3
      return result
      
#### BLACKJACK: Dados tres enteros entre 1 y 11, si su suma es menor o igual a 21, devuelve su suma. Si su suma excede 21 *y* hay un once, reduce la suma total en 10. Finalmente, si la suma (incluso después del ajuste) excede 21, devuelve 'BUST'
    blackjack(5,6,7) --> 18
    blackjack(9,9,9) --> 'BUST'
    blackjack(9,9,11) --> 19

def blackjack(a, b, c):
    suma = a + b + c
    
    # Si la suma es <= 21, devolver la suma
    if suma <= 21:
        return suma
    
    # Si la suma excede 21 y hay un 11, reducir en 10
    if 11 in [a, b, c]:
        suma -= 10
        # Verificar si después del ajuste sigue excediendo 21
        if suma <= 21:
            return suma
    
    # Si aún excede 21, devolver 'BUST'
    return 'BUST'



        
        
