<div align="center">

# Caio Medeiros

### Desenvolvedor Full Stack

Construo sistema que negócio pequeno usa todo dia: site que gera contato,<br>
painel que a equipe opera sozinha e banco que guarda o que importa.

[![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/CaeoFranco)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/caiomedeiros123/)

</div>

---

## Sobre

Trabalho full stack do banco ao deploy: modelagem no Postgres, API e regra de negócio no
servidor, interface em React e a publicação com domínio, TLS e pipeline verde no fim.

O que me diferencia não é a lista de tecnologia, é o contexto: quase tudo que construo roda
para cliente real, com gente de verdade cadastrando produto e recebendo contato do outro
lado. Isso muda o padrão de qualidade. Site que cai é venda perdida de alguém, então build
quebrada não vira deploy, migration sem rollback não entra e credencial não mora no
repositório.

Parte dos projetos já está no ar, o resto está em construção. Como são sistemas de cliente,
os repositórios são privados. Abaixo está o que cada um faz, por segmento.

---

## Stack

**Front-end**

![Next.js](https://img.shields.io/badge/Next.js-000000?style=for-the-badge&logo=nextdotjs&logoColor=white)
![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-3178C6?style=for-the-badge&logo=typescript&logoColor=white)
![Tailwind CSS](https://img.shields.io/badge/Tailwind_CSS-06B6D4?style=for-the-badge&logo=tailwindcss&logoColor=white)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)

**Back-end e dados**

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-4169E1?style=for-the-badge&logo=postgresql&logoColor=white)
![Supabase](https://img.shields.io/badge/Supabase-3FCF8E?style=for-the-badge&logo=supabase&logoColor=white)
![SQL](https://img.shields.io/badge/SQL-CC2927?style=for-the-badge&logo=databricks&logoColor=white)

**Qualidade e automação**

![Vitest](https://img.shields.io/badge/Vitest-6E9F18?style=for-the-badge&logo=vitest&logoColor=white)
![Playwright](https://img.shields.io/badge/Playwright-2EAD33?style=for-the-badge&logo=playwright&logoColor=white)
![ESLint](https://img.shields.io/badge/ESLint-4B32C3?style=for-the-badge&logo=eslint&logoColor=white)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-2088FF?style=for-the-badge&logo=githubactions&logoColor=white)

**Infra e deploy**

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Vercel](https://img.shields.io/badge/Vercel-000000?style=for-the-badge&logo=vercel&logoColor=white)
![NGINX](https://img.shields.io/badge/NGINX-009639?style=for-the-badge&logo=nginx&logoColor=white)
![Cloudflare](https://img.shields.io/badge/Cloudflare-F38020?style=for-the-badge&logo=cloudflare&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![Claude Code](https://img.shields.io/badge/Claude_Code-D97757?style=for-the-badge&logo=anthropic&logoColor=white)

---

## O que eu construo

### Revenda de veículos

Vitrine de estoque com busca e página por veículo (fotos, ficha técnica, opcionais, preço),
formulário de contato que cai num painel interno e área administrativa com login onde a
equipe cadastra, edita e remove veículo sem depender de ninguém. Antes do sistema, a vitrine
da loja era o Instagram e o estoque vivia na cabeça do vendedor.

`Next.js` `TypeScript` `Supabase (Postgres, Auth e Storage)` `Tailwind` `Playwright`
&nbsp;&nbsp;·&nbsp;&nbsp; **3 projetos**

### Serviços técnicos e indústria

Site institucional para empresa que vive de indicação e não aparece na busca. O foco é
presença encontrável: SEO local, conteúdo que descreve o serviço com precisão e caminho
curto do visitante até o WhatsApp. Um dos casos substituiu um site de 2017 que ainda
apontava telefone de outro estado.

`Next.js` `TypeScript` `Tailwind` `Resend` `Vercel`
&nbsp;&nbsp;·&nbsp;&nbsp; **3 projetos**

### Saúde e bem-estar

Landing e site de clínica, com apresentação do serviço, prova social e agendamento por
WhatsApp. Projeto pequeno em superfície e exigente em confiança: quem procura clínica decide
pelo que o site transmite nos primeiros segundos.

`Next.js` `TypeScript` `Tailwind` `Docker`
&nbsp;&nbsp;·&nbsp;&nbsp; **2 projetos**

### Comunidade e cultura

Site de comunidade religiosa, com identidade visual própria e produção de conteúdo de
divulgação apoiada por automação. Requisito central era respeitar a linguagem da comunidade
sem cair em estética genérica de template.

`Next.js` `TypeScript` `Tailwind`
&nbsp;&nbsp;·&nbsp;&nbsp; **1 projeto**

### Infraestrutura compartilhada

Supabase self-hosted em Docker Compose atrás de NGINX, com geração de chaves, papéis de
banco por menor privilégio e um gate na frente. Mais scripts em Node que geram proposta
comercial, sincronizam catálogo e auditam padrão de escrita no CI.

`Docker Compose` `NGINX` `PostgreSQL` `Node.js`

---

## Como eu trabalho

- **Pipeline desde o dia zero.** Lint, checagem de tipos, testes e build a cada push e a cada
  pull request. Pipeline vermelho não vira deploy.
- **Teste em camada.** Vitest para unidade, Playwright para o fluxo de ponta a ponta no
  navegador.
- **Decisão registrada.** ADR para escolha de arquitetura e CHANGELOG atualizado a cada
  alteração, com versionamento semântico.
- **Segredo fora do repositório.** Variável de ambiente e secrets manager, nunca credencial
  no código.
- **Rollback antes do deploy.** Migration só entra em produção com volta documentada e
  testada. Rollback de código sem rollback de schema é falsa segurança.
- **O cliente é dono.** Código, domínio, contas e dados ficam no nome dele.

---

## Estudando agora

- Arquitetura de aplicação e padrão de projeto aplicados a sistema que precisa durar
- Postgres a fundo: modelagem, índice, RLS e plano de execução
- Observabilidade: log estruturado, métrica, health check e alerta guiado por SLO
- Infraestrutura self-hosted com Docker, proxy reverso e TLS
- Desenvolvimento assistido por IA com contexto versionado e revisão humana no merge

---

## Contato

**GitHub:** [@CaeoFranco](https://github.com/CaeoFranco)<br>
**LinkedIn:** [Caio Medeiros](https://www.linkedin.com/in/caiomedeiros123/)

Aberto a conversa sobre projeto, colaboração ou boa discussão técnica.
