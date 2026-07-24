# GoodX1988 v3.3

Corrige o bloqueio automático da tela durante a reprodução.

- Reaplica `FLAG_KEEP_SCREEN_ON` em cada `onResume` dos players de TV, filmes e séries.
- Marca a janela raiz com `setKeepScreenOn(true)` para sobreviver a pausa/retomada do Android.
- Mantém a correção de recursos e o desempenho da v3.2.
