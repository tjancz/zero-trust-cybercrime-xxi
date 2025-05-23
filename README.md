# Zero Trust Open Source Lab

Laboratorium praktyczne: Architektura Zero Trust z wykorzystaniem darmowych narzędzi EDR, SIEM i SOAR  
**Konferencja:** Przestępczość Teleinformatyczna XXI, 16-18 czerwca 2025

---

## Opis

Repozytorium zawiera materiały konferencyjne oraz przykładowe pliki do samodzielnego uruchomienia laboratorium Zero Trust na bazie darmowych rozwiązań open source:

- **Wazuh** (SIEM/EDR)
- **Osquery** (monitoring endpointów)
- **Velociraptor** (forensics/IR)
- **Shuffle** (SOAR)
- **TheHive + Cortex** (zarządzanie incydentami)

Zestaw umożliwia symulację detekcji, automatycznej reakcji i prowadzenia analiz śledczych w środowisku testowym.

---

## Zawartość repozytorium
zero-trust-open-source-lab/
├── docker-compose.yml
├── osquery.conf
├── velociraptor-client-example.yaml
├── playbooks/
│ └── example-playbook.yaml
├── attack-scenarios/
│ └── scenario1.md
├── prezentacja.pdf / prezentacja.pptx
├── docs/
│ └── endpoint-setup.md
└── README.md


---

## Szybki start

1. **Zainstaluj Docker Desktop dla Windows:**  

   https://www.docker.com/products/docker-desktop/

2. **Sklonuj repozytorium:**

git clone https://github.com/TwojNick/zero-trust-open-source-lab.git
cd zero-trust-open-source-lab

3. **Uruchom środowisko:**

docker-compose up -d


4. **Dostęp do narzędzi:**
 - Wazuh/Kibana: http://localhost:5601
 - TheHive: http://localhost:9000
 - Cortex: http://localhost:9001
 - Shuffle: http://localhost:3001

5. **Instalacja agentów na Windows**:  
Szczegóły znajdziesz w `docs/endpoint-setup.md`.

---

## Licencja

- Kod źródłowy: [GNU GPLv3](https://www.gnu.org/licenses/gpl-3.0.html)
- Dokumentacja i grafiki: [Creative Commons Attribution-NonCommercial 4.0](https://creativecommons.org/licenses/by-nc/4.0/)

Jeśli chcesz wykorzystać materiały komercyjnie – skontaktuj się z autorem.

---

## Kontakt

Prezentacja: Tomasz Janczewski  
Konferencja: Przestępczość Teleinformatyczna XXI (16-18 czerwca 2025)  
Email: tomasz@janczewski.it

---

## Więcej

W katalogu `attack-scenarios/` znajdziesz scenariusze do testowania reakcji Zero Trust.  
Prezentacja oraz grafiki znajdują się w katalogu `presentations/`.

