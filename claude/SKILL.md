---
name: anti-vibecoded-web
description: Criar, revisar ou refinar sites e interfaces web para remover sinais de implementação genérica ("vibecodada"), cobrindo direção visual, conteúdo, UX, acessibilidade, SEO, performance e acabamento de produção. Use em landing pages, portfólios, sites institucionais e experiências web; não use apenas para adicionar efeitos decorativos.
---

# Anti Vibecoded Web

Produza uma interface que pareça intencional, específica para a marca e pronta para uso real. Preserve a stack, o escopo e as escolhas explícitas do usuário.

## Fluxo

1. Entenda objetivo, público, ação principal, identidade existente e restrições técnicas. Quando faltarem dados, faça suposições pequenas e declaradas; não invente depoimentos, métricas, clientes ou credenciais.
2. Inspecione o produto renderizado e o código quando disponíveis. Diferencie problemas de direção, conteúdo, interação e engenharia.
3. Defina uma direção antes de polir componentes: promessa, tom, hierarquia, sistema tipográfico, paleta, ritmo espacial e uma ideia visual reconhecível.
4. Corrija primeiro o que bloqueia confiança ou uso: conteúdo genérico, CTA ambíguo, responsividade, navegação, contraste, teclado, estados e performance.
5. Adicione motion ou 3D somente quando houver função clara (ver seção "Motion, scroll e 3D" abaixo).
6. Verifique o resultado renderizado em larguras relevantes e conclua com evidências (ver "Quality gates" abaixo).

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

## Direção visual sem fórmula pronta

### Comece pela tese

Escreva uma frase interna: "Esta experiência deve parecer ___ porque o público precisa sentir/compreender ___." Use isso para filtrar escolhas. "Moderno", "clean" e "premium" são vagos; prefira atributos observáveis como editorial, técnico, artesanal, direto, tátil ou institucional.

### Construa um sistema pequeno

- Uma escala tipográfica com papéis claros, não tamanhos isolados por componente.
- Uma escala de espaçamento e regras de densidade.
- Cor de superfície, texto, ação, feedback e destaque com contraste verificável.
- Raios, bordas e sombras coerentes com o caráter da marca.
- Padrões de interação para links, botões, campos, cards e navegação.

### Crie diferença pelo conteúdo

Antes de adicionar efeito, procure matéria-prima: processo, produto, textura, dados, bastidores, voz, arquivo, geografia, pessoas e resultados reais. Uma composição derivada desse material é mais memorável que uma tendência aplicada por padrão.

### Evite a assinatura automática de gerador

- Não escolha Inter + roxo + glow + cartões arredondados apenas por conveniência.
- Não use ícones genéricos onde fotografia, ilustração, número, palavra ou diagrama comunica melhor.
- Não repita "headline + parágrafo + três cards" em toda seção.
- Não centralize tudo; contraste alinhamento, escala e respiro com intenção.
- Não use copy inflada para compensar ausência de mensagem.

### Use galerias como pesquisa

Ao consultar Inspora, Refero ou outras galerias, registre o princípio observado — ritmo, contraste, navegação, tratamento de mídia — em vez de copiar a aparência. Combine referências de categorias diferentes e valide se a solução ainda serve ao conteúdo, à acessibilidade e à performance.

## Motion, scroll e 3D

### Regra de entrada

Adicione uma ferramenta somente se ela resolver pelo menos uma função: orientar atenção, explicar mudança de estado, preservar continuidade espacial, demonstrar produto ou sustentar uma narrativa. Se a justificativa for apenas "ficar mais premium", simplifique.

### Motion

- Prefira transições ligadas a causa e efeito a animações automáticas em massa.
- Anime `transform` e `opacity` quando possível; evite trabalho de layout por frame.
- Duração e easing devem refletir distância, importância e contexto.
- Não esconda conteúdo essencial até o JavaScript animá-lo.
- Respeite `prefers-reduced-motion` e ofereça estado final equivalente.
- Use uma lib de motion (ex.: Motion/Framer Motion) quando a interação precisa de orquestração, gestos ou transições de layout que CSS puro não expressa bem. Para estados simples, CSS costuma ser suficiente.

### Smooth scroll

- Scroll nativo é o padrão. Use smooth scroll (ex.: Lenis) apenas quando sincronização visual ou narrativa realmente depende disso.
- Preserve teclado, âncoras, seleção de texto, modais, containers aninhados e comportamento touch.
- Respeite redução de movimento e teste Safari/iOS e dispositivos modestos.
- Confirme compatibilidade com scroll snap, iframes e bibliotecas de scroll-trigger.

### 3D e cenas interativas (Spline, Unicorn Studio e similares)

