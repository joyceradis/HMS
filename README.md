# HMS · Estação Clínica de Pronto-Socorro

**Protótipo de workflow clínico para reduzir fricção documental no atendimento de urgência.**

> **English:** Emergency-department workflow prototype focused on reducing documentation friction and unnecessary navigation.

[**Abrir demonstração**](https://joyceradis.github.io/HMS/)

## O que este repositório demonstra

| Competência | Evidência no projeto |
| --- | --- |
| Product discovery | problema observado no pronto-socorro transformado em hipótese de interface e fluxo |
| Prototipação clínica | estação navegável para apresentação, documentação, conduta, reavaliação e destino |
| Lógica client-side | JavaScript para estado de navegação, cenários e interação contextual |
| UX sob restrição | desenho orientado a rapidez, previsibilidade e redução de redigitação |
| Evolução de produto | decisões deste protótipo preservadas e posteriormente aprofundadas no Zera PS |

**Portfolio signal:** clinical UX · workflow prototyping · JavaScript · product iteration · emergency-care domain knowledge

O HMS é um projeto de interface para pronto-socorro de Clínica Médica. Foi criado a partir de um problema operacional concreto: em ambientes de alto volume, o médico precisa registrar, consultar e reutilizar informação clínica com velocidade sem transformar o atendimento em uma sequência de telas e redigitação.

## Problema de produto

A documentação de emergência tende a fragmentar o mesmo atendimento entre história, exame, conduta, resultados, reavaliação e destino. O HMS explora uma estação única que aproxima essas etapas.

```text
ENTRADA
  ↓
APRESENTAÇÃO CLÍNICA
  ↓
DOCUMENTAÇÃO ESTRUTURADA
  ↓
CONDUTA / PENDÊNCIAS
  ↓
REAVALIAÇÃO
  ↓
DESTINO
```

## Objetivos

- reduzir cliques e navegação desnecessária;
- manter informação clínica relevante visível durante o atendimento;
- organizar ferramentas por contexto;
- preservar continuidade entre avaliação inicial e reavaliação;
- oferecer uma interface responsiva, legível e utilizável sob pressão;
- permitir expansão incremental sem reconstruir o sistema a cada nova função.

## Estado atual

O repositório contém uma Home e uma **Estação Clínica** navegável, com interface web estática e lógica em JavaScript. A arquitetura atual funciona como protótipo de produto e laboratório de UX clínica.

Arquivos centrais:

```text
HMS/
├── index.html          # Home
├── estação.html        # estação clínica
├── estação.js          # lógica de interação e cenários
├── css/
│   └── styles.css
├── styles.css
└── README.md
```

## Princípios de UX clínica

**Velocidade não pode eliminar revisão.** Atalhos devem reduzir trabalho mecânico, não confirmação médica.

**Uma informação, múltiplos usos.** Dados já registrados devem poder alimentar etapas posteriores sem redigitação desnecessária.

**Contexto antes de ferramenta.** Calculadoras, protocolos e campos devem aparecer quando forem pertinentes ao fluxo.

**Interface previsível.** Em emergência, consistência de navegação e hierarquia visual são requisitos funcionais.

## Tecnologia

- HTML5;
- CSS3;
- JavaScript;
- arquitetura client-side;
- compatível com publicação estática.

## Executar localmente

```bash
python3 -m http.server 8000
```

Depois acesse `http://localhost:8000`.

## Relação com outros projetos

O HMS representa uma etapa anterior da exploração de workflow clínico que posteriormente ganhou uma arquitetura documental e temporal mais explícita no **Zera PS**. Os repositórios são mantidos separadamente para preservar decisões, experimentos de interface e evolução do produto.

## Status

**Protótipo em desenvolvimento.** Não é sistema assistencial homologado e não deve ser utilizado como fonte autônoma de decisão clínica.

## Autoria

Projeto idealizado e desenvolvido por **Dra. Joyce Radis**, médica com atuação em pronto-socorro, a partir de necessidades observadas no fluxo real de atendimento.
