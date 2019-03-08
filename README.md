# pigeon_hole
pigeon_hole

#Soru: Seçilecek sadece dört takım (m = 4 yuva) sınırlamasıyla, bir takım turnuvasında oynamak isteyen yedi kişiyi (n = 7 güvercin) hayal edin. Bir takım en az kaç kişi içerir?

#Cevap: Güvercin yuvası prensibi bize hepsinin farklı takımlarda oynayamayacağını söyler; yedi oyuncudan en az ikisini içeren en az bir takım olmalıdır.

#Ekrandan girilen takım sayısı ve kisi sayısına bağlı olarak bir takımda en az kaç kişi olabileceğini hesaplayan kod aşağıdaki gibidir.

import math
def pigeonholeprinciple():
    xx=True
    while xx==True:  
        kisi=int(input('kisi sayısı='))
        takim=int(input('takım sayısı='))
        if kisi >=  takim:
            bb = math.ceil(kisi / takim)
            print('en az bir takım', kisi, 'oyuncudan en az', bb ,'oyuncuya sahiptir')
            xx=False
        else:
            print('kisi sayisi takım sayısından büyük yada eşit olmalıdır!!')
            xx=True
    return
