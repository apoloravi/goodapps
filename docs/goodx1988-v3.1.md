# GoodX1988 v3.1

## Alteracoes

- Marca, splash e launcher atualizados para **GoodX 1988**.
- Painel padrao configurado para `http://multi.painelgood.xyz/`.
- Carregamento de logo e fundo legados desativado para reduzir chamadas e tempo de abertura.
- Recursos nao utilizados removidos e imagens do launcher redimensionadas. O APK caiu de aproximadamente 22 MB para 11 MB.
- Primeiro toque dos itens da lista corrigido para nao depender de dois cliques.
- `FLAG_KEEP_SCREEN_ON` aplicado na tela principal e nos players.
- Services do Kotlin preservados no pacote para evitar falha do dispatcher.

## Gestor App

O painel possui a tela `app_manager.php` (menu **Gestor App**) e o endpoint:

```text
/api/app_config.php?app_id=<ID>&key=<CHAVE>
```

O endpoint devolve JSON sem cache com URL do painel, nome, logo, fundo, politica de tela ativa e a flag de VPN L2TP. A VPN permanece desativada (`vpn_l2tp_enabled=false`) até existir um desenho e credenciais próprios para essa funcionalidade.

## Validacao

- Assinaturas v1, v2 e v3 verificadas com `apksigner`.
- Instalacao ADB concluida no pacote `com.example.unitv`.
- Inicializacao observada sem crash fatal.

## Seguranca

Nao inserir usuario, senha de painel ou senha SSH no APK, no Git ou em URLs. O endpoint usa uma chave por aplicativo. Rotacione a senha de root usada durante a manutencao.
