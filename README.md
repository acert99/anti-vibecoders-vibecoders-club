# Anti Vibecoders Club

Uma skill para transformar sites gerados rapidamente em experiências com intenção, identidade e qualidade de produção.

Ela ajuda o Codex (ou o Claude) a revisar ou implementar interfaces sem cair nos sinais clássicos de “site vibecodado”: texto genérico, hierarquia fraca, componentes repetidos, efeitos gratuitos, acessibilidade ignorada e acabamento técnico incompleto.

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
