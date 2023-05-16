# Reto 10

## Punto 1

``` python
def promedio(lista): # Se define la funcion para hallar el promedio que recibe como argumento la lista
    Suma = 0

    for elemento in lista: # Se itera sobre cada elemento que se agregue a la lista y se va sumando
        Suma += elemento
    promedio = Suma / len(lista) # Se calcula el promedio dividiendo la suma por la cantidad de elementos en la lista
    return promedio # Se retorna el resultado del promedio



if __name__ == "__main__":
    lista = [] # Se crea una lista vacia
    X = int(input("Ingrese el tamaño de la lista: ")) # Se solicita la cantidad de elementos de la lista
    for i in range(X):  #Se itera desde cero hasta el tamaño de la lista ingresado por el usuario para ir agregando valores .
        i = float(input("Valores de la lista : ")) # Se solicita cada valor de la lista 
        lista.append(i) # Se agrega cada valor a la lista
    promedio_lista = promedio(lista) # Se llama a la función promedio
    print("El promedio de los números ingresados es: " + str(promedio_lista)) # Se imprime el promedio de la lista
```

## Punto 2

``` python
def productoPunto(listaA:list,listaB:list)->int: #Se declara la función 
    x = 0
    for i in range(len(listaA)): # i va a tomar los valores del 0 a la longitud de la lista
        x += listaA[i]*listaB[i] #Se multiplica los mismos indices de ambas listas y se guardan en X
    return x #Devuelve X

if __name__=="__main__":
    num = int(input("Ingrese la cantidad de números que quiere ingresar a las listas: ")) #Cantidad de números en las listas
    #Listas vacias
    listaA = [] 
    listaB = []
    #Se pregunta según en indice que número quiere que este en la lista
    for i in range(num):
        f = int(input("Ingrese el indice "+str(i)+" de la primera lista: ")) 
        listaA.append(f)
    for n in range(num):
        x = int(input("Ingrese el indice "+str(n)+" de la segunda lista: "))
        listaB.append(x)
print("El producto punto de las listas es:", productoPunto(listaA, listaB))#Se llama la función y se le ponen las listas
```

## Punto 3

``` python
lista1 = [] #Se define una lista vacía
num = int(input("ingrese la cantidad de elementos que tendrá su lista: ")) # preguntamos la longitud de la lista
for i in range(num): # Se itera el proceso la cantidad de veces dicha por el usuario
    real = int(input("ingrese los números reales para su lista: ")) #Solicitamos al usuario los elementos de la liista
    lista1.append(real) # Añadimos los elementos a la lista vacia
print(lista1) #imprimimos la lista

ceros = lista1.count(0) # definimos'ceros' como el conteo de '0' presentes en la lista
for j in range(ceros): # Hacemos el siguiente proceso para cada '0' de la lista
    lista1.remove(0) # eliminamos los '0' de la lista

for m in range(ceros): # Hacemos el siguiente proceso para cada '0' que estaba en la lista
    lista1.append(0) #Añadimos los '0' que habian al final de la lista

print('su lista con todos los ceros al final se ve asi: ',lista1) #Imprimimos la lista
```

Y listo, eso sería todo por este reto. Muchas gracias
