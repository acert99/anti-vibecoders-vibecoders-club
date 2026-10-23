# Anti Vibecoders Club

[![License: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
![Claude Skill](https://img.shields.io/badge/Claude-Skill-6B4FBB)
![Codex Skill](https://img.shields.io/badge/Codex-Skill-10A37F)

Uma skill de IA (para **Claude** e **Codex**) que transforma sites gerados rapidamente em experiências com intenção, identidade e qualidade de produção.

Ela ajuda o agente a revisar ou implementar interfaces sem cair nos sinais clássicos de “site vibecodado” (*vibecoded*): texto genérico, hierarquia fraca, componentes repetidos, efeitos gratuitos, acessibilidade ignorada e acabamento técnico incompleto.

> **English:** An AI skill for **Claude** and **Codex/OpenAI agents** that turns quickly "vibe-coded" websites into intentional, production-quality experiences — covering visual direction, real content, accessibility (WCAG), technical SEO, performance and a launch-ready quality checklist. Install it as a Claude Skill (`claude/SKILL.md`) or a Codex skill (`SKILL.md`).

## O que ela cobre

- direção visual coerente com marca, público e objetivo;
- conteúdo real, hierarquia editorial e CTAs claros;
- responsividade, estados de loading/erro/vazio e rotas úteis;
- SEO técnico e compartilhamento social;
- acessibilidade e redução de movimento;
- performance e uso criterioso de Motion, Lenis, Spline e Unicorn Studio;
- checklist de lançamento baseado em evidências.

## Instalação

### Codex

Copie a pasta deste repositório para a pasta de skills do Codex ou instale a partir do GitHub quando seu ambiente oferecer instalação por repositório.

Depois, peça algo como:

> Use $anti-vibecoded-web para revisar este site e corrigir os sinais de implementação genérica.

> Use $anti-vibecoded-web para criar uma landing page com acabamento de produção, sem efeitos gratuitos.

### Claude

Use o arquivo consolidado [`claude/SKILL.md`](claude/SKILL.md) (mesmo conteúdo do `SKILL.md` + `references/`, reunido em um único documento, já que o formato de skill do Claude não lê múltiplos arquivos de referência). Adicione-o como uma skill da sua conta Claude (ou copie o conteúdo ao criar uma skill nova) e peça algo como:

> Revise este site e corrija os sinais de implementação genérica.

> Crie uma landing page com acabamento de produção, sem efeitos gratuitos.

A skill é ativada automaticamente pela descrição, sem precisar do prefixo `$`.

## Estrutura

- `SKILL.md`: fluxo principal e critérios de decisão (versão Codex);
- `references/quality-gates.md`: checklist de produção;
- `references/visual-direction.md`: como evitar estética genérica;
- `references/motion-and-3d.md`: uso responsável de motion, scroll e 3D;
- `references/library.md`: fontes e repositórios oficiais;
- `claude/SKILL.md`: versão consolidada para uso como skill do Claude.

## Princípio

Um site não parece profissional porque tem mais efeitos. Parece profissional quando cada decisão visual, textual e técnica parece intencional — e continua funcionando para pessoas, dispositivos e condições diferentes.

## Licença

MIT. As ferramentas e sites referenciados mantêm suas próprias licenças e termos.

## Palavras-chave

claude skill · codex skill · ai agent skill · vibecoding · vibe coding · landing page · web design · acessibilidade · WCAG · SEO técnico · design system · claude code · openai codex · llm tools.
