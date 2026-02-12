# 1. Definition des Informationsverbunds (Scope) - SafeLogistics GmbH

## 1.1 Einleitung und Zielsetzung
Dieses Dokument definiert den Geltungsbereich für das Informationssicherheitsmanagementsystem (ISMS) der **SafeLogistics GmbH**. Ziel ist die Absicherung der kritischen Geschäftsprozesse durch die Implementierung des **BSI IT-Grundschutzes (Standard 200-2)**. 

Das Unternehmen ist ein mittelständischer Logistikdienstleister mit Sitz in Karlsruhe und beschäftigt ca. 45 Mitarbeiter.

## 1.2 Institutionelle Abgrenzung
Der Geltungsbereich umfasst alle Abteilungen, Mitarbeiter und IT-Ressourcen am Hauptstandort:
* **Standort:** Karlsruhe (Zentrale).
* **Mitarbeiter:** 45 (inkl. Disposition, Verwaltung und IT-Administration).

## 1.3 Analyse der Geschäftsprozesse
Folgende Kernprozesse sind für den Fortbestand des Unternehmens kritisch und stehen im Fokus des ISMS:
1. **Disposition & Fuhrparkmanagement:** Planung und Überwachung der Logistikketten.
2. **Finanzbuchhaltung:** Abwicklung von Zahlungen und Lohnabrechnungen.
3. **Kundenmanagement (CRM):** Verwaltung sensibler Kundendaten und Verträge.

## 1.4 Identifizierte Assets (Strukturanalyse)

### 1.4.1 IT-Infrastruktur (Hybrid-Umgebung)
* **Server-Systeme:** * 2x HPE ProLiant (Hyper-V Cluster für ERP und SQL-Datenbanken).
    * 1x Backup-Server (Synology NAS mit Air-Gap-Konzept).
* **Client-Infrastruktur:** 35x Managed Laptops (Windows 11), 10x Workstations für die Buchhaltung.
* **Netzwerkkomponenten:** Fortinet Firewall (Perimeter Security), Cisco Managed Switches (VLAN-Segmentierung).

### 1.4.2 Anwendungen und Dienste
* **ERP-System:** Fachspezifische Logistiksoftware zur Sendungsverfolgung.
* **Collaboration:** Microsoft 365 (Hybrid-Modell mit Exchange Online).
* **Datenbanken:** MS SQL Server für Bestandsdaten.

### 1.4.3 Infrastruktur und Räumlichkeiten
* **Serverraum:** Zutrittsgeschützter Bereich mit aktiver Kühlung und Brandmeldesystem.
* **Büroflächen:** Offene Arbeitsbereiche mit Clean-Desk-Policy-Anforderungen.

## 1.5 Netzwerktopologie und Zonierung
Die logische Netzwerkstruktur ist nach dem Prinzip der **Defense-in-Depth** in folgende Zonen unterteilt:
1. **Management-Zone:** Exklusiv für administrative Zugriffe (PAs).
2. **Server-Zone:** Beherbergt die ERP-Server und Datenbanken.
3. **Office-Zone:** Für Standard-Mitarbeiter-Endgeräte.
4. **DMZ:** Für externe Schnittstellen zum Cloud-ERP-Portal.

---
*Erstellt am: 12.02.2026*
*Version: 1.0*