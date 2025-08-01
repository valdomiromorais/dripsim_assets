## Painel de Controle do DripSim

[[README ATUAL]]
[[RELATÓRIO ATUAL]]
[[COMANDOS_AIA]]

### Notas sobre Assets e Memórias
```dataview
TABLE file.name AS "Nota", file.ctime AS "Criado em", file.mtime AS "Atualizado em"
FROM "docs/relatorios/dripsim_vault"
WHERE contains(file.name, "Vinhedo") OR contains(file.name, "Canos") OR contains(file.name, "Memórias")
SORT file.ctime DESC