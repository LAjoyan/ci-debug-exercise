# Fellogg

En rad per fel. Skriv medan du minns hur du gjorde.

| Nr | Vad stod i loggen?                  | Lokalt eller på GitHub? | Hur tog du reda på orsaken? | Hur löste du det? |
|----|--------------------                 |-------------------------|-----------------------------|-------------------|
| 1  | Invalid workflow file               | GitHub                  | Kollade koden och såg att steget var felindenterat| Rättade indenteringen|
| 2  | Unable to find lockfile at `uv.lock`| GitHub  |Läste felmeddelandet som sa att lock-filen saknades och föreslog `uv sync`  | Körde `uv sync` lokalt för att generera `uv.lock` och checkade in filen|
| 3  |  `os` imported but unused  |GitHub| Läste felmeddelandet som sa att `os` imported but unused   | Jag tog bort den raden
|4| unformatted: File would be reformatted | GitHub | Läste loggen som visade en diff på saknade mellanslag | Använde `Ctrl + Shift + F` i editorn för att auto-formatera koden |
| 5 | ModuleNotFoundError: No module named 'numpy' | GitHub | Läste pytest-loggen som klagade på att numpy saknades | Körde `uv add numpy` i terminalen för att installera paketet |

Fortsätt tabellen med fler rader vid behov.
