# Eignungstest Fachinformatiker Systemintegration - Komplettübersicht

## 📋 Struktur der IHK-Abschlussprüfung

### Abschlussprüfung Teil 1 (AP1) - nach 18 Monaten
**Gewichtung:** 20% der Gesamtnote
- **Dauer:** 90 Minuten
- **Punkte:** 100
- **Thema:** Einrichten eines IT-gestützten Arbeitsplatzes

### Abschlussprüfung Teil 2 (AP2) - am Ende der Ausbildung
**Gewichtung:** 80% der Gesamtnote

**Prüfungsbereich 1: Konzeption und Administration von IT-Systemen**
- Dauer: 90 Minuten
- Punkte: 100
- Gewichtung: 40%

**Prüfungsbereich 2: Analyse und Entwicklung von Netzwerken**
- Dauer: 90 Minuten
- Punkte: 100
- Gewichtung: 40%

**Prüfungsbereich 3: Wirtschafts- und Sozialkunde**
- Dauer: 60 Minuten
- Punkte: 100
- Gewichtung: 10%

**Prüfungsbereich 4: Betriebliche Projektarbeit**
- Projektdokumentation + Präsentation + Fachgespräch
- Gewichtung: 50% von AP2

---

## 🎯 Themengebiete im Detail

### 1. HARDWARE & ARBEITSPLÄTZE

#### Was du wissen musst:
- **Hardwarekomponenten:**
  - CPU-Typen (Intel Core i3/i5/i7/i9, Xeon, AMD Ryzen, Threadripper)
  - RAM-Typen (DDR4, DDR5, ECC-RAM für Server)
  - Speicher (HDD, SSD, NVMe, RAID-Level 0/1/5/6/10)
  - Grafikkarten (Workstation vs. Gaming)

- **Bedarfsermittlung:**
  - Hardware-Anforderungen je nach Einsatzzweck (Office, CAD, Entwicklung, Server)
  - Berechnungen: RAM-Bedarf, Storage-Bedarf, USV-Dimensionierung

- **Peripherie:**
  - Monitore (Auflösung, Bildwiederholrate, Panel-Technologien IPS/TN/VA)
  - Eingabegeräte (ergonomische Aspekte)
  - Drucker/Scanner (Laser, Inkjet, Multifunktionsgeräte)

- **Energieversorgung:**
  - USV-Berechnung (VA, Watt, Leistungsfaktor)
  - Überbrückungszeiten
  - Batteriekapazität (Ah-Berechnung)

#### Typische Aufgabenstellungen:
- Arbeitsplatz-Konfiguration für verschiedene Berufsgruppen
- Berechnungen: RAM-Bedarf für spezielle Anwendungen
- USV-Dimensionierung für Serversysteme
- Wirtschaftlichkeitsvergleich verschiedener Hardwarelösungen

---

### 2. NETZWERKTECHNIK

#### OSI-Modell (auswendig lernen!)
1. **Physical Layer** - Kabel, Hubs, Repeater
2. **Data Link Layer** - Switches, MAC-Adressen, Ethernet
3. **Network Layer** - Router, IP-Adressen, Routing
4. **Transport Layer** - TCP/UDP, Ports
5. **Session Layer** - Sitzungsverwaltung
6. **Presentation Layer** - Verschlüsselung, Kodierung
7. **Application Layer** - HTTP, SMTP, DNS, FTP

#### IP-Adressen & Subnetting (SEHR WICHTIG!)
- **IPv4:**
  - Klassen A, B, C, D, E
  - Private Netze (10.0.0.0/8, 172.16.0.0/12, 192.168.0.0/16)
  - Subnetzmasken (CIDR-Notation: /24, /25, /26...)
  - **VLSM** (Variable Length Subnet Masking) - häufig geprüft!

- **Berechnungen können:**
  - Netzadresse bestimmen
  - Broadcast-Adresse bestimmen
  - Anzahl nutzbarer Hosts: 2^(32-Prefix) - 2
  - Subnetz in kleinere Subnetze aufteilen

- **IPv6:**
  - Aufbau (8 Blöcke à 4 Hexadezimalziffern)
  - Kurzschreibweisen
  - Link-Local, Unique Local, Global Unicast
  - Vorteile gegenüber IPv4

