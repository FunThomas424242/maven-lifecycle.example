# maven-lifecycle.example
Beispiel zum Erstellen eines Maven Plugin mit eigenem Lifecycle

* Für den Lifecycle bieten sich Dinge an welche in einem Prozess über mehrere Phasen erstellt werden, z.B.:
 * Aus Videos eine DVD erstellen. Dabei müssen die Videos in Ton und Bild zerlegt, in Stücke geschnitten, vermixt und mit einem Menü versehen auf eine DVD gebrannt werden. Diese Anwendung eignet sich nicht als Beispiel da sehr viele weitere Werkzeuge mit eingebunden werden müssten und das Beispiel dann zu komplex wird.
 * Ein Backup erstellen. Das ist hoffentlich ein einfacher Prozess mit nur ein paar Phasen in denen irgenwie mal Daten kopiert, komprimiert, versioniert und mit Metainformationen versehen werden. Auch müssen irgenwann alte Daten gelöscht werden. Das klingt nach einem Umfang den das Beispiel leisten kann. 
 
## Phasen eines Backups
1. Quellverzeichnis scannen und Veränderungen merken.
2. Delta oder vollen Datenbestand kopieren
3. Datenbestand komprimieren
4. Metadaten hinzufügen
5. Obsolete Daten löschen z.B. bei rollierendem Backup
6. Status schreiben oder Report ausgeben.

# Quellen

* http://blog.sonatype.com/2009/08/create-a-customized-build-process-in-maven/
* http://www.ukrebs-software.de/german/back4sure/doc/chapter_4.html (Phasen eines Backups)
* 

