## checkout-api — evidências
- latencia_p95_ms: 4200 vs baseline 380
- taxa_erro_pct: 7.4 vs baseline 0.3
- cpu_pct: 41
- requisicoes_por_seg: 950
- ultimo_deploy: v3.8.1 em 2026-10-12 14:10 (mudança só de layout de e-mail)

### Logs literais
- 2026-10-12T17:57:30Z WARN  checkout-api pod=checkout-5e2a rid=b07 db.acquire slow wait=1450ms pool=pagamentos
- 2026-10-12T17:58:12Z WARN  checkout-api pod=checkout-7f9c rid=b11 db.acquire slow wait=2210ms pool=pagamentos
- 2026-10-12T18:01:45Z ERROR checkout-api pod=checkout-2b1d rid=b38 PoolTimeout: could not acquire connection from pool 'pagamentos' within 3000ms
- 2026-10-12T18:01:46Z ERROR checkout-api pod=checkout-2b1d rid=b38 POST /checkout 503 3012ms
- 2026-10-12T18:05:09Z ERROR checkout-api pod=checkout-9a0c rid=c04 PoolTimeout: could not acquire connection from pool 'pagamentos' within 3000ms
- 2026-10-12T18:05:10Z ERROR checkout-api pod=checkout-9a0c rid=c04 POST /checkout 503 3008ms
- 2026-10-12T18:12:33Z WARN  checkout-api pod=checkout-7f9c rid=c77 db.acquire slow wait=2890ms pool=pagamentos
- 2026-10-12T18:31:48Z ERROR checkout-api pod=checkout-5e2a rid=d90 PoolTimeout: could not acquire connection from pool 'pagamentos' within 3000ms