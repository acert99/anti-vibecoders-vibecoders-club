---
name: anti-vibecoded-web
description: Criar ou revisar sites para remover sinais de implementação genérica, cobrindo direção visual, conteúdo, acessibilidade, SEO, performance e acabamento de produção.
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

## Referências consolidadas

As seções abaixo reúnem direção visual, quality gates, motion/3D, biblioteca e catálogo auditado em um único documento.

## Curadoria do repositório

Ao adicionar uma referência, exija origem, licença, manutenção, função específica e risco de homogeneização antes de promovê-la. Descoberta não equivale a aprovação: confirme origem, licença, manutenção, função específica e risco de homogeneização antes de mover um candidato para o catálogo.

## Entrega

Relate o que foi alterado, o que foi verificado e o que ainda depende de conteúdo, decisão ou serviço externo. Não esconda limitações atrás de linguagem promocional.

---

# Direção visual sem fórmula pronta

## Comece pela tese

Escreva uma frase interna: “Esta experiência deve parecer ___ porque o público precisa sentir/compreender ___.” Use isso para filtrar escolhas. “Moderno”, “clean” e “premium” são vagos; prefira atributos observáveis como editorial, técnico, artesanal, direto, tátil ou institucional.

## Construa um sistema pequeno

- Uma escala tipográfica com papéis claros, não tamanhos isolados por componente.
- Uma escala de espaçamento e regras de densidade.
- Cor de superfície, texto, ação, feedback e destaque com contraste verificável.
- Raios, bordas e sombras coerentes com o caráter da marca.
- Padrões de interação para links, botões, campos, cards e navegação.

## Crie diferença pelo conteúdo

Antes de adicionar efeito, procure matéria-prima: processo, produto, textura, dados, bastidores, voz, arquivo, geografia, pessoas e resultados reais. Uma composição derivada desse material é mais memorável que uma tendência aplicada por padrão.

## Evite a assinatura automática de gerador

- Não escolha Inter + roxo + glow + cartões arredondados apenas por conveniência.
- Não use ícones genéricos onde fotografia, ilustração, número, palavra ou diagrama comunica melhor.
- Não repita “headline + parágrafo + três cards” em toda seção.
- Não centralize tudo; contraste alinhamento, escala e respiro com intenção.
- Não use copy inflada para compensar ausência de mensagem.

## Use galerias como pesquisa

Ao consultar Inspora, Refero ou outras galerias, registre o princípio observado — ritmo, contraste, navegação, tratamento de mídia — em vez de copiar a aparência. Combine referências de categorias diferentes e valide se a solução ainda serve ao conteúdo, à acessibilidade e à performance.

---

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

---

# Quality gates

Use apenas as partes relevantes ao projeto. Um item só está concluído quando há evidência no código ou no produto renderizado.

## Experiência e conteúdo

- A primeira dobra comunica o que é oferecido, para quem e qual é a próxima ação.
- O CTA principal aparece cedo e usa verbo + consequência clara.
- Título da página e H1 são específicos; a hierarquia de headings é lógica.
- Não há lorem ipsum, depoimentos, logos, avaliações ou números inventados.
- Navegação, links, formulários e ações principais funcionam de verdade.
- Existem páginas ou estados úteis para 404, erro, vazio, loading e sucesso conforme o produto.
- Conteúdo legal e de privacidade existe quando o contexto exige; não gere texto jurídico definitivo sem revisão apropriada.

## Identidade e responsividade

- Tipografia, cor, espaçamento, borda, sombra e movimento seguem tokens ou regras reconhecíveis.
- Pelo menos uma decisão visual é distintiva e derivada da marca ou do conteúdo.
- Mobile recompõe ordem, densidade e prioridade; não é apenas desktop comprimido.
- Layout suporta texto maior, títulos longos e conteúdo real sem quebrar.
- Imagens têm enquadramento, proporção e tratamento consistentes.

## Acessibilidade

- HTML semântico, landmarks e ordem de headings coerentes.
- Navegação completa por teclado, foco visível e ordem de tabulação previsível.
- Labels, nomes acessíveis e mensagens de erro úteis em controles.
- Contraste suficiente e informação não dependente apenas de cor.
- `alt` descreve imagens informativas; imagens decorativas usam alternativa vazia.
- `prefers-reduced-motion` é respeitado; conteúdo não depende de animação para existir.
- Alvos de toque, zoom, orientação e leitor de tela foram considerados.

## SEO e compartilhamento

- Cada rota indexável tem title e meta description próprios.
- Canonical, Open Graph e Twitter Card refletem a página e usam imagem válida.
- Favicon e ícones de aplicação adequados.
- `robots.txt` e `sitemap.xml` existem e correspondem ao ambiente; staging não vaza para indexação.
- Dados estruturados são válidos e representam conteúdo realmente visível.
- 404 usa status correto; redirects e URLs antigas são tratados quando aplicável.

## Performance e resiliência

