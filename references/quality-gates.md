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
