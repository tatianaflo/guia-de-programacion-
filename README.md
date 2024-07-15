# guia-de-programacion-
#ejercicio #3
print ("hola mundo")

#ejercicio #4
mensaje= "!hola mundo!"
print(mensaje)

#ejercicio #5
nombre = input ("¿cual es tu nombre?")
print (f"!hola{nombre}!")

#ejercicio #6
resultado = (3 + 2 / 2 * 5) ** 2
print (resultado)

#ejercicio #7
horas_trabajadas=float(input("¿cuantas horas has trabajado?"))
costo_por_hora=float(input("¿cual es tu costo por hora?"))

paga = horas_trabajadas * costo_por_hora

print ("tu paga es : " + str (paga))


#ejercicio #8 

n= int(input("ingrese un entero positivo: "))
suma = n * (n+1) / 2
print("la suma de los enteros deasde 1 hasta" +str(n)+ "es"+str(suma))


#ejercicio #9
peso = float(input("ingresa tu peso en kg: "))
estatura = float(input("ingresa tu estatura en metros: "))

imc=round(peso/(estatura ** 2), 2)

print("tu indice en masa corporal es:" + repr(imc))

#ejercicio # 10 

num_engranes = int(input("ingrese el numero de engranes vendidos"))
num_cilindros = int(input("ingresa el numero de cilindros vendidos"))

peso_engranes= num_engranes *112
peso_cilindros = num_cilindros * 75 
peso_total = peso_engranes + peso_cilindros

print ( "el peso total del paquete es: " + str(peso_total)+"gramos")

#ejercicio #11
precio_normal= 3.49

num_barras_no_frescas = int(input("ingresa el numero de barras vendidas que no son del dia: "))

descuento = 0.6  # 60% de descuento

precio_final = precio_normal * (1 - descuento)
total_no_frescas = num_barras_no_frescas * precio_final

print ("precio normal de una barra de pan: $" + str(precio_normal) )
print("descuento por no ser fresca; " + str(int(descuento * 100)) + "%")
print("precio final de las barras no frescas: $" + str(round(precio_final,2)))
print("coste final total: $" + str(round(total_no_frescas, 2)))

#ejercicio #12
edad = int ( input("ingresa tu edad: "))

if edad >= 18 : 
    print ("eres mayor de edad.")
else:
    print("eres menor de edad.")

#ejercicio #13
contraseña_almacenada = "contraseña"
contraseña_ingresada = input ("ingresa la contraseña: ")

if contraseña_ingresada.lower()== contraseña_almacenada.lower():
    print("la contraseña coincide.")
else:
    print("la contraseña no coincide.")

#ejercicio #14

try:
    dividiendo = float(input("ingresa el dividendo:"))
    divisor = float(input("ingresa el divisor:"))

    resultado = dividiendo / divisor

    print("el resultado de la division es: ",resultado)
except ZeroDivisionError:
    print("Error:no se puede dividir entre cero ")


    #ejercicio #15
numero = int(input("Ingresa un número entero: "))

if numero %2 == 0:
    print("el numero" , numero, "es par.")
else: 
    print("el numero," , numero,"es impar.")


    #ejercicio #16
palabra = input("ingresa una palabra: ")

for i in range (10):
    print( palabra)


    #ejercicio # 17
numero =int ( input("ingresa un nunero entero positivo:"))

numeros_impares = []

for i in range ( 1,numero+1,2):
    numeros_impares.append(i)

resultado = " , ".join(str(x) for x in numeros_impares)

print ( resultado)
