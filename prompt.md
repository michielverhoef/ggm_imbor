Gebruikte AI: https://lovable.dev/

Gebruik input/VNGR SIM+Grouping NL-1.1-1.65.2.ea-toolbox.xml, dit is het profiel.

# Enumeraties. 
Gebruik input/enumeraties_domeinwaarden.xlsx
Kun je dit excel bestand als uml model weergeven? Verander geen relaties of namen.
Het formaat: het liefst xmi 2.1 geschikt voor EA.

Maak van de waarde van kolom Enumeratietype een Enumeration. Geef de Enumeration als naam de inhoud van kolom Enumeratietype voorafgegaan met de prefix "enum_". Als deze Enumeration al bestaat, gebruik deze dan.
Geef de Enumeration het Stereotype "Enumeratie" zoals in het profiel beschreven staat. Voeg de Tags uit de TaggedValues van Stereotype met name="Enumeratie" toe aan de Enumeration.
Voeg daarna de enumeratiewaarde toe met als naam de waarde van kolom Domeinwaarde.
Geef de enumeratiewaarde de Definition van de kolom DWdef.
Geef de enameratiewaarde het Stereotype "Enumeratiewaarde" zoals in het profiel beschreven staat. Voeg de Tags uit de TaggedValues van Stereotype met name="Enumeratiewaarde" toe aan het attribuut.


# Classes/Objecttypen, 
gebruik input/klassen_attributen.xlsx
Kun je dit excel bestand als uml model weergeven? Verander geen relaties of namen.
Het formaat: het liefst xmi 2.1 geschikt voor EA.

Maak van de waarde van kolom Klasse een Class. Als deze Class al bestaat, gebruik deze dan. Geef de Class het Stereotype "Objecttype" zoals in het profiel beschreven staat. Voeg de Tags uit de TaggedValues van Stereotype met name="Objecttype" toe aan de Class.
Voeg daarn het attribuut toe met als naam de waarde van kolom Attribuut. Geef dit attribuut het type van de kolom Datatype.
Als het Datatype gelijk is aan Enumeratie of Referentie maak het type een verwijzing naar de eerder gemaakte Enumerations. Verwijs naar de Enumeration met als naam de waarde van de kolom Enumeratietype voorafgegaan met de prefix "enum_". 
Geef het attribuut de Definition van de kolom Definitie plus de waarde van kolom Eenheid, gescheiden door een spatie.
Geef het attribuut het Stereotype "Attribuutsoort" zoals in het profiel beschreven staat. Voeg de Tags uit de TaggedValues van Stereotype met name="Attribuutsoort" toe aan het attribuut.


- De stereotypen en tagss zijn niet zichtbaar in de properties van de objecttypen en attributen in EA. Ook worden de verwijzingen naar de enumeraties bij attributen niet opgenomen. Kun je dit repareren:

    Stereotypen en tags zichtbaar in de properties van de objecttypen en attributen in EA
    attributen waar van toepassing in het type van de attributen opnemen

- Bijna goed. De stereotypen ontbreken nog bij de enumeratiewaarden. Kun je die nog toevoegen?

- Helaas, dit is niet het Stereotype uit het profiel. Kun je de Enumeratiewaarden het stereotype "Enumeratiewaarde" zo- als beschreven in het profiel geven? Kun je ook de tags behorend bij Stereotype met de naam "Enumeratiewaarde" toevoegen aan de enumeratiewaarden?



# GUIDs
Gebruik imbor_2025.xml dit bestand bevat de nieuwe versie van het model, dit is IMBOR2025.
Gebruik imbor_oud.xml, dit bestand bevat de oude versie van het model, dit is IMBOROUD.

Vergelijk IMBOR2025 met IMBOROUD.

Voor elk element met het xmi:type="uml:Class" (dit noemen we vanaf nu een Class) in IMBOR2025 zoek het element met xmi:type="uml:Class" 
(dit noemen we vanaf nu een ClassOud) met dezelfde naam in IMBOROUD. Vervang de waarde van het attribuut xmi:id van de Class IMBOR2025 met de waarde van het attribuut xmi:id van de ClassOud uit IMBOROUD. Doe dit voor alle classes in IMBOR2025.


Voor elk packagedElement met het xmi:type="uml:Enumeration" (dit noemen we vanaf nu een Enum) in IMBOR2025 zoek het packagedElement met xmi:type="uml:Enumeration" (dit noemen we vanaf nu een EnumOud) met dezelfde naam in IMBOROUD. 
Vervang de waarde van het attribuut xmi:id van de Enum uit IMBOR2025 met de waarde van het attribuut xmi:id van de EnumsOud uit IMBOROUD. Doe dit voor alle
Enums in IMBOR2025.



