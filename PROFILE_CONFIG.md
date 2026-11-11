# Configuração do perfil

Guia de manutenção do `README.md`. Os comentários HTML no README indicam cada área editável.

**Posicionamento:** AI Engineer (LLMs, RAG, agentes de IA, avaliação e operação), com engenharia de dados e pesquisa como base. Ao incluir conteúdo novo, priorize o que reforça esse posicionamento e mantenha cada afirmação ligada a uma evidência pública (repositório, publicação ou certificado).

## Estrutura do README

| Seção | Conteúdo | Fonte dos dados |
|---|---|---|
| Cabeçalho | Nome, papel, áreas e formação (imagem), seguidos de links | LinkedIn |
| Sobre | Resumo profissional em dois parágrafos | LinkedIn |
| Faixa de métricas | Projetos de IA com CI, testes, ADRs e trabalhos acadêmicos | Repositórios e LinkedIn |
| Projetos em destaque | 4 cards com capa, descrição, stack e link | GitHub |
| Mais projetos | Demais repositórios e projetos em desenvolvimento | GitHub |
| Como construo sistemas de IA | 5 princípios, cada um com link para o projeto que o demonstra | Repositórios |
| Competências | Áreas de AI Engineering, práticas e ferramentas | Repositórios e LinkedIn |
| Pesquisa e publicações | Linhas de pesquisa e lista de publicações por ano | LinkedIn (Publicações) |
| Trajetória | Experiência, formação e idiomas | LinkedIn |
| Certificações e reconhecimentos | Certificados e menções honrosas | LinkedIn |

## Identidade visual

As imagens em `assets/brand/` e `assets/projects/` são geradas pelo kit em `identidade-visual/` (fora deste repositório), com versões `-light.svg` e `-dark.svg`. Não edite os SVGs à mão: altere `generate.py` e gere novamente. Princípios, cores e tipografia estão no `README.md` do kit.

Cada imagem entra no README com `<picture>`, para acompanhar o tema de quem visita:

```html
<picture>
  <source media="(prefers-color-scheme: dark)" srcset="./assets/projects/exemplo-dark.svg">
  <img src="./assets/projects/exemplo-light.svg" width="100%" alt="Descrição com os mesmos números do card.">
</picture>
```

## Pendências

- [ ] ORCID e Currículo Lattes: adicionar os links na linha de links abaixo do cabeçalho.
- [ ] Coautores e DOI das publicações, quando houver.
- [ ] Links das publicações do XXXV CPG – UFLA (2026), quando os anais forem publicados.
- [ ] Repositório do Vault Mind, quando for público.
- [ ] Workflow `snake.yml`: a animação de contribuições saiu do README; desative o workflow se não for mais usar.

## Como atualizar

### Novo projeto em destaque

1. Adicione o projeto em `PROJECTS` no `identidade-visual/generate.py` e gere as capas.
2. Copie um bloco `<td>` da seção "Projetos em destaque" e mantenha a grade com número par de cards.
3. Prefira repositórios públicos com CI passando: quem visita o perfil clica no repositório.
4. Atualize a faixa de métricas (`METRICS`) se os totais mudarem.

### Nova publicação

Adicione um item no ano correspondente, no formato:

```markdown
- **Título.** *Evento ou periódico*, mês ano. `Área` · [Acessar](URL)
```

Atualize também a contagem em `METRICS` e gere as imagens novamente.

### Revisão periódica

1. Atualize experiência, certificações e publicações sempre que o LinkedIn mudar.
2. Revise a data no rodapé.
3. Valide links e imagens na aba **Preview** do GitHub, nos temas claro e escuro, antes de confirmar o commit.

## Verificação antes de publicar

- [ ] Nenhum link de placeholder ativo no README.
- [ ] Links profissionais, de repositórios e de publicações abrem corretamente.
- [ ] Imagens aparecem nos temas claro e escuro.
- [ ] Números dos cards e da faixa de métricas conferem com os repositórios.
- [ ] Nenhum dado pessoal sensível foi incluído.
