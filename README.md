# TP1 — P3: Tramitação dos processos de P&D (BPMN)

ICC412 — Processo de Desenvolvimento de Software · 2026/2 · Prof. Leonardo Marques
Entregável **E1** (Diagrama BPMN) — responsabilidade do Integrante 2.

Modelagem do fluxo de celebração de Acordos de Parceria para Pesquisa, Desenvolvimento
e Inovação (APPDI) do IComp/UFAM: do interesse de uma empresa parceira até a assinatura
e publicação do convênio.

## Estrutura

```
diagrama/
  process-p3.bpmn   ← arquivo nativo (abrir no Camunda Modeler ou bpmn.io)
  process-p3.png    ← exportado em alta resolução
  process-p3.pdf    ← exportado em alta resolução
```

## Como abrir / editar

1. Instale o [Camunda Modeler](https://camunda.com/download/modeler) (gratuito).
2. Abra `diagrama/process-p3.bpmn`.
3. Ao salvar (`Cmd+S`), o Modeler sobrescreve o mesmo arquivo — o histórico de
   versões é mantido pelo git (ver abaixo), não por cópias manuais do arquivo.

## Fontes usadas na modelagem

- `ICC412_TP1_Especificacao.pdf` — enunciado do trabalho.
- Entrevista com a Socorro (Secretaria do IComp), realizada em 10/09/2026.
- **Resolução CONSAD-UFAM nº 047, de 12/11/2024** (Processo nº 055/2024-CONSAD,
  SEI 23105.041071/2024-75) — dispõe sobre a instrução processual do APPDI e traz,
  em anexo, o fluxograma oficial do processo. Esta é a referência normativa
  principal do diagrama.

## Histórico de versões

Cada linha corresponde a um commit relevante deste repositório. Para atualizar
esta tabela depois de commitar, rode `git log --oneline` e copie o hash curto.

| Versão | Commit    | Data       | Descrição |
|--------|-----------|------------|-----------|
| v0.1   | `ef23eaf` | 2026-09-19 | Estrutura inicial do repositório (README, .gitignore, pasta `diagrama/`) — ainda sem o arquivo `.bpmn`. |
| v0.2   | `pendente` | —          | Primeiro esqueleto do diagrama: pools e lanes (Empresa, Professor/Coordenador, Secretaria do IComp, PROTEC, CITEC, PROADM/DCC, Procuradoria Federal, Fundação de Apoio), sem gateways. |
| v0.3   | `pendente` | —          | Adição dos gateways, prazos (Art. 18–20) e da exceção de dispensa da Procuradoria com minuta padrão AGU (Art. 8º), conforme a Resolução 047/2024. |
| v1.0   | `pendente` | —          | Revisão pós-validação com a Socorro (escopo único para pesquisa/capacitação/especialização; remoção de etapa interna do IComp não confirmada) — **versão final de entrega**. |

> Ao fechar cada etapa, atualize a linha correspondente com o hash do commit
> (`git log --oneline -1`) e a data real. Se o diagrama passar por mais uma
> rodada de ajuste depois da v1.0, adicione uma nova linha em vez de reescrever
> uma existente — é isso que comprova o refinamento para o relatório (E3).

## Citando isto no relatório (E3)

Na seção "Justificativa das escolhas de modelagem" ou nas "Limitações", uma frase
como esta já basta: *"O diagrama foi versionado com git ao longo do trabalho; o
histórico completo, incluindo a evolução de rascunho até a versão final, está
documentado no README do repositório de modelagem."* Se quiser, anexe uma captura
de tela de `git log --oneline --graph` como evidência.
