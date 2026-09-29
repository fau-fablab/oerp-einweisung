OpenERP Einweisung
==================

Anleitungen des [FAU FabLab](https://fablab.fau.de) für das Warenwirtschaftssystem [OpenERP/Odoo](https://www.odoo.com/).

Inhalt
------

- Produkt anlegen: Kategorie, Artikelnummer, Preise, Lieferanten, Lagerort, Steuer
- Bestellung bei der MEW im ERP anlegen und Bestellformular ausfüllen
- Richtlinien zur Benennung der Lagerorte
- Neues Geschäftsjahr anlegen (noch sehr kurz)

Download
--------

Die neueste Version aus [GitHub](https://github.com/fau-fablab/oerp-einweisung) ist als PDF abrufbar:

- [Produkt anlegen](https://brain.fablab.fau.de/build/oerp-einweisung/Produkt_anlegen.pdf)
- [Bestellung bei MEW](https://brain.fablab.fau.de/build/oerp-einweisung/Bestellung_bei_MEW.pdf)
- [Richtlinien zur Lagerortbenennung](https://brain.fablab.fau.de/build/oerp-einweisung/lagerbenennung.pdf)
- [Neues Jahr / Periode](https://brain.fablab.fau.de/build/oerp-einweisung/Neues_Jahr_Periode.pdf)

Außerdem baut eine GitHub Action die PDFs bei jedem Push. Auf dem Hauptbranch entsteht dabei ein
[Release](https://github.com/fau-fablab/oerp-einweisung/releases) mit Datums-Version (`vJJJJ.MM.TT`) und den PDFs.

Auschecken und bauen
--------------------

```bash
git clone --recursive git@github.com:fau-fablab/oerp-einweisung.git
cd oerp-einweisung
make
```

Die PDFs landen in `output/`. Layout, Kopf- und Fußzeile und das Logo des FAU FabLab (mit
FAU-Schriftzug) kommen aus dem Untermodul [fablab-document](https://github.com/fau-fablab/fablab-document),
das Logo wiederum aus dessen Untermodul [logo](https://github.com/fau-fablab/logo). Bei einem bestehenden
Klon die Untermodule mit `git submodule update --init --recursive` laden.

Technische Details zum Buildserver: [fau-fablab/buildserver](https://github.com/fau-fablab/buildserver)

[![Build Status](https://brain.fablab.fau.de/build/oerp-einweisung/status.svg)](https://brain.fablab.fau.de/build/oerp-einweisung/)
[![TODOs](https://brain.fablab.fau.de/build/oerp-einweisung/status-todos.svg)](https://brain.fablab.fau.de/build/oerp-einweisung/)
[![PDF bauen](https://github.com/fau-fablab/oerp-einweisung/actions/workflows/pdf.yml/badge.svg)](https://github.com/fau-fablab/oerp-einweisung/actions/workflows/pdf.yml)

Lizenz
------

[![Lizenz: CC BY-SA 3.0](https://licensebuttons.net/l/by-sa/3.0/de/88x31.png)</br>CC BY-SA 3.0](https://creativecommons.org/licenses/by-sa/3.0/)
