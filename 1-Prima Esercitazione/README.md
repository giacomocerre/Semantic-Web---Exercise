**Piccoli HINT**

PARTE 1 (esercizi nelle cartella Base)

---@base--------------------------------------------------------------------------------------------------------------

Quando si usa termini di un vocabolario utilizzando path relativi con "@base" questi devono essere messi tra parentesi angolari e.g: <termine>

Una Tripla è composta da:
<soggetto> relazione <Oggetto> --> l'oggetto va sempre maiusolo il soggetto sempre minuscolo per convenzione.

----------------------------------------------------------------------------------------------------------------------


PARTE 2 (esercizi nelle cartella Prefix)

---@prefix------------------------------------------------------------------------------------------------------------

Quando si usa termini di un vocabolario utilizzando @prefix possiamo:
1- dare un nome al prefisso: @prefix nome: <vocabolario>

******************************************
Esempio con nome del prefisso (in questo caso "ex")
@prefix ex: <https://example.org/> .

ex:soggetto relazione ex:Oggetto
******************************************

2- utilizzare un prefisso di default che non necessita di un nome. ATTENZIONE in tutto il documento un prefisso di default può essere utilizzato solo una volta

******************************************
Esempio con prefisso di default (solo i ":")
@prefix : <https://example.org/> .

:soggetto relazione :Oggetto
******************************************

----------------------------------------------------------------------------------------------------------------------


---Valdazione del codice Turtle-----

http://ttl.summerofcode.be/

------------------------------------