- Trate cenas como mídia pesada: poster/fallback, lazy loading, dimensões reservadas e limite de GPU/CPU.
- Não bloqueie CTA, leitura ou navegação enquanto a cena carrega.
- Pause ou reduza trabalho fora da viewport e em dispositivos limitados quando possível.
- Ofereça experiência estática equivalente para redução de movimento ou falha de WebGL.
- Verifique licença e termos; código disponível publicamente não implica licença open source.

### Orçamento sugerido

Defina antes de implementar: impacto máximo aceitável em bundle, tempo até interação, memória e estabilidade visual. Meça no projeto real; não reutilize números arbitrários como garantia universal.

## Quality gates

Use apenas as partes relevantes ao projeto. Um item só está concluído quando há evidência no código ou no produto renderizado.

### Experiência e conteúdo

- A primeira dobra comunica o que é oferecido, para quem e qual é a próxima ação.
- O CTA principal aparece cedo e usa verbo + consequência clara.
- Título da página e H1 são específicos; a hierarquia de headings é lógica.
- Não há lorem ipsum, depoimentos, logos, avaliações ou números inventados.
- Navegação, links, formulários e ações principais funcionam de verdade.
- Existem páginas ou estados úteis para 404, erro, vazio, loading e sucesso conforme o produto.
- Conteúdo legal e de privacidade existe quando o contexto exige; não gere texto jurídico definitivo sem revisão apropriada.

### Identidade e responsividade

- Tipografia, cor, espaçamento, borda, sombra e movimento seguem tokens ou regras reconhecíveis.
- Pelo menos uma decisão visual é distintiva e derivada da marca ou do conteúdo.
- Mobile recompõe ordem, densidade e prioridade; não é apenas desktop comprimido.
- Layout suporta texto maior, títulos longos e conteúdo real sem quebrar.
- Imagens têm enquadramento, proporção e tratamento consistentes.

### Acessibilidade

- HTML semântico, landmarks e ordem de headings coerentes.
- Navegação completa por teclado, foco visível e ordem de tabulação previsível.
- Labels, nomes acessíveis e mensagens de erro úteis em controles.
- Contraste suficiente e informação não dependente apenas de cor.
- `alt` descreve imagens informativas; imagens decorativas usam alternativa vazia.
- `prefers-reduced-motion` é respeitado; conteúdo não depende de animação para existir.
- Alvos de toque, zoom, orientação e leitor de tela foram considerados.

### SEO e compartilhamento

- Cada rota indexável tem title e meta description próprios.
- Canonical, Open Graph e Twitter Card refletem a página e usam imagem válida.
- Favicon e ícones de aplicação adequados.
- `robots.txt` e `sitemap.xml` existem e correspondem ao ambiente; staging não vaza para indexação.
- Dados estruturados são válidos e representam conteúdo realmente visível.
- 404 usa status correto; redirects e URLs antigas são tratados quando aplicável.

### Performance e resiliência

- Imagens são dimensionadas, comprimidas, responsivas e lazy-loaded fora da primeira dobra.
- Fontes têm formatos modernos, subset quando útil, preload criterioso e fallback compatível.
- JavaScript de terceiros, motion e 3D têm motivo, orçamento e carregamento adiado quando possível.
- O conteúdo essencial permanece útil com rede lenta, falhas parciais e scripts opcionais indisponíveis.
- Evite layout shift reservando espaço para mídia, embeds e conteúdo assíncrono.
- Verifique Core Web Vitals ou métricas equivalentes no ambiente adequado; não prometa pontuação sem medir.

### Produção

- Analytics só é instalado com finalidade definida, eventos nomeados e consentimento quando exigido.
- Segredos não estão no cliente nem no repositório.
- Dependências, console, erros de build, links quebrados e headers de segurança foram revisados.
- Domínio, HTTPS, cache, página de erro e monitoramento estão configurados conforme a hospedagem.
- Não transforme esta checklist em regra cega: nem todo site precisa de política própria, analytics ou várias rotas, mas toda ausência deve ser intencional.

## Biblioteca de referências

Priorize documentação e repositórios oficiais. Versões, licenças e limites podem mudar; verifique antes de implementar.

- Motion (motion.dev) — animação para JavaScript e React.
- Lenis (lenis.dev) — smooth scroll.
- Spline (spline.design) — criação e runtime de experiências 3D.
- Unicorn Studio (unicorn.studio) — experiências visuais interativas; SDK com licença proprietária, leia os termos antes de reutilizar.
- Inspora (inspora.design) e Refero Styles (styles.refero.design) — pesquisa visual; extraia princípios, não clones.
- WCAG 2.2 — critérios de acessibilidade.
- web.dev Core Web Vitals — métricas de performance.
- Google Search Central SEO Starter Guide — fundamentos de SEO.
- Open Graph protocol e Schema.org — metadados e dados estruturados.

## Entrega

Relate o que foi alterado, o que foi verificado e o que ainda depende de conteúdo, decisão ou serviço externo. Não esconda limitações atrás de linguagem promocional.
