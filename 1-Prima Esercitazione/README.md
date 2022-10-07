# Concetti di base
## Triple
Una tripla la descrizione tramite tre _"entità"_ di una relazione. Una tripla si decrive come:
un **Soggetto** in relazione con un **Oggetto** tramite l'uso di un predicato detto **Relazione**.

Generalmente quindi: _`Soggetto relazione Oggetto`_
## Prefissi
### @base
 _(Esercizi della cartella [Base](./Base/))_

Quando si usa termini di un vocabolario utilizzando **path relativi con `@base`** questi devono essere messi tra **parentesi angolari** e.g: `<termine>`

Una Tripla viene scritta formalemte, quando utilizziamo `@base`,questo modo:
`<soggetto> relazione <Oggetto>` --> l'***oggetto va sempre maiusolo** il ***soggetto sempre minuscolo*** per convenzione.

```
@base <http://example.com/> 

<soggetto> relazione <Oggetto>
```

### @prefix

_(Esercizi della cartella [Prefix](./Prefix/))_

Quando si usa termini di un vocabolario utilizzando `@prefix` possiamo:
1. _dare un nome al prefisso_: `@prefix nome: <IRI>`

```esempio
@prefix ex: <https://example.org/> .

ex:soggetto relazione ex:Oggetto
```

2. Utilizzare un **prefisso di default** (_solo :_) che non necessita di un nome.
***ATTENZIONE*** in tutto il documento un prefisso di default può essere utilizzato solo una volta

```
@prefix : <https://example.org/> .

:soggetto relazione :Oggetto
```
