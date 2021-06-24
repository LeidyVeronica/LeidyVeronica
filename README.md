- 👋 Hi, I’m @LeidyVeronica
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...

<!---
LeidyVeronica/LeidyVeronica is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
import sys
import os

usuario1 = 51672
contraseña1 = 27615


op1 = "Cambiar Contraseña"
op2 = "Ingresar coordenadas actuales" 
op3=  "Ubicar zona wifi más cercana"
op4 = "Guardar archivo con ubicación cercana"
op5 = "Actualizar regristros de zona desde el archivo "
op6 = "Elegir opción de menú favorita"
op7 = "Cerrar sesión"
aux = ""
adivinanza1 = "Antes era un trángulo invertido, me separaron de mi hermano siamés y quedé siendo un: " 
adivinanza2 = "Tengo forma de patito arqueado y redondito: "
opciónMenu = 0
opciónFavorita = 0
con = 0

print("Bienvenido al sistema de ubicacion para zonas publicas WIFI") #Datos de salida
usuario = int(input("Ingresa tu usuario:\t "))

if(usuario == usuario1):        #verificacion del usuario y contraseña

    print("Usuario correcto")
    contraseña = int(input("Ingrese la contraseña:\t "))

    if contraseña == contraseña1:
            print("Los datos ingresados son correctos")
            captcha = 672 + ((7 * 2 - 5 * 2) + (6 / 2))
            captcha1 = int(input("672 + 7=\t\t"))
            if captcha == captcha1:
                print("Sesión iniciada")
                print(f"\n1. {op1}", f"2. {op2}", f"3. {op3}", f"4. {op4}", f"5. {op5}", f"6. {op6}", f"7. {op7}", sep ="\n")
                while True:
                    try:
                        opciónMenu = int(input("\nElige una opción: "))
                    except:
                        opciónMenu = 0
                    if opciónMenu not in range(1,8):
                        con = con + 1
                        print(f"\nError")
                        if con > 3:
                            quit()
                    elif opciónMenu == 1:
                        print(f"\nUsted ha elegido la opción {opciónMenu}")
                        break
                    elif opciónMenu == 2:
                        print(f"\nUsted ha elegido la opción {opciónMenu}")
                        break
                    elif opciónMenu == 3:
                        print(f"\nUsted ha elegido la opción {opciónMenu}")
                        break
                    elif opciónMenu == 4:
                        print(f"\nUsted ha elegido la opción {opciónMenu}")
                        break
                    elif opciónMenu == 5:
                        print(f"\nUsted ha elegido la opción {opciónMenu}")
                        break
                    elif opciónMenu == 6:
                        try:
                            opciónFavorita = int(input("Seleccione opción favorita: "))
                        except:
                            sys.exit("Error")
                        if opciónFavorita not in range(1,6):
                            print("Error")
                            break
                        else:
                            try:
                                aux = int(input(f"Para comfirmar por favor responda:{adivinanza1}"))
                            except:
                                None
                            if 7 == aux:
                                try:
                                 aux = int(input(f"Para comfirmar por favor responda:{adivinanza2}"))
                                except:
                                    None
                                if 2 == aux:
                                    os.system("cls")
                                    if opciónFavorita == 1:
                                        print(f"\n1. {op1}", f"2. {op2}", f"3. {op3}", f"4. {op4}", f"5. {op5}", f"6. {op6}", f"7. {op7}", sep ="\n")
                                    elif opciónFavorita == 2:
                                        print(f"\n1. {op2}", f"2. {op1}", f"3. {op3}", f"4. {op4}", f"5. {op5}", f"6. {op6}", f"7. {op7}", sep ="\n")  
                                    elif opciónFavorita == 3:
                                        print(f"\n1. {op3}", f"2. {op1}", f"3. {op3}", f"4. {op4}", f"5. {op5}", f"6. {op6}", f"7. {op7}", sepa ="\n") 
                                    elif opciónFavorita == 4:
                                        print(f"\n1. {op4}", f"2. {op1}", f"3. {op3}", f"4. {op4}", f"5. {op5}", f"6. {op6}", f"7. {op7}", sep ="\n") 
                                    elif opciónFavorita == 5:
                                        print(f"\n1. {op5}", f"2. {op1}", f"3. {op3}", f"4. {op4}", f"5. {op5}", f"6. {op6}", f"7. {op7}", sep ="\n") 
                                else:
                                    sys.exit("Error")
                            else:
                                sys.exit("Error")
                    elif opciónMenu == 7:
                        print("Hasta pronto")
                        break
            else:
                print("Error")

    else:
        print("Error")
else:
    print("Error")
