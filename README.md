# ISMS-Implementierung nach BSI IT-Grundschutz (SafeLogistics GmbH)

Dieses Projekt demonstriert die schrittweise Planung und Modellierung eines Informationssicherheitsmanagementsystems (ISMS) für ein mittelständisches Logistikunternehmen gemäß dem **BSI IT-Grundschutz-Standard 200-2**.

##  Projektübersicht
Das Ziel dieses Projekts ist es, die kritischen Geschäftsprozesse der SafeLogistics GmbH durch strukturierte Sicherheitsanalysen und Richtlinien abzusichern. Es verbindet administrative IT-Erfahrung mit regulatorischen Compliance-Anforderungen.

##  Projektstruktur
Das Repository ist nach den Phasen der BSI-Methodik gegliedert:

* **01_Scope_and_Context**: Definition des Geltungsbereichs und der Rahmenbedingungen.
* **02_Strukturanalyse**: Vollständige Asset-Inventarisierung und Erstellung des Netzplans (Topologie).
* **03_Schutzbedarfsfeststellung**: Klassifizierung der Assets nach Vertraulichkeit, Integrität und Verfügbarkeit.
* **04_Modellierung**: Zuordnung relevanter BSI-Bausteine (z.B. SYS.1.1, APP.4.3) zu den Zielobjekten.
* **05_Policies**: Operative Sicherheitsrichtlinien (Backup-Strategie & Access Control).
* **06_Mapping_ISO_BSI**: Konformitätsmatrix zwischen ISO/IEC 27001:2022 und BSI IT-Grundschutz.

##  Verwendete Technologien & Standards
* **Standards**: BSI IT-Grundschutz (Kompendium 2023), ISO/IEC 27001:2022.
* **Tools**: Microsoft Excel (Asset-Inventory), Draw.io (Netzplan), Git/GitHub (Docs-as-Code).
* **Infrastruktur-Fokus**: Windows Server 2022, Linux (Ubuntu), Fortinet Firewall, Microsoft 365 Cloud.

## Highlights des Projekts
* **Zonierungskonzept**: Trennung des Netzwerks in Management, Server (DMZ) und Office-Zonen zur Minimierung von Lateral Movement.
* **3-2-1 Backup-Strategie**: Implementierung einer Ransomware-resilienten Sicherung.
* **Tiered Admin Model**: Absicherung der Active Directory Administration.