#### VLANs (Virtual LANs)
- Zweck: Segmentierung, Sicherheit, Broadcast-Domains trennen
- VLAN-Tagging (802.1Q)
- Trunk-Ports vs. Access-Ports
- Inter-VLAN-Routing (Layer 3 Switch, Router-on-a-Stick)

#### Routing & Switching
- **Routing-Protokolle:**
  - Statisches Routing
  - Dynamisches Routing (RIP, OSPF, BGP - Grundlagen)
  - Default-Route (0.0.0.0/0)

- **Switching-Konzepte:**
  - MAC-Adress-Tabelle
  - Spanning Tree Protocol (STP) - Loop-Vermeidung
  - Port-Security
  - VTP (VLAN Trunking Protocol)

#### WLAN
- Standards: 802.11a/b/g/n/ac/ax (Wi-Fi 6)
- Frequenzen: 2,4 GHz vs. 5 GHz
- Sicherheit: WPA2, WPA3, Enterprise (RADIUS)
- Captive Portal, SSID-Broadcasting

#### Netzwerkprotokolle (wichtigste merken!)
- **DNS** (Port 53) - Namensauflösung
- **DHCP** (Port 67/68) - IP-Vergabe
- **HTTP/HTTPS** (Port 80/443)
- **FTP** (Port 21), **SFTP** (Port 22)
- **SMTP** (Port 25/587), **IMAP** (Port 993), **POP3** (Port 995)
- **RDP** (Port 3389), **SSH** (Port 22)
- **SMB/CIFS** (Port 445) - Windows-Freigaben
- **SNMP** (Port 161/162) - Monitoring

---

### 3. WINDOWS SERVER & ACTIVE DIRECTORY

#### Active Directory Domain Services (AD DS)
- **Struktur:**
  - Forest (Gesamtstruktur)
  - Tree (Baumstruktur)
  - Domain (Domäne)
  - Organizational Units (OUs)

- **Objekte:**
  - Benutzer
  - Gruppen (Sicherheitsgruppen vs. Verteilergruppen)
  - Computer
  - Gruppenrichtlinien (GPOs)

#### Gruppenrichtlinien (GPOs)
- **Anwendungsbereiche:**
  - Computer Configuration (gilt für Computer)
  - User Configuration (gilt für Benutzer)

- **Typische Einstellungen:**
  - Passwortrichtlinien (Komplexität, Länge, Ablauf)
  - Software-Verteilung
  - Bildschirmsperre
  - USB-Zugriff beschränken
  - Windows Update Einstellungen
  - Ordnerumleitung

- **Vererbung & Filterung:**
  - LSDOU-Reihenfolge (Local, Site, Domain, OU)
  - Enforced (erzwingen)
  - Block Inheritance

#### Benutzer- und Rechteverwaltung
- **Admin-Rollen:**
  - Domain Admin (volle Rechte in Domäne)
  - Enterprise Admin (volle Rechte in Forest)
  - Schema Admin (darf AD-Schema ändern)
  - Least Privilege Prinzip beachten!

- **Roaming Profiles** - Benutzerprofil folgt dem User
- **Folder Redirection** - Dokumente auf Server
- **Logon Scripts** - Automatisierung bei Anmeldung

#### Windows Server-Rollen
- **DNS-Server**
- **DHCP-Server**
- **File Server** (DFS - Distributed File System)
- **Print Server**
- **Hyper-V** (Virtualisierung)
- **Windows Deployment Services (WDS)** - OS-Verteilung

---

### 4. LINUX-GRUNDLAGEN

#### Wichtigste Befehle
```bash
# Dateiverwaltung
ls, cd, pwd, mkdir, rm, cp, mv, touch, cat, less, grep, find

# Rechteverwaltung
chmod, chown, chgrp
# Beispiel: chmod 755 datei.txt (rwxr-xr-x)

# Prozesse
ps, top, htop, kill, systemctl

# Netzwerk
ip addr, ifconfig, ping, traceroute, netstat, ss

# Paketverwaltung
apt (Debian/Ubuntu), yum/dnf (RedHat/CentOS)

# Texteditor
nano, vim
```

#### Berechtigungen (rwx-System)
```
r = 4 (Read)
w = 2 (Write)
x = 1 (Execute)

755 = rwxr-xr-x (Owner: rwx, Group: r-x, Others: r-x)
644 = rw-r--r-- (Owner: rw, Group: r, Others: r)
```

