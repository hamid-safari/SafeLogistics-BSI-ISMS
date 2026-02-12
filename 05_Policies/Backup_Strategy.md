# 5. Datensicherungsrichtlinie (Backup Policy)

**Referenz Baustein:** BSI OPS.1.1.4 & CON.1

## 1. Zielsetzung
Diese Richtlinie definiert die Verfahren zur Sicherung und Wiederherstellung von Daten der SafeLogistics GmbH, um die Verfügbarkeit (Sehr Hoch) sicherzustellen.

## 2. Strategie (3-2-1 Regel)
Wir implementieren eine robuste Backup-Strategie:
* **3 Kopien:** Primärdaten + 2 Backups.
* **2 Medien:** Speicherung auf dem Synology NAS (NAS-01) und LTO-Tapes.
* **1 Offsite:** Eine Kopie wird physisch an einem externen Standort gelagert (Air-Gap).

## 3. Technische Umsetzung (Dein technischer Hintergrund)
* **Full-Backups:** Wöchentlich (Samstags um 22:00 Uhr).
* **Inkrementelle Backups:** Täglich (Alle 4 Stunden während der Betriebszeit).
* **Verschlüsselung:** Alle Backups werden mit AES-256 verschlüsselt (gemäß CON.1).
* **Recovery-Test:** Quartalsweise Durchführung von Wiederherstellungstests für das ERP-System.

## 4. Verantwortlichkeiten
Der IT-Administrator ist für die Überwachung der Backup-Jobs und die Durchführung der Tests verantwortlich.