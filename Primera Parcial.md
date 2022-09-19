# Universidad de Colima
## Programación Funcional
## Profesor: Walter Alexander Mata Lopez
## **Luis Alexis Pizano Navarro**
## 18-09-2022
## 3°B
### Este es mi portafolio de evidencias de la primera parcial

### __1. Calificaciones de 5 alumnos de 5 materias__

    alumnos = ["Alexis","Andrea","Diana","Jason","Josue"]
    materia1 =[10,9,8,7,10]
    materia2 = [9,8,6,7,10]
    materia3 = [6,7,9,7,8]
    materia4 = [8,6,7,9,6]

    encabezado = ["nombre Alumno","Est. de datos","Ecu. diferenciales","Met Númericos","Prog Funcional"]

    def reporte(fmt):
        print(f"{encabezado[0]:^{fmt}} {encabezado[1]:^{fmt}} {encabezado[2]:^{fmt}} {encabezado[3]:^{fmt}}{encabezado[4]:^{fmt}}")
        for i in range (5):
        print(f"{alumnos[i]:^{fmt}} {materia1[i]:^{fmt}} {materia2[i]:^{fmt}} {materia3[i]:^{fmt}} {materia4[i]:^{fmt}}")

    reporte(20)


### __2. Tablas de multiplicar hasta donde el usuario lo indique__

    print("Programa de tablas de multiplicar")

    tabla_desde = 1
    tabla_hasta=int(input("Ingresa el limite de los datos: "))
    desde=1
    hasta=int(input("Valor de las tablas de multiplicar: "))

    for factor1 in range(tabla_desde, tabla_hasta + 1):
    print(f"Tabla de multiplicar del {factor1}:")
    for factor2 in range(desde, hasta +1):
        print(f"{factor1} x {factor2} = {factor1 * factor2}")
        print()


### __3. Programa que saluda__

    print("hola ICI")
    print("segunda clase")
    msj ="hola"
    print(msj)

### __4. Jupyter__

    #Interpolacion de cadenas
    name ="Alexis"
    edad= 18
    print("hola",name,"tienes",edad,"años")
    
    #fstrings
    mensaje = (f"hola {name}, tienes {edad} años")
    mensaje
    print(mensaje)
    print(f"hola {name}, tienes {edad} años")
    
    def saludo():
    print("hola mundo!!!")
    #fstrings
    mensaje= (f"hola {name}, tienes {edad} años")
    mensaje
    print(mensaje)
    print(f"hola {name}, tienes {edad} años")

    def saludo():
    print("hola mundo")
    mi_funcion=saludo()  
    saludo()
    print(mi_funcion)

    def saludo2():
    return "HOLA MUNDO!!"

#### Suma de dos variables
    a=5
    b=10
    res=f"la suma de {a}+{b}={a+b}"
    print(res)
    def suma(a,b):
    return a+b
    res=f"la suma de {a}+{b}={suma(a,b)}"
    print(res)
    
### __5. Listas__
    lista=["uno", "dos", "tres"]
    msg_numeros=f"numeros: {lista}"
    print(msg_numeros)

    tuplas_numeros=("uno", "dos", "tres")
    msg_numeros=f"numeros: {tuplas_numeros}"
    print(msg_numeros)

    set_numeros={"uno","dos","tres","tres"}
    print(set_numeros)

    dict_numeros={"1": "uno", "2": "dos", "3": "tres"}
    msg_dict_numeros = f"numeros: {dict_numeros}"
    print(msg_dict_numeros)
    dos=f"numero:{dict_numeros['2']}"
    print(dos)
    
#### Ejercicio
    #Escriba una funcion que mediante fstrings retorne el mensaje "Hola <nombre> tienes <edad> años".
    #Los argumentos de la funcion si: año actual, año de nacimiento y nombre
    a=18
    b=2003
    c="Luis Alexis"
    def todo(a,b,c):
    return(todo)
    todo=f"Hola, tu nombre es: {c}, naciste en {b}, tienes {a} años"
    print(todo)

### __6. Pycharm__
    Archivo main con sus imports
    import utilerias as util 
    import suma as s 
    import resta as r 
    import division as d 
    import multi as m 
    import cuadrado as c

    if name=="main": print("suma", s.suma(4,5)) print("resta", r.resta(5,3)) print("division", d.division(5,2)) print("multiplicacion", m.multi(5,10)) print("cuadrado", c.cuadrado(10))
#### Suma
    archivo suma
    def suma(a:int, b:int)->int:
    return a + b
    if name=="main": print(suma(4,5))
#### Resta
    archivo resta
    def resta(a:int, b:int)->int:
    return a-b
    if name=="main": print(resta(4,3))
#### Multiplicación
    archivo multiplicacion
    def multi(a:int, b:int )->int:
    return a*b
    if name=="main": print(multi(4,2))
#### División
    archivo division
    def division(a:int, b:int)->float:
    return a/b
    if name=="main": print(division(4,2))
#### Cuadrado
    archivo cuadrado
    def cuadrado(a:int)->int:
    return a*a
    if name=="main": print(cuadrado(5))
    if name=="main": print(suma(4,5)) print(cuadrado(5)) print(resta(4, 3)) print(division(4, 2)) print(multi(4, 2))
    
### __7. Ejercicio en clase __
    #%%
		def saludo_edad_(nombre:str,a_nacimiento:int):
				edad= 2022-a_nacimiento
				print("Hola",nombre,"tienes",edad,"años")
		def calcular_edad(a_actual:int,a_nacimiento:int)->int:
				return a_actual-a_nacimiento
		def saludo(nombre:str,edad:int):
				print ("Hola",nombre,"tienes",edad,"años")

		#%%
		def tabla(x):
				for i in range (11):
						print(x,"*",i,"=",x*i)

		if __name__=="__main__":
				print(tabla(3))
        
		#%%
		def tabla(t,n):
				for i in range (1,n+1):
						print(t,"*",i,"=",t*i)
		if __name__=="__main__":
				print(tabla(3,2))
### __8. Ordenar elementos en una lista__
     ld=[[5,4,6],[7,8,2,1],[3,4,5],[6,7]]
  	print(f"Desordenado: {ld}")
  	ld.sort()
  	print(f"Ordenado: {ld}")

  	ld=[5,4,6,7,8,2,1,3,4,5,6,7]
  	S1= sorted(ld)
  	print(S1)
  	ld=[5,4,6,7,8,2,1,3,4,5,6,7]
  	S2= sorted(ld,reverse=True)
  	print(S2)

  	ceros=[0,0,0,0,0,0,0,0,0]
  	print(ceros)
  	ceros=[0]*9
  	print(ceros)

  	valor_max=max(ld)
  	print(valor_max)

  	valor_min=min(ld)
  	print(valor_min)

  	cuatros=ld.count(4)
  	print(cuatros)

  	repe=[]
  	for i in range (1,9):
  			repe.append(ld.count(i))
  	print(repe)			
