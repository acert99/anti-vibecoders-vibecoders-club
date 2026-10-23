# Motion, scroll e 3D

## Regra de entrada

Adicione uma ferramenta somente se ela resolver pelo menos uma função: orientar atenção, explicar mudança de estado, preservar continuidade espacial, demonstrar produto ou sustentar uma narrativa. Se a justificativa for apenas “ficar mais premium”, simplifique.

## Motion

- Prefira transições ligadas a causa e efeito a animações automáticas em massa.
- Anime `transform` e `opacity` quando possível; evite trabalho de layout por frame.
- Duração e easing devem refletir distância, importância e contexto.
- Não esconda conteúdo essencial até o JavaScript animá-lo.
- Respeite `prefers-reduced-motion` e ofereça estado final equivalente.

Use Motion quando a interação precisa de orquestração, gestos ou transições de layout que CSS não expressa bem. Para estados simples, CSS costuma ser suficiente.

## Lenis e smooth scroll

- Scroll nativo é o padrão. Use Lenis quando sincronização visual ou narrativa realmente depende disso.
- Preserve teclado, âncoras, seleção de texto, modais, containers aninhados e comportamento touch.
- Respeite redução de movimento e teste Safari/iOS e dispositivos modestos.
- Confirme compatibilidade com scroll snap, iframes e bibliotecas de scroll-trigger.

## Spline e Unicorn Studio

- Trate cenas como mídia pesada: poster/fallback, lazy loading, dimensões reservadas e limite de GPU/CPU.
- Não bloqueie CTA, leitura ou navegação enquanto a cena carrega.
- Pause ou reduza trabalho fora da viewport e em dispositivos limitados quando possível.
- Ofereça experiência estática equivalente para redução de movimento ou falha de WebGL.
- Verifique licença e termos. Código disponível publicamente não implica licença open source.

## Orçamento sugerido

Defina antes de implementar: impacto máximo aceitável em bundle, tempo até interação, memória e estabilidade visual. Meça no projeto real; não reutilize números arbitrários como garantia universal.
