---
name: planejamento
description: "Guia o agente a criar planos estruturados para qualquer objetivo: projetos de software, features, estudos, eventos ou tarefas complexas. Usar quando o usuário pedir um plano, roadmap, estratégia, decomposição de tarefa ou organização antes de executar algo."
tags: ["mistral"]
---

# Planejamento

Use esta skill sempre que o usuário pedir para "planejar", "organizar", criar um "plano", "roadmap" ou estruturar uma ideia/tarefa antes de executá-la.

## 1. Entenda antes de planejar

Antes de escrever o plano, garanta que você sabe:
- **Objetivo final**: o que significa "pronto" ou "concluído"?
- **Contexto**: projeto existente ou do zero? Restrições de tempo, equipe, orçamento ou tecnologia?
- **Público**: o plano é para você mesmo executar, para um time, ou para apresentar a alguém?

Se faltar informação essencial, faça no máximo 2-3 perguntas objetivas antes de continuar. Não invente restrições que não foram ditas — registre-as como premissas.

## 2. Decomponha em fases

Quebre o objetivo em **fases ou etapas ordenadas**, cada uma com:
- **Entregável concreto**: o que existe no fim da fase (arquivo, feature, documento, decisão tomada)
- **Critério de conclusão**: como saber que a fase terminou
- **Dependências**: o que precisa estar pronto antes (de outra fase ou externo)

Prefira fases pequenas e verificáveis a fases grandes e vagas. Se o objetivo for simples, o plano pode ter 2-3 fases; se for complexo, evite passar de 7-8 fases — agrupe o que for muito granular.

## 3. Identifique riscos e premissas

Liste:
- **Premissas**: fatos que você está assumindo como verdade (ex.: "o usuário terá acesso à API X")
- **Riscos**: o que pode dar errado e o impacto
- **Mitigação**: uma ação concreta para cada risco relevante

## 4. Estime quando fizer sentido

Se houver restrição de prazo ou esforço, adicione uma estimativa simples por fase (ex.: horas/dias ou pequena/média/grande). Se não houver dados suficientes, diga "estimativa incerta" em vez de inventar números.

## 5. Defina checkpoints

Inclua **pontos de revisão**: após quais fases vale a pena parar, validar com o usuário e ajustar o plano antes de continuar.

## 6. Formato de saída

Entregue o plano em Markdown nesta estrutura:

# Plano: <nome do objetivo>

## Objetivo
Resumo em 1-2 frases do que será alcançado e o critério de sucesso.

## Premissas
- ...

## Fases
### Fase 1: <nome>
- Entregável: ...
- Critério de conclusão: ...
- Dependências: ...
- Estimativa: ... (se aplicável)

### Fase 2: <nome>
...

## Riscos e mitigações
| Risco | Impacto | Mitigação |
|---|---|---|
| ... | ... | ... |

## Checkpoints de revisão
- Após a Fase X: validar ...

## Próximo passo
A primeira ação concreta a executar agora.

## Regras
- Nunca invente fatos, nomes de pessoas, datas ou recursos; marque como premissa.
- Se o pedido for ambíguo, prefira um plano enxuto com perguntas em aberto do que um plano grande e errado.
- Ao atualizar um plano existente, preserve o que já foi concluído e indique o que mudou.
- Adapte o nível de detalhe ao tamanho da tarefa: tarefas simples = plano curto.
- Antes de entregar o plano, consulte o asset `references/checklist.md` e verifique cada item.
