# Kit de marca WST para apresentações e IA

Arquivos oficiais da Water Services and Technologies (WST) para montar apresentações, organizados para uso por pessoas e por IAs.

## Como usar com uma IA

1. Peça que a IA leia `AGENTS.md` (regras da marca) e `brand.json` (valores técnicos) antes de começar.
2. Disponibilize os arquivos de `assets/` (ou os links brutos do GitHub).
3. Peça o conteúdo da apresentação. Para .pptx, a fonte **Arial Nova** é referenciada pelo nome e precisa estar instalada no computador de quem abrir o arquivo.

Se a IA acessa o GitHub, basta o link do repositório e a frase: "Leia o `AGENTS.md` antes de começar". O Claude Code lê o `CLAUDE.md` (que aponta para o `AGENTS.md`) sozinho ao abrir o repositório. Em outras ferramentas isso não é automático: coloque a frase acima nas instruções do projeto ou no primeiro pedido.

Exemplo de pedido:

> Leia AGENTS.md e brand.json deste repositório e use os arquivos de assets/. Monte uma apresentação sobre [tema], com base em [conteúdo ou link]. Cumpra todas as regras sem exceção. Se precisar quebrar alguma, avise e pergunte antes.

## Estrutura

| Pasta ou arquivo | Conteúdo |
|---|---|
| `AGENTS.md` | Regras consolidadas da marca e dos modelos de slide. `CLAUDE.md` apenas aponta para ele |
| `brand.json` | Cores, gradientes, tipografia, margens e arquivos por tipo de slide |
| `docs/` | Guia Rápido da Marca e Guia de Apresentação com IA (fonte oficial, em PDF) |
| `assets/apresentacao/` | Fundo da capa, fundo da capa de seção, overlay do slide de conteúdo e overlay do slide final (PNG 7681 px e SVG) |
| `assets/logo/` | Logo institucional, branco e escala de cinza |
| `assets/simbolo/` | Símbolo nas mesmas três versões |
| `assets/grafismos/` | Textura topográfica (4 cores) e malha tridimensional (2 versões) |

## Qual arquivo usar em cada slide

| Slide | Arquivo |
|---|---|
| Capa | `assets/apresentacao/fundo-capa.png` sobre a foto |
| Capa de seção | `assets/apresentacao/fundo-capa-de-secao.png` |
| Conteúdo com imagem | `assets/apresentacao/overlay-slide-de-conteudo.png` sobre a foto |
| Conteúdo sem imagem | Fundo branco `#FFFFFF` |
| Página final | `assets/apresentacao/overlay-slide-final.png` sobre a foto |

Os overlays têm uma janela transparente em forma de curva: a foto aparece por ela. Coloque a foto **embaixo** e o overlay **por cima**.

## Observações sobre os arquivos

- Não há SVG da logo na versão institucional, só PNG e PDF. Exporte o SVG a partir do `Logo.ai` original, se precisar.
- O manual prevê só três versões da logo. A versão preta do pacote original não foi incluída aqui.
- Os PDFs em `docs/` têm erros de RGB e links `blob` de commit nos botões de download. Os valores corretos estão em `AGENTS.md` e `brand.json`. Os arquivos de slide estão em `assets/apresentacao/`.
- Os arquivos EPS e AI do pacote original não foram copiados. Guarde-os em outro lugar se forem necessários para impressão.
