# 4. Modellierung nach BSI IT-Grundschutz-Kompendium

Die detaillierte Modellierung erfolgt in der Asset-Inventory-Liste. Hier ist eine Übersicht der wichtigsten Bausteine.

In dieser Phase werden den identifizierten Zielobjekten die entsprechenden Bausteine aus dem IT-Grundschutz-Kompendium zugeordnet.

## 4.1 Übergreifende Bausteine (General Modules)
Diese Bausteine gelten für den gesamten Informationsverbund:
* **ISMS.1:** Sicherheitsmanagement (Basis für das gesamte Projekt)
* **ORP.1:** Organisation (Rollen und Verantwortlichkeiten)
* **CON.1:** Kryptokonzept (für Verschlüsselung von ERP/SQL)
* **OPS.1.1.4:** Schutz vor Schadsoftware (Antivirus-Konzept)
* **DER.1:** Detektion und Reaktion (Incident Management)

## 4.2 Prozess- und System-Bausteine (Specific Modules)

| Asset-Gruppe | Baustein-ID | Titel des Bausteins |
| :--- | :--- | :--- |
| **Server-Infrastruktur** | **SYS.1.1** | Allgemeiner Server |
| **Virtualisierung** | **SYS.1.5** | Virtualisierung (für Hyper-V Cluster) |
| **Windows Server** | **SYS.1.2.2** | Windows Server 2022 |
| **Linux (ERP VM)** | **SYS.1.3** | Linux-Server |
| **Datenbanken** | **APP.4.3** | Relationale Datenbanksysteme (SQL) |
| **Netzwerk** | **NET.1.1** | Netzarchitektur und -design |
| **Firewall** | **NET.3.2** | Firewall |
| **Clients** | **SYS.2.1** | Allgemeiner Client (Windows 11) |
| **Cloud (M365)** | **OPS.2.2** | Cloud-Nutzung |
| **Backup (NAS)** | **OPS.1.1.5** | Protokollierung / Logging |

## 4.3 Begründung der Auswahl
Die Auswahl der Bausteine orientiert sich an der **Hybrid-Infrastruktur** der SafeLogistics GmbH. Besonders kritisch ist hierbei der Baustein **SYS.1.5 (Virtualisierung)**, da er die Basis für die Verfügbarkeit des ERP-Systems bildet.


