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
