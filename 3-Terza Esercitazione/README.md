# Esercitazione 3

## OPTIONAL
usato per catturare le trile che non sappaiamo se sono presenti mel grafo
SELECT ?label ?date
WHERE {
    ?iri rdfs:label ?label .
    OPTIONAL
        { ?iri dcterms:date ?date .}
    }

## UNION
unisce due graph pattern diversi

SELECT ?iri ?name
WHERE {
    ?iri a foaf:Person
    UNION { ?iri foaf:familiyName ?name .}
}

## COUNT
operatore epr contare

SELECT ?class (COUNT (?Cclass) AS ?count) 
WHERE {
    ?iri a ?class .
}GROUP BY ?class

Filter not exist
filatr i dati n base alla non esistenza
SELECT ?iri ?label
WHERE {
    ?iri a foaf:Person 
        rdfs:label label .
    FILTER NOT EXIST { ?iri :hasDog ?dog}
}

## MINUS
toglie i risultati che rispecchiano un pattern
SELECT ?iri ?label
WHERE {
    ?iri a foaf:Person 
        rdfs:label label .
    FILTER NOT EXIST { ?iri :hasDog ?dog}
}