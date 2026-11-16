# Pop Granja | Ferrati

Código completo da versão atual do site, com a identidade Ferrati.

## Arquivos

- `public/index.html`: página completa com HTML, CSS, JavaScript, animações, formulário de visita, galeria.
- `public/assets/`: imagens e plantas originais do empreendimento.
- `vercel.json`: configuração para servir o site estático na Vercel.
- `.gitignore`: arquivos locais que não precisam ir para o GitHub.

O projeto usa HTML, CSS e JavaScript puros. Não é necessário instalar dependências, executar build ou configurar variáveis de ambiente.

## Publicar pelo GitHub e Vercel

1. Extraia o ZIP.
2. Crie um repositório no GitHub.
3. Envie o conteúdo desta pasta para a raiz do repositório: a pasta `public`, o arquivo `vercel.json` e os demais arquivos. Não envie apenas o ZIP.
4. Na Vercel, use **Add New → Project**, selecione o repositório e importe.
5. Confira as configurações abaixo e clique em **Deploy**.

| Configuração | Valor |
| --- | --- |
| Framework Preset | Other |
| Root Directory | Raiz do repositório (`./`) |
| Build Command | Vazio / sem comando; ative Override se necessário |
| Output Directory | `public` |
| Install Command | Padrão; não há dependências |
| Environment Variables | Nenhuma |

A configuração principal já está no arquivo `vercel.json`.

## Abrir localmente

Você pode abrir `public/index.html` diretamente no navegador. Para servir por HTTP, com Python instalado, execute na pasta do projeto:

```bash
python -m http.server 8000 --directory public
```

Depois acesse `http://localhost:8000`.

## Editar

Abra `public/index.html` em um editor de texto ou no VS Code. O CSS fica no bloco `<style>` e o JavaScript no bloco `<script>`.

- Nome atual: Ferrati.
- WhatsApp: (11) 94627-8609. Procure `5511946278609` para alterar os links e o texto visível para alterar a apresentação do número.
- Fotos e plantas estão em `public/assets/`, preservando os arquivos originais da versão atual.
- As fontes Archivo e Space Mono são carregadas do Google Fonts, com fontes alternativas no CSS.
- O formulário organiza os dados preenchidos e abre uma conversa no WhatsApp. A confirmação da visita é feita pelo consultor.

## Endereço do site

O endereço antigo do ChatGPT foi removido das tags `canonical` e `og:url` desta cópia para publicação independente. Após publicar, você pode adicionar essas tags com o seu domínio definitivo no `<head>`.

## Referências da configuração

- https://vercel.com/docs/builds/configure-a-build
- https://vercel.com/docs/project-configuration/vercel-json

Este pacote não altera a versão hospedada anteriormente.
