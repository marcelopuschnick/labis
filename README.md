# LabIS — Candidatura · Marcelo Puschnick

Apresentação preparada especificamente para a minha candidatura à vaga de **edição e pós-produção do
Laboratório de Imagem e Som (LabIS)** da **PUC-Campinas**, na Faculdade de Jornalismo / Escola de
Linguagem e Comunicação.

Não é o meu material comercial. É uma proposta de retorno à Universidade: a vaga exercida por inteiro
mais uma camada de automação por IA local que a instituição ainda não tem — construída para ficar e
documentada para os alunos darem continuidade.

---

## Páginas

| Arquivo | Conteúdo |
|---|---|
| `index.html` | Página de recepção — a carta aberta, os números e o diferencial |
| `proposta.html` | Correspondência atividade por atividade com a vaga, a camada de IA local, o piloto em 4 etapas e a contrapartida |
| `sistemas.html` | Os 6 módulos na prática: ingest com IA, roteirização assistida, edição via MCP, ComfyUI, produção em lote e LGPD por desenho |
| `carta.html` | Carta formal ao Prof. Dr. Rogério Bazi, diretor da Faculdade de Jornalismo (1 página A4) |
| `curriculo.html` | Currículo (imprimível) |
| `contato.html` | Contato e disponibilidade |

---

## Sobre a honestidade técnica desta apresentação

Cada módulo em `sistemas.html` vem com etiqueta explícita separando o que **já roda** do que é
**proposta**:

- **Já roda** — ingest/transcrição (Whisper local), extração de mapa de montagem por LLM local,
  validação por um segundo modelo, exportação em EDL/OpenTimelineIO, memória de contexto local,
  documentação gerada do próprio código.
- **Proposta** — edição via MCP (agente operando a timeline) e criação visual com ComfyUI.
  Requerem trabalho de implementação, e no caso do ComfyUI, GPU.

Código dos módulos que já funcionam: [github.com/marcelopuschnick](https://github.com/marcelopuschnick)

---

## Rodando localmente

São páginas estáticas, sem build e sem dependências:

```bash
cd labis
python -m http.server 8000
# abra http://localhost:8000
```

Para gerar o PDF da carta: abra `carta.html` no navegador e imprima em A4 (cabe em uma página,
com "gráficos de fundo" ativado).

---

## Contato

Marcelo Henrique Puschnick · (19) 99946-2258 · marcelo_puschnick@icloud.com