#### Wichtige Verzeichnisse
- `/etc` - Konfigurationsdateien
- `/var` - Variable Daten (Logs in /var/log)
- `/home` - Benutzerverzeichnisse
- `/usr` - Programme
- `/tmp` - Temporäre Dateien

---

### 5. VIRTUALISIERUNG

#### Hypervisor-Typen
- **Typ 1 (Bare Metal):**
  - VMware ESXi, Microsoft Hyper-V, Xen, KVM
  - Läuft direkt auf Hardware
  - Besser für Produktion

- **Typ 2 (Hosted):**
  - VMware Workstation, VirtualBox, Parallels
  - Läuft auf Host-OS
  - Für Test/Entwicklung

#### VMware vSphere-Konzepte
- **ESXi** - Der Hypervisor
- **vCenter** - Zentrale Verwaltung
- **vMotion** - Live-Migration von VMs (ohne Downtime)
- **High Availability (HA)** - Automatischer Restart bei Host-Ausfall
- **DRS** (Distributed Resource Scheduler) - Load Balancing
- **Fault Tolerance** - Vollständige Redundanz (Lockstep)

#### Ressourcen-Management
- **CPU:**
  - vCPU vs. physische Cores
  - CPU-Overcommitment (Ratio 2:1 bis 4:1 möglich)

- **RAM:**
  - Overcommitment mit Ballooning, Compression, Swapping
  - Memory Reservation vs. Limit

- **Storage:**
  - **Thin Provisioning** - wächst dynamisch (spart Platz)
  - **Thick Provisioning** - volle Größe sofort (bessere Performance)
  - VMFS (VMware File System)
  - Datastore

#### Container vs. VMs
| Merkmal | Virtual Machine | Container |
|---------|----------------|-----------|
| Isolation | Vollständig (eigenes OS) | Shared Kernel |
| Startup | Minuten | Sekunden |
| Größe | GB | MB |
| Performance | Overhead durch Hypervisor | Fast native |
| Einsatz | Legacy-Apps, volle Isolation | Microservices, Cloud-Native |

---

### 6. DATENSICHERHEIT & BACKUP

#### Backup-Strategien
- **Vollbackup (Full)** - Alles sichern
- **Inkrementell** - Nur Änderungen seit letztem Backup (klein, aber langsamer Restore)
- **Differentiell** - Änderungen seit letztem Vollbackup (größer, aber schnellerer Restore)

#### 3-2-1-Regel (merken!)
- **3** Kopien der Daten
- **2** verschiedene Medientypen (z.B. Disk + Tape)
- **1** Kopie offsite (extern, geografisch getrennt)

#### RPO & RTO
- **RPO** (Recovery Point Objective) - Wie viel Datenverlust ist akzeptabel? (z.B. 1 Stunde)
- **RTO** (Recovery Time Objective) - Wie schnell muss System wiederhergestellt sein? (z.B. 4 Stunden)

#### Snapshot vs. Backup
- **Snapshot:** Zustandsabbild (temporär, keine vollständige Kopie!)
- **Backup:** Vollständige Kopie auf anderem Medium

#### Disaster Recovery Plan (DRP)
- Notfallplan bei Totalausfall
- Beinhaltet: Backup-Strategie, Ersatzhardware, Kommunikationsplan
- Regelmäßige Tests!

---

### 7. IT-SICHERHEIT

#### Firewall
- **Stateful vs. Stateless:**
  - Stateless: Jedes Paket einzeln (alt)
  - Stateful: Verbindungen tracken (modern)

- **Next-Generation Firewall (NGFW):**
  - Application Control (nicht nur Ports, sondern Apps erkennen)
  - IPS (Intrusion Prevention)
  - URL-Filtering
  - SSL-Inspection
  - Sandboxing

- **DMZ (Demilitarized Zone):**
  - Pufferzone zwischen Internet und internem Netz
  - Für Webserver, Mailserver, etc.

#### VPN (Virtual Private Network)
- **Typen:**
  - **Site-to-Site** - Standorte verbinden
  - **Remote Access** - Einzelne User

- **Protokolle:**
  - **IPsec** - Network-Layer, NAT-Probleme
  - **SSL-VPN / TLS** - Application-Layer, browserbasiert möglich
  - **WireGuard** - Modern, schnell, einfach

- **Split-Tunneling:**
  - Nur Firmen-Traffic über VPN
  - Vorteil: Bandbreite sparen
  - Nachteil: Sicherheitsrisiko

