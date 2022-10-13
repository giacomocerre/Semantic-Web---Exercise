
# FOAF (friend of a friend)
E' un'ontologia che si usa per descrivere **PERSONE** in relazione con altre *Persone* e *Oggetti*.
<a href="http://xmlns.com/foaf/0.1/">Documentazione</a>

`@prefix foaf: <IRI>` --> sintassi per la dichiarazione

Alcune **Classi**:
- _Person_: `foaf:Person` è una classe che reappresenta le **persone** *(Qualcosa è un `foaf:person` se è una persona viva/morta/inventata/reale)* <a href="http://xmlns.com/foaf/0.1/#term_Person">doc.</a>
- _Organization_: La `foaf:Organization` è una classe che rappresenta le **istituzioni sociali come aziende, società ecc.** <a href="http://xmlns.com/foaf/0.1/#term_Organization">doc.</a>

Alcune **Proprietà**:
- _knows_: `foaf:knows` Identifica la proprietà per la quale una persona conosce un'altra persona.**(type: foaf:Person)** - <a href="http://xmlns.com/foaf/0.1/#term_knows">doc.</a>
- _name_: `foaf:name` Idefica il nome di qualcosa **(type: xsd:string)** - <a href="http://xmlns.com/foaf/0.1/#term_name">doc.</a>
- _givenName_: `foaf_givenName` Identifica il nome di una persona **(type: xsd:string)** - <a href="http://xmlns.com/foaf/0.1/#term_givenname">doc.</a>
- _familyName_: `foaf:familiyName` Identifica il cognome di una persona **(type: xsd:string)** - <a href="http://xmlns.com/foaf/0.1/#term_family_name">doc.</a>
- _homepage_: `foaf:homepage` Identifica una risorsa o un documento. **(type: foaf:Agent)** - <a href="http://xmlns.com/foaf/0.1/#term_homepage">doc.</a>

</hr>

# DUBLIN CORE
Metadati di risrse digitali o fisiche e.g.: biblioteche o archivi
3 namespace --> `dc`, `dcterms`, `dytype`

`@prefix dc: <IRI>` --> sintassi per la dichiarazione

Alcune **Classi**

Per le classi si usa `dctype:`:
- _Text_: `dctype:Text` Identifica una classe per esprimere **libri, lettere, dissertazioni, poesie, giornali, articoli, etc...** - <a href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/dcmitype/Text/">doc.</a>
- _Event_: `dctype:Event` Identifa una classe per esprimere un evento non persistente, basato sul tempo come ad esempio una **mostra, una conferenza etc..** - <a  href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/dcmitype/Event/">doc.</a>

Alcune **Proprietà**:

Per le proprietà si usa `dcterms:`
- _creator_: `dcterms:creator` Idenfica un entità responsabile della creazione di una risorsa **(type: IRI)** - <a  href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#creator">doc.</a>
- _title_: `dcterms:title` Identifica il nome di un risorsa **(type: xsd:string)** - <a  href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/title">doc.</a>
- _date_: `dcterms:date` Identifica una data nei formato <a href="https://www.w3.org/TR/NOTE-datetime">W3CDTF</a> **(type: xsd:date)** - <a  href="https://www.dublincore.org/specifications/dublin-core/dcmi-terms/#http://purl.org/dc/terms/date">doc.</a>
- _issued_: `dcterms:issued` Identifica una **data di rilascio di un risorsa in modo formale**. Si puo mettere solo la _data_ oppure anche _data/ora_ **(type: xsd:date)** - <a  href="">doc.</a> 
- _language_: `dcterms: language` Identifica il **linguaggio di una risorsa** in formato no letterale. Si possono usare solo quelli esistendi negli standard _ISO 639-2_ o _ISO 639-3_ o un _tag IETF Best Current Practice 47_<a href="https://www.rfc-editor.org/info/bcp47">[ IETF ]</a>  **(type: IRI)** - <a  href="">doc.</a>

# Wikidata Knowledge Based
Free and Open. Può essere editata sia da bot che da umani.</br>
<a href="https://www.wikidata.org/entity/">WikiData</a>

`@prefix wd: <IRI>` --> sintassi per la dichiarazione


## Link utili
- <a href="https://prefix.cc/]">Sito per trovare gli IRI tramite un n amesapce specifico `www.prefix.cc`</a> 
- <a href="http://ttl.summerofcode.be/">Sito per la validazione del codice Tutrtle</a>