# Ensalamento UniBrasil

Sistema web para organizar, publicar e consultar o ensalamento (alocação de salas e horários) de uma instituição de ensino superior.

Projeto 1 da disciplina **Prática Profissional em Desenvolvimento Web — Engenharia de Software** (UniBrasil). Trabalho acadêmico, não é uma publicação institucional oficial da universidade.

## Stack

- **Front-end**: HTML, CSS e JavaScript puro, sem framework de aplicação. Base visual do painel administrativo: kit de UI [Light Bootstrap Dashboard](https://github.com/creativetimofficial/light-bootstrap-dashboard) (Creative Tim), reaproveitando apenas os componentes usados nas telas do projeto.
- **Núcleo / API**: Node.js, publicado em contêiner Docker.
- **Banco de dados**: PostgreSQL gerenciado (Supabase), também usado para autenticação federada (Google / Microsoft).

## Publicação

- Front-end: GitHub Pages (branch `main`, raiz do repositório).
- API: contêiner Docker publicado no Render.
- Banco: Supabase.

> Endereço do ambiente em execução: *a preencher assim que a primeira versão for publicada.*

## Como rodar localmente

- **Front-end**: abra os arquivos `.html` diretamente no navegador, ou sirva a pasta com qualquer servidor estático (ex.: extensão "Live Server" do VS Code). Não depende de instalação nenhuma.
- **API**: instruções de build e execução via Docker serão detalhadas aqui assim que a API existir (semana 1–2 do cronograma do projeto).

## Licença

Este projeto usa licença **MIT** — ver [LICENSE](./LICENSE).

**Justificativa:** MIT foi escolhida por ser a licença mais permissiva e simples entre as opções usuais. Ela permite que qualquer pessoa use, copie, modifique e redistribua o código — inclusive comercialmente — desde que mantenha o aviso de copyright e o texto da licença; não há garantia sobre o software. Diferente de licenças copyleft como a GPL, ela não obriga que projetos derivados também sejam abertos. Como este é um projeto acadêmico público, cujo propósito inclui ser inspecionado e eventualmente estudado por outras pessoas, uma licença permissiva e sem restrições de redistribuição fez mais sentido do que uma copyleft ou proprietária.

## Equipe

| Nome | Matrícula | Papel no projeto | Acesso no repositório |
|---|---|---|---|
| Guilherme Tyszkouski | 2025207312 | Infraestrutura, banco de dados e autenticação | Administrador — commit direto na `main` |
| João Pedro Sehnem Scheuer | 2026108288 | Front-end e experiência de uso | Colaborador — contribui via *pull request* |
| Paulo Cézar Mendonça Molena | 2026108305 | API e núcleo de regras de alocação | Colaborador — contribui via *pull request* |

## Divisão de tarefas

Para manter a distribuição de trabalho equilibrada — e rastreável por commits, *pull requests* e revisões, como exige a disciplina — cada integrante tem uma frente principal:

- **Guilherme Tyszkouski**: núcleo de regras (RB-01 a RB-12) e heurística de alocação, endpoints da API, integração front-end ↔ back-end (autenticação federada, chamadas autenticadas, contrato de dados), infraestrutura (Supabase, Docker, Render) e revisão/*merge* dos *pull requests*.
- **João Pedro Sehnem Scheuer**: front-end das telas de Administrador e Coordenador (painel de alocação, conflitos e pendências, formulário de necessidades da turma).
- **Paulo Cézar Mendonça Molena**: front-end das telas de Aluno e Professor (consulta do ensalamento, agenda, localização de sala), responsividade e acessibilidade gerais.

A documentação acadêmica (este README, a área "sobre" publicada no site e o memorial descritivo) é responsabilidade compartilhada dos três, revisada em conjunto antes de cada publicação. Combinado do grupo: mesmo o administrador tendo permissão de commit direto na `main`, todas as contribuições — inclusive as dele — passam por *pull request*, para manter o registro de participação de todos e permitir revisão cruzada do núcleo antes da prova de autoria.

## Status

Projeto em desenvolvimento — este README será expandido conforme cada parte for implementada.
