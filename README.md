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

#### **01 Cadenas**

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

#### **02 Tuplas**

Considérese la siguiente tupla:
## Tupla de ejemplo
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

#### **03 Listas**

Crea una lista a_lit con los siguientes elementos 1, hello, [1,2,3] y True.

R = a_list = [1, 'hello', [1, 2, 3] , True] // a_list

Encuentra el valor almacenado en el índice 1 de a_list.

R = a_list[1]

Obtén el elemento almacenado en el índice 1, 2 y 3 de a_list.

R = a_list[1:4]

Concatena las siguientes listas A = [1, 'a'] y B = [2, 1, 'd']:

R = A = [1, 'a']  // B = [2, 1, 'd'] // A + B

#### **04 Conjuntos**
Transformar la lista ['rap','house','electronic music', 'rap'] en un conjunto:

R = set(['rap','house','electronic music','rap'])

Considera que la lista A = [1, 2, 2, 1] y el conjunto B = set([1, 2, 2, 1])suman sum(A) = sum(B)

R = A = [1, 2, 2, 1]  // B = set([1, 2, 2, 1]) // print("the sum of A is:", sum(A)) // print("the sum of B is:", sum(B))

Crea un nuevo conjunto album_set3 que sea la unión de album_set1 y album_set2:
album_set1 = set(["Thriller", 'AC/DC', 'Back in Black'])
album_set2 = set([ "AC/DC", "Back in Black", "The Dark Side of the Moon"])

R = album_set3 = album_set1.union(album_set2) // album_set3

Averigua si album_set1 es un subconjunto de album_set3:

R = album_set1.issubset(album_set3)

#### **05 Diccionarios**

Necesitarás este diccionario para las siguientes dos preguntas:
soundtrack_dic = {"The Bodyguard":"1992", "Saturday Night Fever":"1977"}
soundtrack_dic 
a) En el diccionario <code>soundtrack_dict</code>. ¿Cuáles son las llaves?

R = soundtrack_dic.keys() 

b) En el diccionario <code>soundtrack_dict</code>. ¿Cuáles son los valores?

R = soundtrack_dic.values() 

Necesitarás este diccionario para las siguientes preguntas:
Los discos Back in Black, The Bodyguard y Thriller poseen el siguiente record de ventas en millones, 50, 50 y 65 respectivamente:

a) Crea un diccionario album_sales_dict donde las llaves sean el nombre del disco y los valores la cantidad de ventas en millones.

R = album_sales_dict = {"The Bodyguard":50, "Back in Black":50, "Thriller":65}

b) Usa el diccionario para encontrar las ventas totales de Thriller:

R = album_sales_dict["Thriller"]

c) Encuentra los nombres de los discos dentro del diccionario mediante el método keys:

R = album_sales_dict.keys()

d) Encuentra los records de ventas dentro del diccionario mediante el método values:

R =  album_sales_dict.values()

#### **06 Condiciones**

Escribe una declaración if que determine si un disco musical tiene una calificación mayor a 8. Compruébalo utilizando el calificación del disco <b>“Back in Black”</b> el cual tiene un valor de 8.5. Si la condición es verdadera, imprime “"This album is Amazing!"”

R = rating = 8.5 // if rating > 8: // print ("This album is Amazing!")

Escribe una declaración if-else que determine lo siguiente. Si la calificación es mayor que 8 imprime “this album is amazing”. Si es menor o igual a 8 que imprima “this album is ok”.

R = rating = 8.5 // if rating > 8: // print ("this album is amazing") // else: print ("this album is ok")

Escribe una declaración if que determine si un disco fue lanzado antes de 1980 o en los años 1991 o 1993. Si la condición es verdadera imprime el año de lanzamiento.

R = album_year = 1979 // if album_year < 1980 or album_year == 1991 or album_year == 1993: // print ("this album came out already")

#### **07 Bucles**

Escribe un bucle <code>for</code> que imprima todos los elementos entre <b>-5</b> y <b>5</b> usando la función range.

R = for i in range(-5, 6): // print(i)

Imprime los elementos de la siguiente lista: Genres=[ 'rock', 'R&B', 'Soundtrack', 'R&B', 'soul', 'pop'] Y asegúrate de seguir las convenciones del lenguaje Python

R = Genres = ['rock', 'R&B', 'Soundtrack', 'R&B', 'soul', 'pop'] // for Genre in Genres: // print(Genre)

Escribe un bucle for que imprima la siguiente lista: squares=['red', 'yellow', 'green', 'purple', 'blue']

R = squares=['red', 'yellow', 'green', 'purple', 'blue'] // for square in squares: // print(square)

Escribe un bucle while que muestre los valores de la calificación de las canciones de un disco almacenados en la lista <code>PlayListRatings</code>. Si la calificación es menor a 6, sal del bucle. La lista <code>PlayListRatings</code> esta compuesta por: PlayListRatings = [10, 9.5, 10, 8, 7.5, 5, 10, 10]

R = PlayListRatings = [10, 9.5, 10, 8, 7.5, 5, 10, 10] //i = 1 // Rating = PlayListRatings[0] // while(Rating >= 6): // print(Rating) // Rating = PlayListRatings[i] // i = i + 1

Escribe un bucle while que copie las cadenas 'orange' de la lista <code>squares</code> a la lista new_squares. Detente y sal del ciclo si el valor en la lista no es 'orange':

R = squares = ['orange', 'orange', 'purple', 'blue ', 'orange'] // new_squares = [] // i = 0 // while(squares[i] == 'orange'): // new_squares.append(squares[i]) // i = i + 1 // print (new_squares)

#### **08 Funciones**

Cree una función que divida la primera entrada por la segunda entrada:

R = def div(a, b): // return(a/b)

Utilice la función con  para la siguiente pregunta.

def con(a, b):
    return(a + b)

R = yes, for example: // con(2, 2)

¿Se puede usar la función <code> con </code> que definimos antes para concentrar una lista o tupla?

R = con(['a', 1], ['b', 1])

#### **09

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



        
        
