## Beschreibung des Netzplans (Zonierungskonzept)

Die Netzwerkinfrastruktur der SafeLogistics GmbH wurde gemäß **BSI IT-Grundschutz NET.1.1** in logische Sicherheitszonen unterteilt:

1. **Management-Zone (VLAN 10):** Isolierter Bereich für administrative Aufgaben (CLI-01) und Backup-Infrastruktur (NAS-01). Der Zugriff auf Server erfolgt ausschließlich über gesicherte Protokolle.
2. **Server-Zone / DMZ (VLAN 20):** Hier befinden sich die virtualisierten Kernanwendungen (ERP, SQL). Diese Zone ist durch die Firewall strikt von der Office-Zone getrennt.
3. **Office-Zone (VLAN 30):** Bereich für die Endgeräte der Mitarbeiter (Logistics-Laptops).
4. **External/Cloud:** Anbindung an Microsoft 365 über verschlüsselte Kanäle.

**Sicherheitsmechanismus:** Die Fortinet Firewall (FW-01) fungiert als zentraler Inspektion-Punkt für den gesamten Traffic zwischen den Zonen (Inter-VLAN Routing).


Hinweis zu Abhängigkeiten: Um die Übersichtlichkeit des Netzplans zu gewährleisten, wurden nur die kritischen logischen Datenflüsse (z.B. ERP zu SQL) explizit mit Pfeilen dargestellt. Infrastrukturelle Abhängigkeiten (wie VM zu Host oder Backup-Verbindungen) sind durch die Zonierung und Beschriftung impliziert