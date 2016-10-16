# JMBAG
0036483630

#Pitanje 1:
U folderu su dva nova filea, ClassLibrary1.dll i ClassLibrary1.pdb.
Ako pobrišem dll, aplikacija se ne može pokrenuti jer ne može loadati klasu iz ClassLibrary1 
koju koristimo u konzolnoj aplikaciji (CLR ne zna gdje bi ju tražio).
Da bi se program uspješno pokrenuo uz exe datoteku treba poslati i ClassLibrary1.dll
(ostale datoteke unutar debug foldera nisu nužne za pokretanje konzolne aplikacije).

#Pitanje 2:
Aplikacija je koristila staru verziju class library asemblija jer nismo buildali rješenje
da koristi novu verziju.

#Pitanje 3:
Ispisalo se Pero: Hello World.

#Pitanje 4:
U folderu se nalazi i PeroClassLibrary.dll.

#Pitanje 5:
Ako obrišem originalni dll na disku, aplikacija se normalno pokreće, ne bi radilo kada
bi pobrisala i dll koji se nalazi u debug folderu, očito se koristi taj dll što se može 
vidjeti iz references liste - navedeni path za pero dll je onaj do debug foldera.

#Pitanje 6:
Build se uspješno izvršio i nakon builda u packages direktoriju se ponovo 
nalazi nodatime folder.