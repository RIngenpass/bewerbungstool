# bewerbungstool
Bewerbungstool

 <img src="Screenshot 2025-05-28 100248.png" alt="Projektlogo" width="300">

Benutzerdokumentation - Bewerbungstool
1. Einleitung
Das Bewerbungstool dient der automatisierten Erstellung von individuellen Bewerbungsschreiben. Es nutzt Word-Vorlagen mit Platzhaltern, die automatisch durch Bewerberdaten ersetzt werden. Anschließend werden die fertigen Bewerbungen als PDF-Dateien gespeichert. Das Tool bietet auch eine Massengenerierung für mehrere Unternehmen.
2. Systemanforderungen
•	Windows 10 oder höher
•	.NET 8.0 Runtime
•	Microsoft Word installiert (für Platzhalterersetzung)
•	PDF-Reader empfohlen
3. Installation
•	Das Projekt lässt sich mit Visual Studio öffnen (über Bewerbungstool.sln).
•	Alternativ kann die EXE aus dem Debug/Release-Ordner verwendet werden.
•	Alle Vorlagen- und Datendateien müssen im gleichen Verzeichnis wie die EXE liegen.
4. Bedienungsanleitung
4.1 Einzelbewerbung erstellen
1.	Starte das Programm.
2.	Gib im Formular deine persönlichen Daten ein.
3.	Lade eine Word-Vorlage mit Platzhaltern (z. B. {{Vorname}}, {{Nachname}}, {{Firma}}).
4.	Klicke auf "Bewerbung erstellen".
5.	Die generierte Bewerbung wird als PDF gespeichert.
4.2 Massengenerierung
1.	Lade eine Textdatei mit den Firmendaten (z. B. Firmenname, Ansprechpartner, Adresse).
2.	Gib deine Bewerberdaten einmal ein.
3.	Klicke auf "Massen-Erstellen".
4.	Das Tool erstellt für jede Firma ein individuelles Anschreiben als PDF.
4.3 PDF-Vorschau anzeigen
•	Nach der Generierung kannst du das PDF im Vorschaufenster öffnen.
4.4 Unterschrift hinzufügen
•	Beim Start wirst du gefragt, ob eine digitale Unterschrift verwendet werden soll.
•	Wenn "Ja" gewählt wird, erscheint eine Datei-Auswahl zur Auswahl einer Bilddatei (z. B. .png).
5. Hauptfunktionen im Überblick
•	WordChanger: Ersetzt Platzhalter in Word-Vorlagen.
•	ConvertToPDF: Konvertiert die Word-Datei in eine PDF.
•	PdfMerger: Führt mehrere PDFs zusammen (z. B. Anschreiben + Lebenslauf).
•	LoadData: Liest Daten aus CSV/TXT-Dateien ein.
6. Fehlerbehandlung
•	Fehlerhafte Vorlagen (falsche Platzhalter) führen zu einer Fehlermeldung.
•	Wenn Word nicht installiert ist, kann keine Generierung erfolgen.
•	Pfade mit Sonderzeichen sollten vermieden werden.
7. Kontakt / Support
Bei Problemen wenden Sie sich bitte an den Entwickler: Rene Ingenpas	
________________________________________


Aufbau der Textdatei für die Massengeneration:
		Firma=    		Hier muss der Firmenname stehen
 		zuHaenden=		Hier der Ansprechpartner oder die Personalabteilung
 		Strasse= 		Hier die Straße der Firma
 		PLZ=			Hier die PLZ, sowie Ort 47554 Musterstadt
		Title=			Der Titel für die Bewerbung. z.B. „Bewerbung als…“
 		Bewerbungstex1=  	Der erste Absatz der Bewerbung, meist der Text warum      					man sich auf diese Firma bewirbt
 		Bewerbungstex2= 	Der zweite Absatz über deine Qualifikationen
 		Bewerbungstex3=	Zeitpunkt etc. ab wann man zur Verfügung steht 
		Bewerbungstex4= 	Abschluss der Bewerbung, z.B. Ich freue mich sehr,  					wenn ich Ihr Team in dieser Zeit tatkräftig unterstützen					darf. Über eine Einladung zum persönlichen Gespräch					freue ich mich sehr.

Aufbau der Vorlage:
 	*der Header:
	 

 	*Die Anschrift der Firma:

 
 	*Die Bewerbung an sich:
 
