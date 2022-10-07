
# FOAF (friend of a friend)
E' un'ontologia che si usa per descrivere **PERSONE** in relazione con altre *Persone* e *Oggetti*.
<a href="http://xmlns.com/foaf/0.1/">Documentazione</a>

`@prefix foaf: <IRI>` --> sintassi generale

Alcune **Classi**:
- _Person_: `foaf:Person` è una classe che reappresenta le **persone** *(Qualcosa è un `foaf:person` se è una persona viva/morta/inventata/reale)* <a href="http://xmlns.com/foaf/0.1/#term_Person">doc.</a>
- _Organization_: La `foaf:Organization` è una classe che rappresenta le **istituzioni sociali come aziende, società ecc.** <a href="http://xmlns.com/foaf/0.1/#term_Organization">doc.</a>

alcune **Proprietà**:
- _knows_: `foaf:knows` Identifica la proprietà per la quale una persona conosce un'altra persona.**(type: foaf:Person)** - <a href="http://xmlns.com/foaf/0.1/#term_knows">doc.</a>
- _name_: `foaf:name` Idefica il nome di qualcosa **(type: xsd:string)** - <a href="http://xmlns.com/foaf/0.1/#term_name">doc.</a>
- _givenName_: `foaf_givenName` Identifica il nome di una persona **(type: xsd:string)** - <a href="http://xmlns.com/foaf/0.1/#term_givenname">doc.</a>
- _familyName_: `foaf:familiyName` Identifica il cognome di una persona **(type: xsd:string)** - <a href="http://xmlns.com/foaf/0.1/#term_family_name">doc.</a>
- _homepage_: `foaf:homepage` Identifica una risorsa o un documento. **(type: foaf:Agent)** - <a href="http://xmlns.com/foaf/0.1/#term_homepage">doc.</a>

# DUBLIN CORE
Metadati di risrse digitali o fisiche e.g.: biblioteche o archivi
3 namespace --> dc, dcterms, dytype

- `dctype:` per le classi
    - `dctype:Text` --> classe relative ai testi (book, poems, novels...) - <a>doc.</a>
    - `dctype:Event` - <a>doc.</a>
- `dcterms:` proprietà
    - `dcterms:creator` (IRI) - <a>doc.</a>
    - `dcterms:title` (xsd:string) - <a>doc.</a>
    - `dcterms:date` (xsd:date) - <a>doc.</a>
    - `dcterms:issued` (xsd:date) - <a>doc.</a> 
    - `dcterms: language` (IRI) - <a>doc.</a>

# Wikidata Knowledge Based
Free and Open. Può essere editata sia da bot che da umani.

## Link utili
https://prefix.cc/ --> serve per cercare gli IRI tramite un dato namespace
https://www.wikidata.org/entity/ --> wd: prefix for Wikidata IRI
