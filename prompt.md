Gebruikte AI: https://lovable.dev/

# Enumeraties. 
Gebruik input/enumeraties_domeinwaarden.xlsx
Kun je dit excel bestand als uml model weergeven? Verander geen relaties of namen.
Het formaat: het liefst xmi geschikt voor EA.

Maak van de waarde van kolom Enumeratietype een Enumeration. Geef de Enumeration als naam de inhoud van kolom Enumeratietype voorafgegaan met de prefix "enum_". Als deze Enumeration al bestaat, gebruik deze dan.
Voeg daarna de enumeratiewaarde toe met als naam de waarde van kolom Domeinwaarde.
Geef de enumeratiewaarde de Definition van de kolom DWdef


# Classes/Objecttypen, 
gebruik input/klassen_attributen.xlsx
Kun je dit excel bestand als uml model weergeven? Verander geen relaties of namen.
Het formaat: het liefst xmi geschikt voor EA.

Maak van de waarde van kolom Klasse een Class. Als deze Class al bestaat, gebruik deze dan.
Voeg daarn het attribuut toe met als naam de waarde van kolom Attribuut. Geef dit attribuut het type van de kolom Datatype.
Als het Datatype gelijk is aan Enumeratie of Referentie maak het type een verwijzing naar de eerder gemaakte Enumerations. Verwijs naar de Enumeration met als naam de waarde van de kolom Enumeratietype voorafgegaan met de prefix "enum_". 
Geef het attribuut de Definition van de kolom Definitie plus de waarde van kolom Eenheid, gescheiden door een spatie.


# MIM profiel
TODO