#### Verschlüsselung
- **Symmetrisch:** AES (schnell, gleicher Schlüssel)
- **Asymmetrisch:** RSA (langsam, Public/Private Key)
- **Hybrid:** TLS/SSL (asymmetrisch für Schlüsselaustausch, dann symmetrisch)

#### Malware-Arten
- **Virus** - Benötigt Wirtsprogramm
- **Wurm** - Verbreitet sich selbst
- **Trojaner** - Tarnt sich als nützliche Software
- **Ransomware** - Verschlüsselt Daten, fordert Lösegeld
- **Spyware** - Ausspionieren
- **Rootkit** - Versteckt sich tief im System

#### Authentifizierung
- **Faktoren:**
  - Wissen (Passwort)
  - Besitz (Token, Smartcard)
  - Biometrie (Fingerabdruck)

- **Multi-Faktor-Authentifizierung (MFA/2FA):** Kombination mehrerer Faktoren

---

### 8. DATENBANKEN

#### Relationale Datenbanken
- **Produkte:** MySQL, PostgreSQL, Oracle, Microsoft SQL Server
- **SQL-Grundlagen:**
  - SELECT, INSERT, UPDATE, DELETE
  - WHERE, ORDER BY, GROUP BY, JOIN
  - Primärschlüssel, Fremdschlüssel

#### ACID-Eigenschaften (wichtig!)
- **Atomicity** - Alles oder nichts (Transaktion)
- **Consistency** - Konsistente Zustände (Constraints)
- **Isolation** - Transaktionen isoliert
- **Durability** - Dauerhafte Speicherung nach Commit

#### Hochverfügbarkeit
- **Master-Slave-Replikation** - Asynchron, Lesezugriffe auf Slaves
- **Master-Master-Replikation** - Synchron, beide schreibbar
- **Clustering** - Oracle RAC, MySQL Cluster

#### Index
- Beschleunigt Abfragen (wie Inhaltsverzeichnis)
- B-Tree-Struktur
- **Nachteil:** UPDATE/INSERT langsamer

---

### 9. MONITORING & ITSM

#### SNMP (Simple Network Management Protocol)
- **Polling:** Monitoring-System fragt ab (aktiv)
- **Traps:** Gerät sendet bei Event (passiv)
- MIB (Management Information Base) - Datenstruktur

#### ITIL-Basics
- **Incident:** Störung (sofort beheben)
- **Problem:** Ursache (langfristig analysieren)
- **Change:** Geplante Änderung (Change-Request erforderlich)
- **Service Level Agreement (SLA):** Vereinbarte Verfügbarkeit/Reaktionszeit

#### Verfügbarkeitsberechnung
```
Verfügbarkeit = MTBF / (MTBF + MTTR) × 100%

MTBF = Mean Time Between Failures (Zeit zwischen Ausfällen)
MTTR = Mean Time To Repair (Reparaturzeit)
```

**Verfügbarkeitsklassen:**
- 99% = 3,65 Tage Ausfall/Jahr
- 99,9% = 8,76 Stunden Ausfall/Jahr
- 99,99% = 52,56 Minuten Ausfall/Jahr
- 99,999% (Five Nines) = 5,26 Minuten Ausfall/Jahr

#### Redundanz-Berechnung
- **Serienschaltung:** Verfügbarkeit multiplizieren (A × B)
- **Parallelschaltung:** 1 - (1 - A) × (1 - B)

---

### 10. DATENSCHUTZ (DSGVO)

#### Grundprinzipien
- **Rechtmäßigkeit, Verarbeitung nach Treu und Glauben**
- **Zweckbindung** - Nur für bestimmten Zweck
- **Datenminimierung** - Nur notwendige Daten
- **Richtigkeit**
- **Speicherbegrenzung** - Löschen, wenn nicht mehr nötig
- **Integrität und Vertraulichkeit**

#### Betroffenenrechte
- Auskunftsrecht
- Recht auf Berichtigung
- Recht auf Löschung ("Recht auf Vergessenwerden")
- Recht auf Datenübertragbarkeit

#### TOMs (Technische und Organisatorische Maßnahmen)
- Zutrittskontrolle (Gebäudezugang)
- Zugangskontrolle (IT-System-Zugang)
- Zugriffskontrolle (Berechtigungen)
- Verschlüsselung
- Pseudonymisierung
- Backup
- Schulungen

