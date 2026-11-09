# Costalog · Controle de Cartões Corporativos

Portal interno para registro de compras realizadas com cartões corporativos e posterior registro dos lançamentos fiscais/contábeis.

## Módulos
- **Painel:** indicadores por período, cartão, estabelecimento e status de lançamento.
- **Registro de compras:** cadastro de cartão, local, data e múltiplos produtos; condições de parcelamento e juros independentes por item.
- **Registro de lançamentos:** fila de compras pendentes, formulário de lançamento ERP, detalhamento por centro de custo e histórico.
- **Cartões corporativos:** cadastro, edição, ativação/desativação e exclusão de cartões.

## Publicação
O projeto é estático e pode ser publicado pelo GitHub Pages. Em **Settings → Pages**, selecione a branch `main` e a pasta `/ (root)`.

## Armazenamento e integração
Nesta primeira versão, os registros são persistidos no `localStorage` do navegador. Isso significa que os dados ficam disponíveis no mesmo navegador/dispositivo e não são compartilhados automaticamente entre colaboradores.

A consulta ao ERP é somente um ponto de extensão demonstrativo: nenhum sistema externo é consultado. Para produção multiusuário, implemente API autenticada, banco de dados centralizado, controle de acesso e integração ERP segura no servidor. Nunca coloque tokens ou senhas no JavaScript público.

## Arquivos
- `index.html`: estrutura da aplicação.
- `css/style.css`: identidade visual Costalog e layout responsivo.
- `js/script.js`: regras de negócio e persistência local.
- `assets/`: logotipos oficiais Costalog.
