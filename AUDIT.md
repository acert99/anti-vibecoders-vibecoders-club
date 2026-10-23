# Política de curadoria

Esta política impede que o repositório vire uma coleção de links. A data da auditoria registra uma fotografia, não uma garantia futura.

## Fluxo

1. Registrar o candidato em `research/candidates.md` sem alterar a skill.
2. Confirmar repositório oficial ou relação verificável com o produto.
3. Verificar licença no próprio repositório e identificar exceções por pasta ou pacote.
4. Verificar se está arquivado, se tem documentação útil e se a atividade é compatível com seu papel.
5. Definir uma única função para a skill e comparar alternativas da mesma categoria.
6. Pontuar, registrar riscos e classificar.
7. Promover apenas quando o item muda uma decisão real do agente.

## Portões eliminatórios

- origem enganosa ou não verificável;
- licença ausente, incompatível ou confundida com “código visível”;
- documentação insuficiente para uso responsável;
- duplicação sem vantagem clara;
- incentivo predominante à cópia visual, conteúdo fictício ou efeitos sem função;
- problemas graves conhecidos sem alerta ou mitigação.

Um projeto proprietário pode permanecer como referência externa, mas nunca deve ser apresentado como open source.

## Pontuação

Avalie de 0 a 5:

- `R` relevância para evitar interfaces genéricas;
- `F` confiança na fonte/origem;
- `L` clareza e adequação da licença;
- `M` manutenção e saúde do projeto;
- `D` qualidade da documentação e exemplos;
- `A` aplicabilidade sem impor estética pronta.

Total máximo: 30.

- 24–30: aprovado, se nenhum portão eliminatório falhar;
- 19–23: referência condicional;
- 14–18: experimental/em espera;
- 0–13: rejeitado;
- qualquer nota: pode ser rejeitado por portão eliminatório.

## Regras do catálogo

- Máximo recomendado de três referências com a mesma função principal.
- Cada entrada deve dizer quando usar, quando evitar, licença e data da auditoria.
- O catálogo não é carregado por padrão: a `SKILL.md` o indica apenas em decisões de ferramenta.
- Stars não entram na pontuação.
- Não copiar documentação extensa; resumir a decisão e apontar para a fonte oficial.
- Revisar entradas anuais ou quando houver mudança relevante de licença, mantenedor ou estado do projeto.
- Remoções ficam registradas em `research/rejected.md`; não apagar histórico silenciosamente.

## Evidência mínima

Para cada auditoria, guardar URL canônica, vínculo oficial, licença observada, estado arquivado/não arquivado, função, riscos, pontuação, classificação e data. Quando uma evidência não puder ser confirmada, marcar `não confirmado` em vez de inferir.
