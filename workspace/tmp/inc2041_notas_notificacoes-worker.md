## notificacoes-worker — evidências
- mensagens_pendentes: 1340 vs baseline 120
- taxa_erro_pct: 0.4
- consumidores_ativos: 4
- ultimo_deploy: v1.22.0 em 2026-10-05 10:00

### Linha do tempo
- 2026-10-12T17:50:00Z INFO  notificacoes-worker consumidores=4 pendentes=118
- 2026-10-12T18:05:00Z INFO  notificacoes-worker consumidores=4 pendentes=410 duplicadas_detectadas=63
- 2026-10-12T18:20:00Z INFO  notificacoes-worker consumidores=4 pendentes=870 duplicadas_detectadas=201
- 2026-10-12T18:40:00Z INFO  notificacoes-worker consumidores=4 pendentes=1340 duplicadas_detectadas=388 erros=0.4%

### Observações
- Não houve ERROR/WARN nos logs filtrados.
- O aumento de pendentes e duplicadas é compatível com efeito colateral de retries da API produtora.