#### Pseudonymisierung vs. Anonymisierung
- **Pseudonymisierung:** Mit Zusatzinfo rückführbar (z.B. Patient-ID statt Name)
- **Anonymisierung:** Nicht rückführbar (komplett entfernt)

---

### 11. PROJEKTMANAGEMENT (für betriebliche Projektarbeit)

#### Klassisches Projektmanagement
- **Phasen:** Initiierung, Planung, Durchführung, Abschluss
- **Magisches Dreieck:** Zeit, Kosten, Qualität
- **Gantt-Diagramm** - Zeitplanung
- **Meilensteine** - Wichtige Etappenziele

#### Agile Methoden
- **Scrum:**
  - Sprints (2-4 Wochen)
  - Daily Standup
  - Product Backlog, Sprint Backlog
  - Retrospektive

- **Kanban:**
  - Board mit Spalten (To Do, In Progress, Done)
  - WIP-Limits (Work in Progress)

---

### 12. WIRTSCHAFTS- UND SOZIALKUNDE

#### Arbeitsrecht
- **Arbeitsvertrag** - Rechte und Pflichten
- **Kündigungsfristen:**
  - Probezeit: 2 Wochen
  - Nach 2 Jahren: 1 Monat
  - Nach 5 Jahren: 2 Monate
  - Nach 8 Jahren: 3 Monate
  - Nach 20 Jahren: 7 Monate

- **Abmahnung:** Rüge vor Kündigung (bei Fehlverhalten)
- **Arbeitszeiten:**
  - Max. 8 Stunden/Tag (10 Stunden bei Ausgleich)
  - 11 Stunden Ruhezeit zwischen Arbeitstagen
  - Pausenregelung (6h → 30 Min, 9h → 45 Min)

#### Ausbildung
- **Berufsbildungsgesetz (BBiG)**
- **Ausbildungsvertrag** - Schriftform erforderlich
- **Probezeit:** 1-4 Monate
- **Jugendarbeitsschutzgesetz** - Für U18
- **Überstunden:** Nach Vereinbarung bezahlt oder Freizeitausgleich

#### Sozialversicherung (5 Säulen)
1. **Krankenversicherung** (~14,6% + Zusatzbeitrag)
2. **Pflegeversicherung** (~3%)
3. **Rentenversicherung** (~18,6%)
4. **Arbeitslosenversicherung** (~2,6%)
5. **Unfallversicherung** (nur Arbeitgeber)

**Aufteilung:** Je ~50% Arbeitgeber + Arbeitnehmer (außer UV)

#### Steuern
- **Lohnsteuer** - je nach Steuerklasse
- **Solidaritätszuschlag**
- **Kirchensteuer** (freiwillig)

#### Tarifvertrag & Gewerkschaften
- **Tarifautonomie** - Gewerkschaften + Arbeitgeberverbände verhandeln
- **Tarifvertrag** - Mindestlohn, Urlaub, Arbeitszeiten
- **Betriebsrat** - Mitbestimmung der Arbeitnehmer

#### Betriebsübergang (§ 613a BGB)
- Betrieb wechselt Inhaber
- Arbeitsverhältnisse bleiben bestehen
- Kündigungsschutz für 1 Jahr

---

## 📊 Typische Aufgabenformate

### 1. Multiple Choice
- Kreuzchen-Aufgaben (A/B/C/D)
- Oft nur eine richtige Antwort
- Tipp: Ausschlussprinzip

### 2. Berechnungen
- Subnetting (IP-Bereiche ermitteln)
- RAM/Storage-Bedarf
- USV-Dimensionierung
- Verfügbarkeit (MTBF/MTTR)
- Wirtschaftlichkeit (ROI, Amortisation)

### 3. Szenarien
- Beschreibe ein Netzwerkkonzept für Firma X
- Erstelle ein Backup-Konzept mit RPO/RTO
- Plane Arbeitsplätze für verschiedene Abteilungen
- Firewall-Regelwerk erstellen

### 4. Fehleranalyse
- Server nicht erreichbar - systematisches Troubleshooting
- Netzwerkprobleme - OSI-Schichten abarbeiten
- Sicherheitsvorfall - Sofortmaßnahmen

### 5. Vergleichsaufgaben
- Technologie A vs. B (Tabelle mit Vor-/Nachteilen)
- Beispiel: Thick vs. Thin Provisioning, SSL-VPN vs. IPsec

