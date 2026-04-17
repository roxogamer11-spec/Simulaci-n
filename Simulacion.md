import random

n = 10000
Uno = 0
Dos = 0
Tres = 0
Cuatro = 0
Cinco = 0
Seis = 0

for i in range(n):
    Dado = random.randint(1,6)
    
    if Dado == 1:
        Uno += 1
    elif Dado == 2:
        Dos += 1
    elif Dado == 3:
        Tres += 1
    elif Dado == 4:
        Cuatro += 1
    elif Dado == 5:
        Cinco += 1
    else:
        Seis += 1

print("\n==============Resultados==============") 
print(f"Total de lanzamientos: {n}") 

# Probabilidades

print("\nCara [] Frecuencia [] Probabilidad Empírica [] Probabilidad Teórica")

print("--------------------------------------------------------------")

print(f"1    [] {Uno}       [] {Uno/n:.4f}               [] 0.1667")

print(f"2    [] {Dos}       [] {Dos/n:.4f}               [] 0.1667")

print(f"3    [] {Tres}       [] {Tres/n:.4f}               [] 0.1667")

print(f"4    [] {Cuatro}       [] {Cuatro/n:.4f}               [] 0.1667")

print(f"5    [] {Cinco}       [] {Cinco/n:.4f}               [] 0.1667")

print(f"6    [] {Seis}       [] {Seis/n:.4f}               [] 0.1667")
