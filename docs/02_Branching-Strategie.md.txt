# Branching-Strategie

Für dieses Projekt gilt folgende Strategie:

- **main**  
  Enthält stets stabilen, deploybaren Code. Änderungen erfolgen ausschliesslich über Pull Requests.

- **feature/XYZ**  
  Für neue Features wird ein eigener Branch erstellt (z. B. `feature/hauptseite`). 
Nach Fertigstellung und Test werden diese in `main` gemergt.

- **bugfix/XYZ**  
  Bei Fehlerbehebungen wird ein separater Branch angelegt (z. B. `bugfix/login-issue`). 
Auch hier erfolgt der Merge in `main` nach Abschluss der Arbeiten.

- **release/vX.X**  
  Vor einem Release wird ein Release-Branch erstellt, um finale Tests und kleinere Anpassungen vorzunehmen. 
Anschliessend wird der Branch in `main` gemergt und ein Tag gesetzt.

Alle Branches werden über Pull Requests in den `main`-Branch integriert, wobei Code Reviews und automatisierte Tests durchgeführt werden.