---

## 🎓 Lernstrategien & Tipps

### Vor dem Test
1. **Strukturiert lernen:**
   - Nutze die vorhandenen Musterprüfungen (du hast 21 Stück!)
   - Mache jede Prüfung unter Zeitdruck (90 Min)
   - Korrigiere und verstehe Fehler

2. **Subnetting üben:**
   - Ist eines der wichtigsten Themen!
   - Täglich 10 Aufgaben rechnen
   - Online-Tools: subnetting.net, subnet-calculator.com

3. **Karteikarten:**
   - Ports auswendig lernen (HTTP 80, HTTPS 443, SSH 22...)
   - OSI-Modell
   - RAID-Level
   - SQL-Befehle

4. **Praxisnähe:**
   - Eigenes Heimlabor (VirtualBox + VMs)
   - Windows Server testen
   - Linux-VM aufsetzen
   - Netzwerke simulieren (GNS3, Packet Tracer)

### Im Test
1. **Zeitmanagement:**
   - Nicht an einer Aufgabe hängenbleiben
   - Schwierige überspringen, später wiederkommen
   - Letzte 10 Minuten: Durchsicht

2. **Berechnungen:**
   - Immer Rechenweg zeigen (Teilpunkte!)
   - Einheiten nicht vergessen (GB, VA, %, Ah...)
   - Plausibilität prüfen (5 TB RAM unrealistisch)

3. **Fachbegriffe:**
   - Korrekte Terminologie verwenden
   - Abkürzungen beim ersten Mal ausschreiben

4. **Skizzen:**
   - Netzwerkdiagramme zeichnen (auch wenn nicht explizit gefordert)
   - Visualisierung hilft beim Verständnis

---

## 📚 Deine vorhandenen Materialien nutzen

Du hast bereits exzellente Ressourcen:

### IHK Musterprüfungen (10-21)
- **Strategie:** Mache eine pro Woche unter Prüfungsbedingungen
- Kontrolliere mit Lösungen
- Notiere Schwachstellen
- Wiederhole schwierige Themen

### FISI_200_Uebungsaufgaben.docx
- Perfekt für tägliches Training
- 10 Aufgaben pro Tag

### FISI_Pruefungskompendium_Komplett.docx
- Theoretisches Nachschlagewerk
- Als Lerngrundlage nutzen

### Lernplan_IT_Systemintegration.docx
- Strukturiere deine Wochen

---

## ⚡ Schnell-Checkliste: Was du SOFORT auswendig wissen musst

### 🔴 Kritisch wichtig (auswendig!)
- [ ] OSI-Modell (alle 7 Schichten)
- [ ] TCP/IP-Modell (4 Schichten)
- [ ] Standard-Ports (HTTP, HTTPS, SSH, FTP, SMTP, DNS, DHCP, RDP, SMB)
- [ ] Private IP-Bereiche (10.x, 172.16-31.x, 192.168.x.x)
- [ ] RAID-Level (0, 1, 5, 6, 10)
- [ ] ACID-Eigenschaften
- [ ] 3-2-1-Backup-Regel
- [ ] RPO vs. RTO
- [ ] DSGVO-Grundsätze
- [ ] Sozialversicherungen (5 Säulen)

### 🟡 Sehr wichtig (verstehen + anwenden können)
- [ ] Subnetting / VLSM
- [ ] VLAN-Konzepte
- [ ] Active Directory (OUs, GPOs)
- [ ] Virtualisierung (VMware HA, vMotion)
- [ ] Firewall-Regeln erstellen
- [ ] VPN-Typen
- [ ] Verfügbarkeitsberechnung (MTBF/MTTR)
- [ ] Troubleshooting-Methodik

### 🟢 Wichtig (Grundverständnis)
- [ ] Linux-Befehle
- [ ] SQL-Grundlagen
- [ ] ITIL (Incident/Problem/Change)
- [ ] Projektmanagement (klassisch vs. agil)
- [ ] Arbeitsrecht (Kündigungsfristen, Pausenregelung)

---

## 🚀 4-Wochen-Crashplan

### Woche 1: Grundlagen festigen
- **Tag 1-2:** Netzwerktechnik (OSI, TCP/IP, Ports)
- **Tag 3-4:** Subnetting intensiv (50+ Aufgaben)
- **Tag 5:** Hardware & Arbeitsplätze
- **Tag 6:** Musterprüfung 5 (90 Min)
- **Tag 7:** Auswertung + Wiederholung Schwachstellen

