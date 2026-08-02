# /shake-the-model

Komenda Claude Code, która sprawdza rozszerzalność modelu wzdłuż jednej metryki biznesowej:
z opisu biznesu (bez architektury) generuje prawdopodobne przyszłe wymagania, a potem liczy,
ile modułów każde z nich zmusza do zmiany.

## Instalacja

1. Skopiuj `commands/` i `agents/` do `.claude/` swojego projektu (albo do `~/.claude/`).
2. Skopiuj skille, z których korzysta komenda, do `~/.claude/skills/`:
   - `business-brief` — opis biznesu bez śladów rozwiązania,
   - `competitor-scan` — zestawienie tego, co oferuje konkurencja,
   - `change-impact` — ocena zasięgu zmiany dla każdego wymagania.

## Użycie

```
/shake-the-model path/to/context-map.md "czas do złożenia oferty" 8
```
