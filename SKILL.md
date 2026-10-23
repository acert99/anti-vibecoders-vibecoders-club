---
name: anti-vibecoded-web
description: Criar, revisar ou refinar sites para remover sinais de implementação genérica ou “vibecodada”, cobrindo direção visual, conteúdo, UX, acessibilidade, SEO, performance e acabamento de produção. Use em landing pages, portfólios, sites institucionais e experiências web; não use apenas para adicionar efeitos decorativos.
---

# Anti Vibecoded Web

Produza uma interface que pareça intencional, específica para a marca e pronta para uso real. Preserve a stack, o escopo e as escolhas explícitas do usuário.

## Fluxo

1. Entenda objetivo, público, ação principal, identidade existente e restrições técnicas. Quando faltarem dados, faça suposições pequenas e declaradas; não invente depoimentos, métricas, clientes ou credenciais.
2. Inspecione o produto renderizado e o código quando disponíveis. Diferencie problemas de direção, conteúdo, interação e engenharia.
3. Defina uma direção antes de polir componentes: promessa, tom, hierarquia, sistema tipográfico, paleta, ritmo espacial e uma ideia visual reconhecível.
4. Corrija primeiro o que bloqueia confiança ou uso: conteúdo genérico, CTA ambíguo, responsividade, navegação, contraste, teclado, estados e performance.
5. Adicione motion ou 3D somente quando houver função clara. Leia [references/motion-and-3d.md](references/motion-and-3d.md) antes de usar Motion, Lenis, Spline ou Unicorn Studio.
6. Verifique o resultado renderizado em larguras relevantes e conclua com evidências. Leia [references/quality-gates.md](references/quality-gates.md) para revisão ou entrega final.

## Critérios de decisão

- Especificidade vence decoração: conteúdo, imagens, exemplos e interações devem pertencer àquele negócio.
- Hierarquia vence uniformidade: cada seção precisa ter função, prioridade e ritmo próprios sem abandonar o sistema.
- Sistemas vencem remendos: use tokens e padrões consistentes, evitando valores arbitrários repetidos.
- Clareza vence novidade: navegação, formulários e CTAs não devem exigir descoberta.
- Evidência vence afirmação: não declare acessibilidade, SEO, performance ou responsividade sem verificar.
- Menos efeitos, melhor dirigidos: um gesto memorável e coerente vale mais do que animação em todos os elementos.

## Sinais que exigem correção

- hero com promessa intercambiável e CTA sem consequência clara;
- gradientes, glow, glassmorphism, bento grids ou ícones usados como padrão automático;
- seções com a mesma composição e o mesmo peso visual;
- texto fictício, métricas sem fonte ou imagens aleatórias;
- tudo animando ao entrar na tela, parallax constante ou scroll que interfere no controle do usuário;
- componentes sem estados hover, focus, active, disabled, loading, error, empty e success quando aplicáveis;
- layout que apenas encolhe no mobile em vez de recompor conteúdo e prioridade;
- página única tratada como produto completo, sem rotas auxiliares necessárias;
- metadados, compartilhamento, favicon, robots e sitemap esquecidos;
- dependências ou experiências pesadas adicionadas sem orçamento e fallback.

## Referências

- Para direção visual e diferenciação, leia [references/visual-direction.md](references/visual-direction.md).
- Para checklist técnico e editorial, leia [references/quality-gates.md](references/quality-gates.md).
- Para fontes oficiais e ferramentas, consulte [references/library.md](references/library.md). Use referências como repertório, não como licença para copiar.
- Para escolher dependências ou exemplos já auditados, consulte [references/catalog.md](references/catalog.md). Não promova itens da fila de pesquisa automaticamente.

## Curadoria do repositório

Ao adicionar uma referência, siga [AUDIT.md](AUDIT.md). Descoberta não equivale a aprovação: confirme origem, licença, manutenção, função específica e risco de homogeneização antes de mover um candidato para o catálogo.

## Entrega

Relate o que foi alterado, o que foi verificado e o que ainda depende de conteúdo, decisão ou serviço externo. Não esconda limitações atrás de linguagem promocional.
