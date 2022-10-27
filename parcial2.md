**EJERCICIO 1**

DFD Que cuente del 1 al 10 y sume los valores

[![1-ER-PROBLEMA-FOR.jpg](https://i.postimg.cc/VN1fR72k/1-ER-PROBLEMA-FOR.jpg)](https://postimg.cc/21cNjxzs)

[![1-ER-PRBLEMA-WHILE.jpg](https://i.postimg.cc/FKZ9nyQg/1-ER-PRBLEMA-WHILE.jpg)](https://postimg.cc/B8j9j1bX)

[![1-ER-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/RFpvvvhW/1-ER-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/R6tkR5cm)

**Prueba de escritorio**

|Corridas|S|C/i|Resultado(s+c/i)|
|-|-|-|-|
|1|0|1|1|
|2|1|2|3|
|3|3|3|6|
|4|6|4|10|

**Entradas= 0**

**Salidas= 1**

**Ciclo for**

```dart
void main(List<String> args) {
  int s = 0;
  for (var i = 1; i <= 10; i++) {
    s += i;
  }
  print("La suma de los valores es: $s");
}
```
**_Ciclo while:_**
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  while (c <= 10) {
    s += c;
    c++;
  }
  print("El resultado de la suma de los valores es:$s");
```
**_Ciclo do-while:_**
```dart
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s += c;
    c++;
  } while (c <= 10);
  print("El resultado de la suma de los valores es:$s");
```



**EJERCICIO 2**

Realiza un DFD que obtenga la suma de los primeros 5 numeros pares

[![2-DO-PROBLEMA-WHILE.jpg](https://i.postimg.cc/4nRJKBgt/2-DO-PROBLEMA-WHILE.jpg)](https://postimg.cc/V04yp95L)

[![2-DO-PROBLEMA-FOR.jpg](https://i.postimg.cc/Vk1CpFCd/2-DO-PROBLEMA-FOR.jpg)](https://postimg.cc/hfyv7TMB)

[![2-DO-PROBLEMA-DO-WHILE.jpg](https://i.postimg.cc/7LtJC8Q2/2-DO-PROBLEMA-DO-WHILE.jpg)](https://postimg.cc/VSMkTTwf)

**Prueba de Escritorio**

|Corridas|C|S+C*2|S|
|-|-|-|-|
|1|1|0+2|2|
|2|2|2+2|4|
|3|3|4+6|10|
|4|4|10+8|18|
|5|5|18+10|28|

**Entradas=0**

**Salidas=1**

**Ciclo for**

```dart
void main(List<String> args) {
  int s = 0;
  for (var i = 2; i <= 10; i = i + 2) {
    s = s + i;
  }
  print("resultado de la suma de numeros pares es:$s");
}
```
**Ciclo while**

```dart
void main(List<String> args) {
  int s = 0, c = 1;

  do {
    s = s + c * 2;
    c = c + 1;
  } while (c <= 5);
  print("la suma de numeros pares es:$s");
}
```
**Ciclo Do-while**

```dart
void main(List<String> args) {
  int s = 0, c = 1;
  while (c <= 5) {
    s = s + c * 2;
    c = c + 1;
  }
  print("resultado de la suma de numeros pares:$s");
}
```


**EJERCICIO 3**

Escribe un DFD que almacene el numero N leido del teclado en un array de 10 espacios

[![3-ER-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/9MTZGJkb/3-ER-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/ZBbWmF4v)

[![3-ER-PROBLEMA-FOR.jpg](https://i.postimg.cc/vHGfV7t7/3-ER-PROBLEMA-FOR.jpg)](https://postimg.cc/rzYD6rbz)

[![3-ER-PROBLEMA-WHILE.jpg](https://i.postimg.cc/d18Z7D7S/3-ER-PROBLEMA-WHILE.jpg)](https://postimg.cc/S2xx3SfW)

|Corrida|Contador/posicion en el array|Numero ingresado|
|-|-|-|
|1|0|5|
|2|1|5|
|3|2|5|
|4|3|5|

Ejemplo del array

|5|
|-|
|5|
|5|
|5|

**Entradas= 1**

**Salidas=1**

**Ciclo for**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
```
**Ciclo While**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
**Ciclo Do-While**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```


**Ejercicio 4**

Escribe un dfd que almacene los N numeros leidos del teclado en el vector de 10

[![4-TP-PROBLEMA-WHILE.jpg](https://i.postimg.cc/RhN4nDhp/4-TP-PROBLEMA-WHILE.jpg)](https://postimg.cc/BP9drNx2)

[![4-TP-PROBLEMA-FOR.jpg](https://i.postimg.cc/8PfTp9qj/4-TP-PROBLEMA-FOR.jpg)](https://postimg.cc/hfnkMy4B)

[![4-TP-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/d1SKvj62/4-TP-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/2bvt7vPy)

**Prueba de escritorio**

|Corrida|Contador|Numeros usados|Numero ingresado|
|-|-|-|-|
|1|0|1|5|
|2|1|2|7|
|3|2|3|8|

Ejemplo del array 

|5|
|-|
|7|
|8|

**_Ciclo for:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  for (var i = 0; i <= 9; i++) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
    }
  }
  stdout.write("aqui esta la lista, $arra");
}
```
**_Ciclo while:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  while (i <= 9) {
    String? s = stdin.readLineSync();
    if (s != null) {
      int ner = int.parse(s);
      arra[i] = ner;
    }
    i++;
  }
  stdout.write("Tu lista es, $arra ");
}
```
**_Ciclo do-while:_**
```dart
void main() {
  var arra = new List.filled(10, 0);
  stdout.write("Dame diez numeros\n ");
  stdout.write("----------\n");
  int i = 0;
  do {
    String? s = stdin.readLineSync();
    if (s != null) {
      int n = int.parse(s);
      arra[i] = n;
      i++;
    }
  } while (i <= 9);
  stdout.write("Tu lista es $arra ");
}
```

#### 1.4 Entradas
10 números leídos del teclado.
#### Salidas
A[10], lleno con elementos



**EJERCICIO 5**


Escribe un dfd que almacene un contador negativo del 10 al 0 en un vector

[![5-TO-PROBLEMA-WHILE.jpg](https://i.postimg.cc/bNPZsQjx/5-TO-PROBLEMA-WHILE.jpg)](https://postimg.cc/s1njLGxx)

[![5-TO-PROBLEMA-FOR.jpg](https://i.postimg.cc/26v555c9/5-TO-PROBLEMA-FOR.jpg)](https://postimg.cc/VrfwGzcX)

[![5-TO-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/kGmgRdLJ/5-TO-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/62MXFF9g)

**Prueba de escritorio**

|Corrida|Contador|Posicion del vector|Numero asignado al vector|
|-|-|-|-|
|1|10|0|10|
|2|10|1|9|
|3|9|2|8|

**Ejemplo del array**

|10|
|-|
|9|
|8|
|7|
|6|

**Ciclo For**
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  for (var i = 10; i >= 0; i--) {
    arr[10 - i] = i;
  }
  print(arr);
}
```
**Ciclo while**

```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  while (c >= 0) {
    arr[10 - c] = c;
    c = c - 1;
  }
  print(arr);
}
```

**Ciclo Do-While**
```dart
void main() {
  var arr = <int>[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10];
  int c = 10;
  do {
    arr[10 - c] = c;
    c = c - 1;
  } while (c >= 0);
  print(arr);
}
```


**EJERCICIO 6**


Realiza un dfd que almacene en un vector todos los numeros pares leidos hasta completar los espacios

[![6-TO-PROBLEMA-WHILE.jpg](https://i.postimg.cc/pddH7dM5/6-TO-PROBLEMA-WHILE.jpg)](https://postimg.cc/MngNfqTz)

[![6-TO-PROBLEMA-FOR.jpg](https://i.postimg.cc/1tk1fcnD/6-TO-PROBLEMA-FOR.jpg)](https://postimg.cc/9RYnk9Bf)

[![6-TO-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/br1cbDkW/6-TO-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/0K5B1Nt0)

**Prueba de esritorio**

|Corrida|Numero ingresado|%2?|%2-->(c)=N y C=c+1|
|-|-|-|-|
|1|6|si|(0)-->6 and c=1|
|2|4|si|(1)-->4 and C=2|
|3|3|no||

**Ejemplo del array hasta ahora**

|6|
|-|
|4|

**Ciclo for**
```python
listanumeros = []
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
numerousuario = int(input("introdusca otro numero: "))
listanumeros.append(numerousuario)

print(f"los numeros son {listanumeros}")

def pares(listanumeros):
    listanumeros = []


for n in listanumeros:
    if n % 2 == 0:
        print("Estos numeros son pares"+ "  " + str(n))
```
**Ciclo while**

```python
listanumeros = []
numerousuario = int(input("introdusca un numero: "))
listanumeros.append(numerousuario)
decision = input("¿desea añadadir mas numeros?: ")

while decision == "s" or decision == "s":
    numerousuario = int(input("introdusca otro numero: "))
    listanumeros.append(numerousuario)
    decision = input("¿desea añadir otro numero?: ")


print(f"los numeros son {listanumeros}")
for n in listanumeros:
    if n % 2 == 0:
        print("Este numero de la lista es par" + str(n))
        


input("por favor, precione una tecla para salir.")
```
**Ciclo Do-While**

```dart
print("PARES")
numero_1 = int(input("Escriba un número entero: "))
numero_2 = int(input(f"Escriba un número entero mayor o igual que {numero_1}: "))

if numero_2 < numero_1:
        print(f"¡Le he pedido un número entero mayor o igual que {numero_1}!")
else:
        for i in range(numero_1, numero_2 + 1):
            if i % 2 == 0:
                print(f"El número {i} es par.")
```



**EJERCICIO 7**


Realiza un dfd que obtenga el promedio de las calificacion aprobadas y la cantidad de alumnos reprobados, la calificacion entre 0 y 10 y el maximo de alumnos es de 15

[![7-MO-PROBLEMA-WHILE.jpg](https://i.postimg.cc/YCFvDbkm/7-MO-PROBLEMA-WHILE.jpg)](https://postimg.cc/mPbZt3Pb)

[![7-MO-PROBLEMA-FOR.jpg](https://i.postimg.cc/661T9Dpv/7-MO-PROBLEMA-FOR.jpg)](https://postimg.cc/0rD9nXmk)

[![7-MO-PROBLEMA-DOWHILE.jpg](https://i.postimg.cc/WpKbRg5m/7-MO-PROBLEMA-DOWHILE.jpg)](https://postimg.cc/yWmzcg4W)

**Prueba de escritorio**

|corrida|contador|numero de vector|N|N>6-->C+1 and print en vector|
|-|-|-|-|-|
|1|1|0|5||
|2|1|0|8|C=C+1 and (0)=N|
|3|2|1|9|C=c+1 and (1)=N|

Ejemplo del array hast ahora

|9|
|-|
|8|

**Ciclo en for**

```dart
alumnos = list(range(15))
p_aprobados = 0
j = 0

for i in alumnos: 
    while(True):
        calificacion = int(input("Ingresa la calificación >>"))
        if (calificacion >= 0 and calificacion <= 10):
            break
        else:
            print("Calificación fuera de rango. Intenta de nuevo")
 
    if (calificacion < 6):
     alumnos[i] = "R"
    else:
     p_aprobados = calificacion + p_aprobados
     j = j + 1
     alumnos[i] = "A"

print("\033[33;1m",alumnos,"\033[39m")
print("El promedio de calificación de los aprobados es de >>",round(p_aprobados/j,2))
print("El total de aprobados fueron >> ",j)
print("El total de reprobados fueron >> ",(len(alumnos)-j))
```

**_Ciclo while:_**
```python
alumnos = list(range(15))
p_aprobados = 0
j = 0

for i in alumnos: 
    while(True):
        calificacion = int(input("Ingresa la calificación >>"))
        if (calificacion >= 0 and calificacion <= 10):
            break
        else:
            print("Calificación fuera de rango. Intenta de nuevo")
 
    if (calificacion < 6):
     alumnos[i] = "R"
    else:
     p_aprobados = calificacion + p_aprobados
     j = j + 1
     alumnos[i] = "A"

print("\033[33;1m",alumnos,"\033[39m")
print("El promedio de calificación de los aprobados es de >>",round(p_aprobados/j,2))
print("El total de aprobados fueron >> ",j)
print("El total de reprobados fueron >> ",(len(alumnos)-j))
```
**_Ciclo do-while:_**
```dart
void main() {
  double PromA = 0;
  var contr = 0;
  double sumaA = 0;
  double contA = 0;
  double cal1 = 0;
  double cal2 = 1;
  var cont = 0;
  stdout.write("Dame las calificaciones\n ");
  stdout.write("----------\n");
  do {
    double c = double.parse(stdin.readLineSync()!);
    cont = cont +1;
    if (c > 10) {
      print('La calificacion no puede ser mayor a 10');
      cont = cont - 1;
    }
    if (c < 0) {
      print('La calificacion no puede ser menor a 0');
      cont = cont - 1;
    }
    if (c < 6 && c > 0) {
      contr = contr + 1;
    }
    if (c <= 10 && c >= 6) {
      cal1 = c;
      sumaA = sumaA + cal1;
      contA++;
    }
    if (cal1 > cal2) {
      cal2 = cal1;
    }
  } while (cont <= 14);
  PromA = sumaA / contA;
  print('El promedio de aprobados es $PromA');
  print('La calificacion mas alta es $cal2');
  print('La cantidad de reprobados son $contr');
}
```

#### 1.4 Entradas
Calificacines
#### Salidas
Calificaciones, promedio de las calificaciones aprobatorias y cantidad de alumnos reprobados.


**EJERCICIO 8**


Crea un dfd que capture N numeros en el rango [li,ls] donde LI=limite inferior y LS=Limite superior para li<ls y ls>0, obtener:
  
  Cantidad de numeros pares y su promedio
  
  Cantidad de numeros impares y su promedio
  
  ¿Que promedio es mayor?
 

[![8while.jpg](https://i.postimg.cc/ZKtQGqzs/8while.jpg)](https://postimg.cc/Z0Hj34R6)

[![8for.jpg](https://i.postimg.cc/3x9b0C4z/8for.jpg)](https://postimg.cc/sMQJtWJJ)

[![8dowhile.jpg](https://i.postimg.cc/qqfmH1S6/8dowhile.jpg)](https://postimg.cc/LYTkz3Hm)
  
  **Prueba de escritorio**
  
|Corrida|N|N%2?|si-->Sp=Sp+N and Cp=Cp+1|No--->Si=Si+N and Ci=Ci+1|
|-|-|-|-|-|
|1|5|no|...|Si:5 and Ci:1|
  |2|6|si|sp:6 and cp:1|
  |3|7|no|...|si:12 and ci:2|
  |4|2|si|si:7 and CP:2|
  
  **Ciclo for**
  
  ```python
  sp=0
cp=0
pp=0
si=0
ci=0
pi=0
li=-1
ls=-1
n=-1
num=-1

while(li<0):
    li = int(input("Limite inferior: "))
    
    if(li<0):
        print("Tiene que ser mayor a 0")
        
while(ls<li):
    ls = int(input("Limite superior: "))
    
    if(ls<li):
        print("Tiene que ser mayor que el limite inferior")
        
while(n<0):
    n = int(input("¿Cuantos numeros? "))
    
    if(n<0):
        print("Tiene que ser mayor a 0")
    
for i in range(n): 
    while(num<=li or num>=ls):
        num = int(input("Dame un numero de LI y LS: "))
        
        if(num<=li or num>=ls):
            print("Tiene que estar dentro del LI al LS")

    if(num%2==0):
        sp=sp+num
        cp=cp+1
    else:
        si=si+num
        ci=ci+1
        
    num=-1       
         
if(sp==0 or cp==0):
    pp=0
else:
    pp=sp/cp
    
if(si==0 or ci==0):
    pi=0
else:
    pi=si/ci
    
if(pp>pi):
    print("El PP es mayor que el PI")
else:
    print("El PI es mayor que el PP")
  ```
  **Ciclo while**
  
  ```python
  print("Dame Límite inferior: ")
Li = int(input())
while Li<0:
    print("El límite inferior debe ser mayor a 0")
    print("Dame Límite inferior: ")
    Li = int(input())

print("Dame límite superior: ")
Ls = int(input())
while Ls<=Li:
    print("El límite superior no puede ser menor o igual al limite inferior")
    print("Dame límite superior: ")
    Ls = int(input())
  ```
  **Ciclo Do-while**
  
  ```dart
  pares = 0
impares = 0

lista=[]
for x in range(10):
    valor=int(input("Ingrese un valor entero: "))
    lista.append(valor)
print(lista)

for a in lista:
    if a % 2 == 0:
        pares = pares + a
    else:
        impares = impares + a
print("La suma de los números pares es: ",pares)
print("La suma de los números impares es: ",impares)

prom_pares = pares / a
prom_impares = impares / a

print("El promedio de los números pares es: ",prom_pares)
print("El promedio de los números impares es: ",prom_impares)

if prom_pares > prom_impares:
    print("El promedio de los pares es mayor que el promedio de los impares.")
else:
    print("El promedio de los números impares es mayor que el promedio de los pares.")
  ```
  
  
  **EJERCICIO 9**
  
  

Escribe un dfd que obtenga la frecuencia de N calificaciones entre 1 y 10 indique la cantidad de reprobados y la cantidad de aprobados, el promedio de aprodabos y reprobados

[![9while.jpg](https://i.postimg.cc/zfxM4mnd/9while.jpg)](https://postimg.cc/TyWCW4Nm)

[![9for.jpg](https://i.postimg.cc/Qt5Q11xp/9for.jpg)](https://postimg.cc/JDrHWyXn)

[![9dowuile.jpg](https://i.postimg.cc/hvDXvdJ4/9dowuile.jpg)](https://postimg.cc/N9nsPL7Z)

**Prueba de Escritorio**
  
  |CAL[1,10]|N  |N>0 |i  |i<=N|CAL[1,10]|C  |C>0, C<=10|CAL[C]++|i++|CAL|
|---------|---|----|---|----|---------|---|----------|--------|---|---|
|9        |4  |4>0 |0  |0<=4| 0        |9  |9>0, 9<=0 |10      |1  |9  |
|9        |   |    |1  |1<=4|1         |9  |9>0, 9<=0 |10      |2  |9  |
|8        |4  |4>0 |0  |2<=4| 2        |8  |8>0, 8<=0 |9       |3  |8  |
|7        |   |    |1  |3<=4|  3       |7  |7>0, 7<=0 |8       |4  |7  |




|CR |CA |PR |PA |PG |SR |SA |N  |i  |i<=n|NUM|NUM>0,NUM<=10|NUM>=6|CA+1|SA+NUM|CR+1|SR+NUM|i++|PA=SA/CA|PR=SR/CR|PG=(PR+PA)/2|PG |
|---|---|---|---|---|---|---|---|---|----|---|-------------|------|----|------|----|------|---|--------|--------|------------|---|
|0  |0  |0  |0  |0  |0  |0  |4  |0  |0< 4|8  |8>=0,8<=10   |8>=6  |1   |8     |0   |0     |1  |
|0  |1  |0  |0  |0  |0  |8  |4  |1  |1< 4|5  |5>=0,5<=10   |5>=6  |1   |8     |1   |5     |2  |
|1  |1  |0  |0  |0  |5  |8  |4  |2  |2< 4|9  |9>=0,9<=10   |9>=6  |2   |17    |1   |5     |3  |
|1  |2  |0  |0  |0  |5  |7  |4  |3  |3< 4|3  |3>=0,3<=10   |3>=6  |2   |17    |2   |8     |4  |17/2    |8/4     |(8.5+4)/2   |6.25|


#### 1.4 Entradas.
N

C

NUM

#### 1.5 Salidas.


**Ciclo for**
  
  
```dart
void main() {
  double CR = 0;
  double CA = 0;
  double PA = 0;
  double PG = 0;
  double SR = 0;
  double SA = 0;
  double PR = 0;

  //Ingresar el numero de calificaciones
  int Calif = int.parse(stdin.readLineSync()!);

  if (Calif > 0) {
    for (var i = 0; i >= Calif; i++) {
      //Calificacion [1,10]
      int n = int.parse(stdin.readLineSync()!);

      if (n > 0 && n <= 10) {
        var Cal;
        Cal[n]++;

        if (n >= 6) {
          CA = CA + 1;
          SA = SA + n;
        } else {
          CR = CR + 1;
          SR = SR + n;
        }
        print("La cantidad de alumnos reprobados CR");
        print("Cantidad de alumnos aprobados CA");

        PA = SA % CA;
        PR = SR % CR;
        PG = (PA + PR) % 2;
      } else {
        print("La calificacion tiene que estar en entre 0 y 10");
      }
    }
  } else {
    print("Las calificaciones no pueden ser 0");
  }
}
```
**Ciclo while**
```dart
void main() {
  double CR = 0;
  double CA = 0;
  double PA = 0;
  double PG = 0;
  double SR = 0;
  double SA = 0;
  double PR = 0;

  //Ingresar el numero de calificaciones
  int n = int.parse(stdin.readLineSync()!);
  var Cont;
  while (n > 0 && Cont <= 2) {
    if (n >= 6) {
      CA = CA + 1;
      SA = SA + n;
      Cont = Cont + 1;
    } else {
      CR = CR + 1;
      SR = SR + n;
      Cont = Cont + 1;
    }
    PA = SA / CA;
    PR = SR / CR;
    PG = (PA + PR) / 2;

    print("La cantidad de alumnos aprobados es $CA");
    print("La cantidad de alumnos reprobados es $CR");
    print("El promedio de aprobados es $PA");
    print("El promedio general es $PG");
  }
}
```
**Ciclo Do-While**
```python
  Calificaciones=int(input("Ingrese la cantidad de calificaciones"))
vec=[]
n=0
cont = 0
while(True):
    calificacion=int(input("Calificacion: "))
    n=n+calificacion
    vec.append(calificacion)
    cont += 1
    if(cont>=Calificaciones):
        break;
        
aprobado=0
promedioAprobados = 0
for h in vec:
    if h>=5:
        aprobado=aprobado+1
        promedioAprobados = promedioAprobados + h
promedioAprobados = promedioAprobados / aprobado
reprobado=0
for k in vec:
    if k<=5:
        reprobado=reprobado+1
print("Cantidad de aprobados:", aprobado)
print("Cantidad de reprobados:", reprobado)
print("Promedio de aprobados:", promedioAprobados)

```
