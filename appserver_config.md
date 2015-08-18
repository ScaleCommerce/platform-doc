# Konfiguration der Appserver

Unsere Appserver verwenden Apache mit mod_php und ausgeschalteter .htaccess-Unterstützung.
Dies ist der performanteste Weg um eine PHP-Applikation zu betreibe.

## Wie bekomme ich dennoch Support für .htaccess?
Sämtliche Regeln, die es in .htaccess gibt, können auch in gleicher Syntax ditrekt in die Apache Konfiguration geschrieben werden.

**Nachteil:** Nach Änderungen daran, muss der Service einmal neue gestartet werden.

**Vorteil:** Da der Server nicht bei jedem Aufruf erneut alle Verzeichnisse prüfen muss, wird der Prozess wesentlich beschleunigt.

**Umsetzung:** Doku, wie Du die Konfiguration beeinflussen kannst folgt. Solange wende dich einfach per Mail oder HipChat an uns.