### Woche 2: Server & Virtualisierung
- **Tag 1-2:** Windows Server, Active Directory, GPOs
- **Tag 3:** Linux-Grundlagen
- **Tag 4:** Virtualisierung (VMware, Hyper-V)
- **Tag 5:** Datenbanken (SQL, ACID)
- **Tag 6:** Musterprüfung 6 (90 Min)
- **Tag 7:** Auswertung

### Woche 3: Sicherheit & Management
- **Tag 1-2:** IT-Sicherheit (Firewall, VPN, Verschlüsselung)
- **Tag 3:** Backup & Disaster Recovery
- **Tag 4:** Monitoring (SNMP, ITIL)
- **Tag 5:** DSGVO & Datenschutz
- **Tag 6:** Musterprüfung 10 (90 Min)
- **Tag 7:** Auswertung

### Woche 4: WiSo & Prüfungssimulation
- **Tag 1:** Arbeitsrecht, Sozialversicherung, Steuern
- **Tag 2:** Musterprüfung 12 (vollständig, alle Teile)
- **Tag 3:** Musterprüfung 16 (vollständig)
- **Tag 4:** Schwachstellen gezielt wiederholen
- **Tag 5:** Musterprüfung 20 (vollständig)
- **Tag 6:** Letzte Wiederholungen, Karteikarten
- **Tag 7:** Ausruhen, früh schlafen!

---

## 🎯 Prüfungstag

### Vorbereitung
- [ ] Ausgeschlafen (8 Stunden!)
- [ ] Ausreichend Wasser trinken
- [ ] Leichtes Frühstück (kein Völlegefühl)
- [ ] Personalausweis/Ausbildungsnachweis mitbringen
- [ ] Mehrere Stifte (schwarz/blau)
- [ ] Taschenrechner (falls erlaubt)

### Während der Prüfung
- [ ] Zuerst komplett durchlesen (Überblick)
- [ ] Einfache Aufgaben zuerst (Selbstvertrauen)
- [ ] Bei Blockade: Nächste Aufgabe (zurückkommen!)
- [ ] Zeitpuffer für Kontrolle (10 Min)
- [ ] Alle Aufgaben versuchen (Teilpunkte!)

---

## 📖 Zusätzliche Online-Ressourcen

### Interaktive Übungen
- **Professor Messer** (YouTube) - CompTIA-Videos (ähnliche Themen)
- **NetworkChuck** (YouTube) - Netzwerktechnik anschaulich
- **CBT Nuggets** - Professionelle IT-Trainings
- **IT-Berufe-Podcast** - Spezifisch für deutsche IHK-Prüfungen

### Tools zum Üben
- **Subnetting:** subnetipv4.com, subnettingpractice.com
- **Cisco Packet Tracer** - Netzwerke simulieren (kostenlos)
- **GNS3** - Erweiterte Netzwerksimulation
- **VirtualBox** - VMs für Server-Übungen (kostenlos)

### Communities
- **fachinformatiker.de** - Forum für Azubis
- **reddit.com/r/de_EDV** - Deutsche IT-Community
- **IHK-Prüfungsaufgaben** - Alte Prüfungen (bei IHK anfragen)

---

## 💡 Abschließende Tipps

### Was Prüfer sehen wollen
✅ **Strukturiertes Denken** - Systematisch vorgehen
✅ **Fachsprache** - Korrekte Begriffe verwenden
✅ **Praxisbezug** - Realistische Lösungen
✅ **Wirtschaftlichkeit** - Kosten-Nutzen beachten
✅ **Sicherheit** - Immer mitdenken (DSGVO, Backup, Firewall)

### Häufige Fehler vermeiden
❌ Keine Einheiten bei Berechnungen
❌ Unrealistische Werte (1 TB RAM für Office-PC)
❌ Sicherheitsaspekte vergessen
❌ Zeitmanagement - zu lange bei einer Aufgabe
❌ Unleserliche Handschrift

---

**Du schaffst das! 💪 Mit den vorhandenen 21 Musterprüfungen bist du bestens ausgestattet. Nutze sie intensiv!**

**Viel Erfolg bei deiner Prüfung zum Fachinformatiker Systemintegration! 🎓**
