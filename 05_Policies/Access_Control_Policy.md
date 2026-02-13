5. Zugriffskontroll-Richtlinie (Access Control Policy)

Referenz Bausteine: BSI ORP.4 (Identitäts- und Berechtigungsmanagement) & SYS.1.2.2 (Windows Server)
1. Zielsetzung

Diese Richtlinie legt die Regeln für den Zugriff auf IT-Systeme und Daten der SafeLogistics GmbH fest. Ziel ist es, unbefugte Zugriffe zu verhindern و اطمینان از رعایت اصل Least Privilege است.
2. Identitätsmanagement (Active Directory)

Die Verwaltung aller Benutzerkonten erfolgt zentral über das Microsoft Active Directory (AD).

    Einmalige Identifikatoren: Jeder Mitarbeiter erhält eine eindeutige User-ID. Gemeinsam genutzte Konten (Generic Accounts) sind untersagt.

    Onboarding/Offboarding: Konten werden sofort nach dem Ausscheiden eines Mitarbeiters deaktiviert (gemäß ORP.4.A7).

    Passwort-Policy: Erzwingung komplexer Passwörter (mind. 12 Zeichen, MFA für Cloud-Zugriffe).

3. Berechtigungskonzept (RBAC)

Wir nutzen das Role-Based Access Control (RBAC) Modell:

    Gruppenrichtlinien (GPOs): Zugrechte werden ausschließlich über AD-Gruppen (nicht direkt auf User-Ebene) vergeben.

    Separation of Duties (SoD): Trennung zwischen administrativen und operativen Konten.

    Tiered Administration Model:  Mehrstufiges Verwaltungsmodell: Administratoren verfügen über zwei Benutzerkonten: eines für alltägliche Aufgaben und ein weiteres mit erweiterten Zugriffsrechten (Domänenadministrator), das ausschließlich für die Serververwaltung verwendet wird.

4. Privilegierte Zugriffe (PAs)

Besondere Anforderungen für Administratoren:

    Admin-Workstation: Administrative Aufgaben dürfen nur von der dedizierten CLI-01 durchgeführt werden.

    Remote Access: Externer Zugriff für Wartungsarbeiten erfolgt ausschließlich über eine verschlüsselte VPN-Verbindung mit 2-Faktor-Authentisierung (2FA).

5. Überprüfung (Review)

Alle Berechtigungen werden halbjährlich durch die Abteilungsleiter (z.B. Head of Logistics) und den IT-Admin überprüft (User Access Review)
