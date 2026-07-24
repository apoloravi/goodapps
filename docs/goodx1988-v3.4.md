# GoodX1988 v3.4

Primeira integração com o Gestor App remoto.

- Consulta `app_config.php` por nome do aplicativo e chave própria no início do login.
- Usa o `panel_url` publicado no painel quando a resposta é válida.
- Mantém `multi.painelgood.xyz` como fallback offline.
- O painel inicializa o cadastro GoodX1988 e permite múltiplos aplicativos no mesmo gestor.

As próximas propriedades (logo, fundo e flags adicionais) podem ser aplicadas pelo cliente remoto sem alterar o contrato do endpoint.
