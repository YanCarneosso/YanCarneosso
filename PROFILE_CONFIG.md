# Configuração do perfil

Use esta checklist antes de publicar. No `README.md`, pesquise por `SEU_` para localizar todos os campos pendentes.

## Dados e links

- [x] Username do GitHub configurado como `YanCarneosso` (inclusive nas URLs da animação).
- [x] LinkedIn configurado como `yan-costa-carneosso-b1343721b`.
- [x] E-mail configurado como `yancarneosso@gmail.com`.
- [ ] `SEU_ORCID` → URL pública do ORCID.
- [ ] `SEU_LATTES` → URL pública do Currículo Lattes.
- [ ] `SEU_PORTFOLIO` → URL do portfólio.
- [ ] Adicionar links institucionais da UNILA/UFLA se desejar.

## Projetos

- [ ] `SEU_REPOSITORIO_VAULT_MIND` e `SEU_VAULT_MIND_DEMO`.
- [ ] `SEU_REPOSITORIO_LEGAL_AI` e `SEU_LEGAL_AI_ARTIGO`.
- [ ] `SEU_REPOSITORIO_DEFI` e `SEU_DEFI_ARTIGO_DEMO`.
- [x] Repositório de fraudes: `YanCarneosso/fraud-detection-ml`.
- [ ] `SEU_FRAUDES_DEMO`.
- [ ] `SEU_REPOSITORIO_HIDROGENIO` e `SEU_HIDROGENIO_ARTIGO`.
- [ ] `SEU_REPOSITORIO_DADOS` e `SEU_DADOS_DEMO`.

Se algum material ainda não for público, substitua o link por texto simples como `Repositório privado` ou `Documentação em preparação`. Não publique um placeholder como se fosse uma URL final.

## Manutenção

1. Edite textos e links diretamente no `README.md`; os comentários HTML indicam cada área.
2. Atualize `assets/banner.svg` e os mini-banners somente se o nome ou a identidade visual mudar.
3. Para um novo projeto, duplique uma célula da tabela e crie um SVG em `assets/projects/`.
4. Revise a linha `Última atualização` no rodapé após mudanças importantes.
5. Valide os links na aba **Preview** do GitHub antes de confirmar o commit.

## Ativação da animação de contribuições

1. Publique este repositório com o mesmo nome do seu username do GitHub.
2. Em **Settings → Actions → General → Workflow permissions**, permita leitura e escrita.
3. Abra **Actions → Generate contribution snake → Run workflow**.
4. Confirme que a branch `output` e os dois SVGs foram criados.
5. O workflow roda diariamente às 03:23 UTC e também permite execução manual.

O workflow usa apenas o `GITHUB_TOKEN` temporário fornecido pelo GitHub Actions. Nenhum token pessoal deve ser criado ou salvo.

## Verificação final

- [ ] Todos os placeholders `SEU_` foram removidos ou explicados.
- [ ] Links profissionais abrem corretamente.
- [ ] Links de repositórios, artigos e demonstrações estão públicos.
- [ ] Banner e seis mini-banners aparecem no preview.
- [ ] Cards de estatísticas mostram o username correto.
- [ ] A animação funciona nos temas claro e escuro.
- [ ] Nenhum dado pessoal sensível foi incluído.