- Imagens são dimensionadas, comprimidas, responsivas e lazy-loaded fora da primeira dobra.
- Fontes têm formatos modernos, subset quando útil, preload criterioso e fallback compatível.
- JavaScript de terceiros, motion e 3D têm motivo, orçamento e carregamento adiado quando possível.
- O conteúdo essencial permanece útil com rede lenta, falhas parciais e scripts opcionais indisponíveis.
- Evite layout shift reservando espaço para mídia, embeds e conteúdo assíncrono.
- Verifique Core Web Vitals ou métricas equivalentes no ambiente adequado; não prometa pontuação sem medir.

## Produção

- Analytics só é instalado com finalidade definida, eventos nomeados e consentimento quando exigido.
- Segredos não estão no cliente nem no repositório.
- Dependências, console, erros de build, links quebrados e headers de segurança foram revisados.
- Domínio, HTTPS, cache, página de erro e monitoramento estão configurados conforme a hospedagem.
- Não transforme a checklist da imagem em regra cega: por exemplo, nem todo site precisa de política própria, analytics ou várias rotas, mas toda ausência deve ser intencional.

---

# Biblioteca de referências

Priorize documentação e repositórios oficiais. Versões, licenças e limites podem mudar; verifique antes de implementar.

## Implementação

- [Motion](https://motion.dev/) — animação para JavaScript e React. Repositório: [motiondivision/motion](https://github.com/motiondivision/motion).
- [GSAP](https://gsap.com/) — animação avançada sob a licença padrão da GreenSock. O uso pode ser gratuito, mas não trate o código como open source; confirme os termos atuais. Repositório: [greensock/GSAP](https://github.com/greensock/GSAP).
- [Lenis](https://lenis.dev/) — smooth scroll. Repositório: [darkroomengineering/lenis](https://github.com/darkroomengineering/lenis).
- [Three.js](https://threejs.org/) e [React Three Fiber](https://r3f.docs.pmnd.rs/) — base para 3D customizado no navegador e sua integração declarativa com React. Repositórios: [mrdoob/three.js](https://github.com/mrdoob/three.js) e [pmndrs/react-three-fiber](https://github.com/pmndrs/react-three-fiber).
- [Rive](https://rive.app/) — animações vetoriais interativas para microinterações e estados visuais. Repositório: [rive-app/rive-wasm](https://github.com/rive-app/rive-wasm).
- [Spline](https://spline.design/) — criação e runtime de experiências 3D. Organização: [splinetool](https://github.com/splinetool); integração React: [splinetool/react-spline](https://github.com/splinetool/react-spline).
- [Unicorn Studio](https://www.unicorn.studio/) — experiências visuais interativas. SDK: [hiunicornstudio/unicornstudio.js](https://github.com/hiunicornstudio/unicornstudio.js). O SDK publicado tem licença proprietária; leia os termos antes de reutilizar ou modificar.
- [Spell](https://spell.sh/) — referência para experiências 3D geradas por IA; confirme documentação, exportação, licença e custo antes de assumir integração.

## Design systems e componentes

- [shadcn/ui](https://ui.shadcn.com/) — componentes copiados para o projeto e adaptados localmente. Use como base técnica, não como identidade pronta. Repositório: [shadcn-ui/ui](https://github.com/shadcn-ui/ui).
- [Radix UI](https://www.radix-ui.com/) — primitivos acessíveis para foco, teclado e ARIA antes do estilo visual. Repositório: [radix-ui/primitives](https://github.com/radix-ui/primitives).

## Pesquisa visual

- [Inspora](https://www.inspora.design/) — arquivo de trabalhos visuais para pesquisa de direção.
- [Refero Styles](https://styles.refero.design/) — referências organizadas por estilos e padrões.
- [Awwwards](https://www.awwwards.com/), [Recent.Design](https://recent.design/), [SiteInspire](https://www.siteinspire.com/), [Land-book](https://land-book.com/) e [One Page Love](https://onepagelove.com/) — galerias para calibrar repertório; extraia princípios, não layouts.

Esses sites não são dependências obrigatórias e nem todos expõem um repositório público oficial. Não atribua um repositório por semelhança de nome.

## Repositórios de execução em produção

Projetos open source úteis para estudar hierarquia, densidade, estados e acabamento — não para copiar.

- [calcom/cal.diy](https://github.com/calcom/cal.diy) — produto de agendamento com sistema visual aplicado em produção.
- [supabase/supabase](https://github.com/supabase/supabase) — produto, site e documentação com conteúdo técnico denso.
- [tldraw/tldraw](https://github.com/tldraw/tldraw) e [excalidraw/excalidraw](https://github.com/excalidraw/excalidraw) — interação e estado refinados em interfaces de canvas.

## Fontes fundamentais

- [WCAG 2.2](https://www.w3.org/TR/WCAG22/) — critérios de acessibilidade.
- [WCAG 2.2 — quick reference](https://www.w3.org/WAI/WCAG22/quickref/) — filtro prático por critério.
- [web.dev — Core Web Vitals](https://web.dev/articles/vitals) — métricas de experiência e performance.
- [Google Search Central — SEO Starter Guide](https://developers.google.com/search/docs/fundamentals/seo-starter-guide) — fundamentos de descoberta e indexação.
- [Open Graph protocol](https://ogp.me/) — metadados de compartilhamento.
- [Schema.org](https://schema.org/) — vocabulário de dados estruturados.

---

# Catálogo auditado

Auditoria inicial: 2026-10-22. Os repositórios abaixo estavam públicos e não arquivados na data da consulta. Verifique versões e licenças novamente antes de adotar.

## Motion e scroll

| Repositório | Função | Use quando | Evite quando | Licença | Nota |
|---|---|---|---|---|---:|
| [motiondivision/motion](https://github.com/motiondivision/motion) | animação JS/React | gestos, layout e sequências justificadas | CSS resolve o estado simples | MIT | 28 |
| [darkroomengineering/lenis](https://github.com/darkroomengineering/lenis) | smooth scroll | narrativa ou sincronização visual depende do scroll | scroll nativo atende; compatibilidade é incerta | MIT | 26 |
| [formkit/auto-animate](https://github.com/formkit/auto-animate) | transições automáticas de layout | listas e estados simples precisam continuidade | controle coreográfico detalhado é necessário | MIT | 23 |

## 3D e WebGL

| Repositório | Função | Use quando | Evite quando | Licença | Nota |
|---|---|---|---|---|---:|
| [mrdoob/three.js](https://github.com/mrdoob/three.js) | engine WebGL/WebGPU | experiência 3D customizada justifica engenharia própria | mídia estática ou ferramenta visual basta | MIT | 27 |
| [pmndrs/react-three-fiber](https://github.com/pmndrs/react-three-fiber) | Three.js declarativo em React | cena pertence à arquitetura React | integração simples não exige reconciler | MIT | 26 |
| [splinetool/react-spline](https://github.com/splinetool/react-spline) | incorporar cenas Spline | equipe produz cenas no editor Spline | falta fallback, orçamento ou controle de carregamento | MIT | 22 |

## Primitivos acessíveis e sistemas

| Repositório | Função | Use quando | Evite quando | Licença | Nota |
|---|---|---|---|---|---:|
| [radix-ui/primitives](https://github.com/radix-ui/primitives) | primitivas headless acessíveis | React precisa de comportamento complexo sem visual imposto | componente nativo simples basta | MIT | 28 |
| [adobe/react-spectrum](https://github.com/adobe/react-spectrum) | hooks e componentes acessíveis | produto complexo exige padrões robustos | peso e abstração excedem o escopo | Apache-2.0 | 27 |
| [tailwindlabs/headlessui](https://github.com/tailwindlabs/headlessui) | componentes headless | React/Vue precisa de interações acessíveis | projeto não usa stack compatível | MIT | 25 |
| [shadcn-ui/ui](https://github.com/shadcn-ui/ui) | código de componentes adaptável | serve como base técnica a ser redesenhada | aparência padrão seria mantida | MIT | 22 |

MUI, Chakra UI e Mantine permanecem referências condicionais: maduros e permissivos, mas podem dominar a identidade se usados sem direção visual própria.

## Acessibilidade e padrões

| Repositório | Função | Limite | Licença | Nota |
|---|---|---|---|---:|
| [dequelabs/axe-core](https://github.com/dequelabs/axe-core) | testes automatizados de acessibilidade | automação não substitui revisão manual | MPL-2.0 | 27 |
| [jsx-eslint/eslint-plugin-jsx-a11y](https://github.com/jsx-eslint/eslint-plugin-jsx-a11y) | lint de JSX | encontra padrões, não experiência completa | MIT | 25 |
| [w3c/wcag](https://github.com/w3c/wcag) | fonte normativa da WCAG | consultar versão publicada e contexto | documento oficial | 28 |
| [whatwg/html](https://github.com/whatwg/html) | padrão vivo de HTML | usar como fonte, não tutorial rápido | especificação WHATWG | 27 |

## Performance, teste e documentação

| Repositório | Função | Limite | Licença | Nota |
|---|---|---|---|---:|
| [GoogleChrome/lighthouse](https://github.com/GoogleChrome/lighthouse) | diagnóstico de qualidade e performance | pontuação não equivale a experiência real | Apache-2.0 | 27 |
| [GoogleChrome/lighthouse-ci](https://github.com/GoogleChrome/lighthouse-ci) | regressão em CI | exige orçamento e ambiente estável | Apache-2.0 | 25 |
| [microsoft/playwright](https://github.com/microsoft/playwright) | teste real em navegadores | seletores e cenários precisam representar usuários | Apache-2.0 | 28 |
| [storybookjs/storybook](https://github.com/storybookjs/storybook) | estados e documentação de componentes | não substitui teste integrado da página | MIT | 26 |

## Referências condicionais adicionais

- [mui/material-ui](https://github.com/mui/material-ui), [chakra-ui/chakra-ui](https://github.com/chakra-ui/chakra-ui) e [mantinedev/mantine](https://github.com/mantinedev/mantine): boas referências de API, estados e sistemas; redesenhar identidade.
- [vercel/geist-font](https://github.com/vercel/geist-font): tipografia útil, não escolha automática para todo produto.
- [vercel/examples](https://github.com/vercel/examples): padrões técnicos por stack; exemplos não são direção de produto.
