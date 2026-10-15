# Validação UX com Persona Sintética by Bruna Fonseca

Skill de avaliação exploratória de protótipos web usando uma **persona sintética descrita em arquivo `.md`**. O agente navega pelo protótipo, registra evidências e aplica o Framework de Feedback.

**Autoria:** Bruna Fonseca | b-a.BA Educação Corporativa | D² [do Discovery ao Delivery]

## O que faz

1. Lê as características, necessidades e limitações da persona.
2. Acessa uma URL pública e percorre jornadas do protótipo com uma ferramenta real de navegador.
3. Registra ações, telas, resultados observados e fluxos não testados.
4. Interpreta descobertas pela perspectiva da persona, separando observações de hipóteses.
5. Organiza o **Framework de Feedback**: o que funciona, melhorias, dúvidas e novas ideias.
6. Entrega um relatório `.md`, um quadrante visual (PNG quando a ferramenta permitir) e oportunidades priorizadas.

> Esta é uma avaliação sintética de usabilidade, não substitui testes com usuários reais.

## Entradas necessárias

- Arquivo `persona.md` contendo o perfil da persona.
- URL pública do protótipo.

## Arquivos da Skill

```text
validar-prototipo-persona/
├── SKILL.md
├── agents/
│   └── openai.yaml
└── references/
    └── relatorio-template.md
```

## Instalação para VS Code / Codex

1. Clone o repositório em que estes arquivos forem publicados.
2. Copie a pasta `validar-prototipo-persona` para `.agents/skills/` no seu projeto Codex.
3. Abra o projeto no VS Code com um agente compatível e ferramentas de navegador habilitadas.
4. Disponibilize a persona `.md` e informe a URL do protótipo.

O VS Code pode oferecer ferramentas de navegador integradas para agentes compatíveis. No Claude Code, uma alternativa é configurar Playwright MCP seguindo a [documentação oficial](https://code.claude.com/docs/en/mcp-quickstart).

Sem navegador habilitado, a Skill **não simula uma navegação inexistente**: ela informa a limitação e pode oferecer apenas análise documental com sua concordância.

## Exemplo de uso

> Use a Skill `validar-prototipo-persona` para avaliar o protótipo em `https://exemplo.com` com base no arquivo `persona.md`. Navegue pelas jornadas acessíveis, registre evidências e gere o relatório Markdown e o quadrante visual.

## Entregáveis

- `validacao-ux-[produto].md`: observações, análise, limitações e prioridades.
- `quadrante-feedback-[produto].png`: matriz visual 2×2, se houver capacidade de exportação.

## Segurança e limites

Não executar pagamentos, publicações, exclusões, cadastros externos ou alterações no protótipo sem autorização específica. Não inventar telas, acessos, evidências ou resultados. Diferenciar sempre o que a interface demonstrou da interpretação inferida para a persona.
