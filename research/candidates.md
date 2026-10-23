# Fila e resultado da primeira triagem

Auditoria: 2026-10-22. Escopo: 28 repositórios. Estado público e não arquivado foi conferido via GitHub; licenças foram lidas no arquivo do repositório quando disponível.

## Aprovados para o catálogo (15)

`motiondivision/motion`, `darkroomengineering/lenis`, `mrdoob/three.js`, `pmndrs/react-three-fiber`, `radix-ui/primitives`, `adobe/react-spectrum`, `tailwindlabs/headlessui`, `dequelabs/axe-core`, `jsx-eslint/eslint-plugin-jsx-a11y`, `GoogleChrome/lighthouse`, `GoogleChrome/lighthouse-ci`, `microsoft/playwright`, `storybookjs/storybook`, `w3c/wcag`, `whatwg/html`.

## Referência condicional (8)

- `splinetool/react-spline` — integração oficial útil; 3D precisa fallback e orçamento.
- `formkit/auto-animate` — excelente para transições simples; pode mascarar ausência de direção de motion.
- `shadcn-ui/ui` — base técnica útil; alto risco de homogeneização visual.
- `mui/material-ui`, `chakra-ui/chakra-ui`, `mantinedev/mantine` — maduros; identidade padrão não deve dirigir a marca.
- `vercel/geist-font` — boa fonte, não escolha universal.
- `vercel/examples` — referência técnica ampla demais para orientar estética.

## Em espera (3)

- `ariakit/ariakit` — projeto relevante, mas o monorepo contém licenças diferentes; auditar por pacote antes de recomendar.
- `pa11y/pa11y` — ferramenta útil sob LGPL-3.0; avaliar implicações e sobreposição com axe/Lighthouse.
- `BuilderIO/partytown` — solução especializada para scripts de terceiros; verificar estado, licença e benefício atual antes de promover.

## Não promovidos (2)

- `greensock/GSAP` — ferramenta forte, mas usa licença padrão própria; manter como opção condicionada aos termos, não como padrão aberto.
- `hiunicornstudio/unicornstudio.js` — SDK oficial com licença proprietária descrita no README; referência de integração, não dependência open source.

## Segunda triagem (2026-10-23)

Escopo: 31 repositórios consultados via API do GitHub; licença confirmada no arquivo de licença para os promovidos.

- Aprovados (5): `floating-ui/floating-ui`, `w3c/aria-practices`, `lovell/sharp`, `fontsource/fontsource`, `GoogleChrome/web-vitals`.
- Condicionais (6): `primer/react`, `alphagov/govuk-design-system`, `lucide-icons/lucide`, `tabler/tabler-icons`, `d3/d3`, `observablehq/plot`.
- Em espera: `theatre-js/theatre` (último push 2024-08-14), `rsms/inter` (último push 2024-11-19; sobrepõe Geist), `uswds/uswds` (licença mista, auditar por pasta).
- Rejeitado: `primer/design` (arquivado).
- Não confirmado: notas são estimativas do avaliador; documentação foi conferida só pela presença do README.

## Próxima rodada sugerida

Investigar conteúdo e tipografia, imagens responsivas, performance de fontes, view transitions, Web Components, segurança de frontend e exemplos de direção visual baseados em conteúdo. Cada nova rodada deve comparar candidatos com os já aprovados, não apenas somar nomes.
