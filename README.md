# Vitrine – Site AXIS EVS (Site 2)

Site vitrine público da **AXIS EVS** — espaço de nutrição funcional e acompanhamento personalizado.

## Páginas

| Arquivo | Descrição |
|---|---|
| `index.html` | Página inicial (hero, sobre, cardápio, programas, contato) |
| `cardapio.html` | Listagem completa do cardápio com filtros por categoria |
| `programas.html` | Programas de acompanhamento disponíveis |

## Stack

| Tecnologia | Uso |
|---|---|
| HTML + Tailwind CSS (CDN) | Interface visual responsiva |
| JavaScript (ES Modules) | Lógica dinâmica do frontend |
| Vite | Bundler / build tool |
| Supabase | Backend: banco de dados (leitura pública) |

## Hospedagem

Este repositório contém o **build estático de produção** gerado pelo Vite.  
O arquivo de entrada principal é `index.html` na raiz.

### Como publicar no GitHub Pages

1. Faça o upload/push dos arquivos desta pasta para um repositório GitHub
2. Vá em **Settings → Pages**
3. Em *Source*, selecione **Deploy from a branch** → branch `main` → pasta `/ (root)`
4. Clique em **Save** — seu site estará disponível em:  
   `https://<seu-usuario>.github.io/<nome-do-repositorio>/`

## Conteúdo Dinâmico

O conteúdo (cardápio, programas, textos da home) é carregado automaticamente do **Supabase** via chave pública `anon`.  
As imagens personalizadas (logo, fotos dos produtos) também são servidas via Supabase Storage ou embutidas no bundle.

> ⚠️ Esta é a vitrine **somente leitura**. Para gerenciar o conteúdo, acesse o painel Admin (site1).
