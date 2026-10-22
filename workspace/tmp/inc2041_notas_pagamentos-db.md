## pagamentos-db — evidências
- conexoes_ativas: 10
- conexoes_max_pool: 10 vs baseline 50
- espera_por_conexao_p95_ms: 3100
- cpu_pct: 23
- queries_lentas_por_min: 2
- ultimo_deploy: config v2.14.0 em 2026-10-12 17:55 (refatoração de variáveis de ambiente do pool)

### Logs literais
- 2026-10-12T17:55:00Z INFO  deploy config v2.14.0 aplicado por pipeline infra-config (autor: bot-refactor-env)
- 2026-10-12T17:55:04Z INFO  pgbouncer restart: pool_mode=transaction default_pool_size=10 (antes: 50) origem=DB_POOL_SIZE
- 2026-10-12T17:55:05Z WARN  pgbouncer DB_POOL_MAX ausente; usando default_pool_size como limite
- 2026-10-12T17:58:30Z WARN  pgbouncer cl_waiting=37 sv_active=10 sv_idle=0
- 2026-10-12T18:05:00Z WARN  pgbouncer cl_waiting=112 sv_active=10 sv_idle=0
- 2026-10-12T18:40:00Z WARN  pgbouncer cl_waiting=98 sv_active=10 sv_idle=0