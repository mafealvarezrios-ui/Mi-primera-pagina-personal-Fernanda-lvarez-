# Maria Fernanda Alvarez Rios #

# Tarea 2 - Ejercicios Unidad 1 #

# Reto 1 simula el comportamiento de la tortuga usando solo print() e input() #
        
         pasos = 50
         print("Creando tortuga simulada que da...", pasos, "pasos")
         print("-" * pasos + ">")
  

# Reto 2 Tortuga bajando
            r = []
         print("tortuga bajando")
         while True:
        input()
        r.append("|")
       print("\n" * 30)
       print("tortuga bajando")
       for x in r[:-1]: print(" ", x)
       print("  🐢")

  
# Reto 3 Girar y dibujar usando solo print() e input()
         adelante: 15
         abajo:20
        pasos_adelante = int(input("¿Cuántos pasos avanza la tortuga? "))
        pasos_abajo = int(input("¿Cuántos pasos baja después de girar? "))
        
        print("-" * pasos_adelante + ">")
        for i in range(pasos_abajo):
        print(" " * pasos_adelante + "|")
        print(" " * pasos_adelante + "V")

        print("La tortuga avanzó", pasos_adelante, "pasos.")
        print("Luego bajó", pasos_abajo, "pasos.")

        
# Reto 4 Encapsula los comportamientos anteriores usando funciones

         pasos_adelante = int(input("¿Cuántos pasos avanza la tortuga? "))
         pasos_abajo = int(input("¿Cuántos pasos baja la tortuga? "))
       
        def adelante(n):
           print("→" * n)
 
      def abajo(n):
        for _ in range(n):
           print("↓")

      
# Reto 5 La tortuga baja las escalones

    pasos_adelante = 15   # pasos hacia la derecha
    pasos_abajo = 20      # pasos hacia abajo


    posicion_x = 0  


     def adelante(pasos):
       global posicion_x
       # Tramo horizontal
       print(" " * posicion_x + "-" * pasos + ">")
       posicion_x += pasos   # Se acumula la posición


    def abajo(pasos):
       global posicion_x
       # Tramo vertical
       for i in range(pasos):
        print(" " * posicion_x + "|")
      # Pie del tramo
      print(" " * posicion_x + "V")


    adelante(pasos_adelante)
    abajo(pasos_abajo)

    adelante(pasos_adelante)
    abajo(pasos_abajo)

    adelante(pasos_adelante)
    abajo(pasos_abajo)


        
