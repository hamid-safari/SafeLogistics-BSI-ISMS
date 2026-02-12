Asset-ID,V,I,A,Begründung des Schutzbedarfs
VM-ERP,Hoch,Hoch,Sehr Hoch,Ein Ausfall führt zum sofortigen Stillstand der Logistikprozesse und verursacht massive finanzielle Schäden.
VM-SQL,Sehr Hoch,Sehr Hoch,Hoch,Enthält sensible Kundendaten (DSGVO-relevant) und alle Finanztransaktionen; Datenmanipulation hätte kritische Folgen.
NAS-01,Hoch,Sehr Hoch,Hoch,Zentrale Komponente der Backup-Strategie; die Integrität der Backups ist essenziell für die Wiederherstellung nach Ransomware-Angriffen.
CLI-02,Normal,Normal,Normal,"Standard-Arbeitsplatz; bei Defekt kurzfristig austauschbar, ohne den Gesamtbetrieb der SafeLogistics GmbH zu gefährden.

### 3.1 Zusammenfassung und Ergebnis
Die Analyse zeigt, dass die Verfügbarkeit des ERP-Systems und die Integrität der SQL-Datenbanken die kritischsten Faktoren für die SafeLogistics GmbH darstellen. 

**Kumulationseffekt:** Ein Ausfall der Virtualisierungsebene (SRV-01/02) führt zum gleichzeitigen Ausfall aller kritischen Anwendungen (ERP & SQL). Daher wird der Schutzbedarf für die Infrastruktur-Hosts analog zu den Gast-Systemen als "Hoch" bis "Sehr Hoch" eingestuft.

**Vererbungseffekt:**
Der Schutzbedarf der Fachanwendung (VM-ERP) überträgt sich direkt auf die Backup-Systeme (NAS-01), da ohne konsistente Backups die geforderte Verfügbarkeit nicht garantiert werden kann.