# Maria Fernanda Alvarez Rios #

# Tarea 2 - Ejercicios Unidad 1 #

# Reto 1 simula el comportamiento de la tortuga usando solo print() e input() #
         pasos = 50
         print("Creando tortuga simulada que da...", pasos, "pasos")
         print("-" * pasos + ">")
  

# Reto 2 Tortuga bajando
        
  
# Reto 3 Girar y dibujar usando solo print() e input()
         pasos_bajada = 15
         pasos_adelante = 10

         print("-" * pasos_adelante + ">")

         for i in range(pasos_bajada):
         print(" " * pasos_adelante + "|")   

         print(" " * pasos_adelante + "V")


        pasos_totales = pasos_adelante + pasos_bajada

        print("La tortuga avanzo", pasos_adelante,"pasos.")
        print("La tortuga bajo", pasos_bajada, "pasos.")
        print("La tortuga recorrió un total de", pasos_totales, "pasos.")
     
# Reto 4 Encapsula los comportamientos anteriores usando funciones

        pasos_adelante = int(input("¿Cuántos pasos avanza la tortuga? "))
        pasos_abajo = int(input("¿Cuántos pasos baja la tortuga? "))
 
        def adelante(pasos):
        global pasos_adelante
        pasos_adelante = pasos
        print("-" * pasos + ">")


        def abajo(pasos):
        for i in range(pasos):
        print(" " * pasos_adelante + "|")

       print(" " * pasos_adelante + "V")

       adelante(pasos_adelante)
       abajo(pasos_abajo)

# Reto 5 La tortuga baja las escalones

        def  Escalón 1
        adelante(5)
        abajo(2)

       def  Escalón 2
       adelante(5)
       abajo(2)

      def Escalón 3
      adelante(5)
      abajo(2)
