# za_ispit

## zadatak 4

def povrsina_trokuta(T_1, T_2, T_3):
    asd = 0
    P = 0.5 * abs(int(T_1[0]) * (int(T_2[1]) - int(T_3[1])) + int(T_2[0]) * (int(T_3[1]) - int(T_1[1])) + int(T_3[0])  * (int(T_1[1]) - int(T_2[1])))
    return P

def tocke():
    T = []
    T.append(input("Unesite koordinatu X: "))
    T.append(input("Unesite koordinatu Y: "))
    return T
    

T1 = tocke()
T2 = tocke()
T3 = tocke()

povrsina = povrsina_trokuta(T1, T2, T3)
if povrsina == 0:
    print("Zadane točke ne tvore trokut jer je površina trokuta 0")
else:
    print("Površina trokuta je: " + str(povrsina))
    
    
    
