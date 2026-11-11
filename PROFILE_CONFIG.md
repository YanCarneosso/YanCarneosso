# Configuração do perfil

Guia de manutenção do `README.md`. Os comentários HTML no README indicam cada área editável.

**Posicionamento:** AI Engineer (LLMs, RAG, agentes de IA, avaliação e operação), com engenharia de dados e pesquisa como base. Ao incluir conteúdo novo, priorize o que reforça esse posicionamento e mantenha cada afirmação ligada a uma evidência pública (repositório, publicação ou certificado).

## Estrutura do README

| Seção | Conteúdo | Fonte dos dados |
|---|---|---|
| Cabeçalho | Banner, headline, apresentação, contatos e navegação | LinkedIn |
| Sobre | Foco em AI Engineering, atuação atual, formação e resumo em tabela | LinkedIn |
| Como construo sistemas de IA | 5 princípios de engenharia, cada um com link para o projeto que o demonstra | Repositórios |
| Competências | Áreas de AI Engineering, práticas e ferramentas comprovadas nos projetos | Repositórios e LinkedIn |
| Projetos em destaque | 4 cards com mini-banner (repositórios públicos com CI verde) | GitHub |
| Mais projetos | Tabela com os demais repositórios e projetos em desenvolvimento | GitHub |
| Pesquisa e publicações | 3 linhas de pesquisa e lista de publicações por ano | LinkedIn (Publicações) |
| Trajetória | Experiência e formação | LinkedIn |
| Certificações e reconhecimentos | Certificados e menções honrosas | LinkedIn |
| Contribuições | Animação gerada pelo workflow `snake.yml` | GitHub Actions |

## Pendências

- [ ] ORCID: descomentar o badge no cabeçalho e trocar o `href` pela URL pública.
- [ ] Currículo Lattes: descomentar o badge no cabeçalho e trocar o `href` pela URL pública.
- [ ] Coautores e DOI das publicações, quando houver.
- [ ] Links das publicações do XXXV CPG – UFLA (2026), quando os anais forem publicados.
- [ ] Repositório do Vault Mind, quando for público (adicionar o link na tabela "Mais projetos").
- [ ] Corrigir o CI do `fraud-detection-ml` (workflows "Qualidade do código" e "Publicar relatório no GitHub Pages" falhando desde 28/07/2026). Ele saiu dos destaques, mas continua linkado em "Como construo sistemas de IA" e em "Mais projetos".

## Como atualizar

### Novo projeto em destaque

1. Crie um mini-banner em `assets/projects/` com 720 × 260 px, seguindo o padrão dos existentes (fundo em gradiente escuro, rótulo em maiúsculas, título de 34–38 px, ícone à direita a partir de x ≈ 470).
2. Copie um bloco `<td>` da seção "Projetos em destaque" e mantenha a grade com número par de cards.
3. Prefira repositórios públicos com CI passando: quem visita o perfil clica no repositório.

### Nova publicação

Adicione um item no ano correspondente, no formato:

```markdown
- **Título.** *Evento ou periódico*, mês ano. `Área` · [Acessar](URL)
```

Atualize também a contagem de trabalhos acadêmicos na tabela da seção "Sobre".

### Revisão periódica

1. Atualize experiência, certificações e publicações sempre que o LinkedIn mudar.
2. Revise a linha "Última atualização" no rodapé.
3. Valide links e imagens na aba **Preview** do GitHub antes de confirmar o commit.

## Assets

| Arquivo | Uso |
|---|---|
| `assets/banner.svg` | Cabeçalho |
| `assets/dividers/neural-divider.svg` | Separadores entre seções |
| `assets/projects/atlas-wiki.svg`, `delivery-orchestrator.svg`, `mentoria-ml.svg`, `deepseek-harness.svg` | Projetos em destaque |
| `assets/projects/legal-ai.svg`, `defi-automation.svg`, `green-hydrogen.svg` | Linhas de pesquisa |
| `assets/projects/fraud-detection.svg` | Sem uso no momento; volta aos destaques quando o CI do repositório for corrigido |
| `assets/projects/vault-mind.svg`, `data-engineering.svg`, `assets/github-activity.svg` | Sem uso no momento; reservados para quando houver repositório ou demonstração pública |

Ícones de tecnologia vêm do [devicon](https://devicon.dev) via jsDelivr, e os badges de contato, do [shields.io](https://shields.io). O ícone da AWS do devicon não está disponível pelo CDN, por isso a AWS aparece apenas na tabela de competências.

## Animação de contribuições

O workflow `.github/workflows/snake.yml` roda diariamente às 03:23 UTC (e também manualmente) e publica os SVGs claro e escuro na branch `output`. Ele usa apenas o `GITHUB_TOKEN` temporário do GitHub Actions; nenhum token pessoal deve ser criado ou salvo.

## Verificação antes de publicar

- [ ] Nenhum link de placeholder ativo no README.
- [ ] Links profissionais, de repositórios e de publicações abrem corretamente.
- [ ] Banner, mini-banners e ícones aparecem no Preview.
- [ ] A animação de contribuições funciona nos temas claro e escuro.
- [ ] Nenhum dado pessoal sensível foi incluído.
