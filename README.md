**Repositório organizacional — `.github`**

**Propósito**
- Este repositório centraliza arquivos de governança e configuração que são compartilhados por todos os repositórios da organização *Sala de Situação — UNB*. Ele serve para:
	- Fornecer templates de issue/PR e arquivos de comunidade (CODE_OF_CONDUCT, CONTRIBUTING, SECURITY).
	- Armazenar workflows do GitHub Actions reutilizáveis e configurações organizacionais (ex.: `dependabot.yml`).
	- Definir `CODEOWNERS` e políticas padrão para repositórios da organização.

**O que contém (exemplos comuns)**
- `.github/ISSUE_TEMPLATE/` — templates de issue
- `.github/pull_request_template.md` — template de PR
- `.github/workflows/` — workflows de CI/CD compartilhados
- `CODEOWNERS` — responsáveis por diretórios/arquivos
- `CONTRIBUTING.md` — guia de contribuição organizacional
- `SECURITY.md` — política de segurança e disclosure
- `CODE_OF_CONDUCT.md` — conduta da comunidade
- `dependabot.yml` — configuração do Dependabot

**Como usar este repositório**
- Para manter consistência, os mantenedores dos repositórios individuais devem:
	1. Habilitar templates e arquivos padrão nas configurações do repositório (Settings → Features → Community health) quando necessário.
	2. Copiar ou referenciar templates deste repositório ao criar novos repositórios ou ao atualizar existentes.
	3. Reutilizar workflows do diretório `.github/workflows/` colocando um arquivo `workflow` que execute ou importe os templates compartilhados.

**Fluxo para alterar templates / workflows**
- Abra uma issue neste repositório para discutir mudanças de impacto.
- Submeta uma Pull Request com as alterações propostas. Marque os `CODEOWNERS` apropriados para revisão.
- Teste alterações em um repositório piloto antes de aplicar em massa (usar repositório temporário para validar Actions).

**Boas práticas**
- Mantenha templates claros e genéricos para minimizar ajustes por repositório.
- Evite colocar segredos neste repositório.
- Documente mudanças relevantes no histórico da PR para que times consumidores saibam como migrar.

**Governança e responsáveis**
- Time responsável: *Sala de Situação — UNB* (substituir por equipe GitHub/owners reais).
- Para solicitações de suporte ou dúvidas, abra uma issue ou envie email para o time de governança.

---

Se quiser, posso também:
- adicionar templates de `ISSUE_TEMPLATE` e `PULL_REQUEST_TEMPLATE` prontos;
- criar um `CONTRIBUTING.md` mais detalhado;
- adicionar exemplos de `workflow` reutilizáveis no `.github/workflows/`.
