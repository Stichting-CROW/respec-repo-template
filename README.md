# ReSpec-template

A GitHub repository template for CROW-style ReSpec documents, to be used for technical specifications.

> **Wat betekent dit voor mij**:
>
> - Voor een nieuw project: volg onderstaand stappenplan.
> - Voor een nieuw document binnen een bestaand project: volg het stappenplan op [stichting-crow/respec-document-template].

## Stappenplan nieuwe ReSpec (verander mij na kopie!)

Dit stappenplan gaat uit van de specificatiestandaarden van CROW.

Voor korte namen geldt:

- kleine letters
- geen underscores (`_`) maar koppeltekens (`-`).

1. Bedenk een **korte naam** voor het project.

   Dit wordt ook de naam van de GitHub-repository.
   _informatiemodel beheer openbare ruimte_: `imbor`,
   _datastandaard fietsparkeren_: `datastd-fietspark`,
   _standaard uitwisselingsformaat globale visuele weginspectiebestanden in RDF_: `stufweg-rdf`,
   etc.

2. Bedenk of werkversies en discussies niet-openbaar moeten zijn.

   Het wordt aanbevolen om werkversies publiek te bewerken.
   Openbare repositories zijn ook altijd gratis.
   Let op dat alle voorgaande versies van een document in GitHub altijd terug te halen zijn.
   Oncomplimenteuze opmerkingen, wachtwoorden, etc. blijven in principe\* altijd beschikbaar.

3. Klik op [_Use this template_](generate).

   Bij _owner_: ‘stichting-crow’ of de GitHub-organisatie van je werkgroep.  
   Bij _repository name_: de korte naam van het project.  
   Bij _description_: Een korte beschrijving van je project. Nederlands, Engels, mag allemaal.  
   Bij _public/private_: Als je het niet zeker weet, kies _public_.  
   Bij _include all branches_: Niet noodzakelijk.

Vervolgens maakt GitHub een nieuwe repository aan,
kopieert-ie de inhoud van [stichting-crow/respec-repo-template]
en start-ie het aanmaken van het eerste document binnen de repo.
Dat duurt zo'n 30 seconden, waarna het lampje in de balk bovenin op groen springt.

## Bewerken

Voor het bewerken van de bestanden kun je gebruiken

- de webinterface van Git (niet aangeraden)
- de webinterface van VS Code (druk op <kbd>.</kbd>)
- Visual Studio Code geïnstalleerd op je computer.

Voor VS Code worden er ook aanbevolen extensies meegegeven in deze repository.

## Publiceren

1. **Werkversies** (`DRAFT` of `WD`) worden continu gepubliceerd op `https://docs.crow.nl/{{repository-korte-naam}}/{{document-korte-naam}}.
2. **Referentieversies**, bijvoorbeeld voor een review of consultatie, maak je door naar [GitHub Actions](actions/workflows/lifecycle.yml) te gaan en daar op _Run workflow_ te drukken.
3. Voor op de startpagina van _docs.crow.nl_: zie de [README van docs.crow.nl][publiceer-readme].

## Configuratie

Lees de [beknopte handleiding voor ReSpec][wiki].

[ghio]: https://stichting-crow.github.io
[themas]: https://www.crow.nl/thema-s/
[wiki]: https://github.com/stichting-crow/respec/wiki
[publiceer-readme]: https://github.com/stichting-crow/stichting-crow.github.io/blob/main/README.md#publiceren
[stichting-crow/respec-document-template]: https://github.com/stichting-crow/respec-document-template
[stichting-crow/respec-repo-template]: https://github.com/stichting-crow/respec-repo-template
