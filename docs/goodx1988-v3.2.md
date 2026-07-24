# GoodX1988 v3.2

Correção de encerramento ao abrir a lista de canais.

O crash era `Resources$NotFoundException` no recurso `lb_ic_play`: a tabela de recursos havia sido compactada, mas três referências Smali ainda usavam o ID anterior. As referências foram alinhadas ao ID atual do drawable existente.

Também preserva as otimizações e a proteção `KEEP_SCREEN_ON` da v3.1.
