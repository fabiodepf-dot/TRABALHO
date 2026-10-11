# Perfil dos Candidatos às Eleições Gerais 2026

Projeto final do curso **DS-PY-004 — Técnicas de Programação I** (CAIXA Verso — Turma 1735).

**Integrantes:** Fabio de Paula Freitas, Flaviane Cristina Pereira Marra e Galvanir Machado Galvão.

## Objetivo
Analisar o perfil de quem se candidatou nas Eleições Gerais de 2026 (gênero, raça/cor e grau de instrução) e verificar se a participação feminina muda entre as regiões.

## A base
- **Fonte:** Tribunal Superior Eleitoral (TSE) — Portal de Dados Abertos (arquivo de candidatos).
- **Arquivo:** `dados/consulta_cand_2026_BRASIL.csv` (separador `;`, codificação `latin-1`).
- **Tamanho:** 20.989 linhas e 50 colunas. Cada linha é uma candidatura.
- **Recorte:** 1º turno, 04/10/2026, todo o Brasil.

## Perguntas
1. Qual é a distribuição de gênero entre os candidatos?
2. Como está distribuída a raça/cor dos candidatos?
3. Qual é o grau de instrução dos candidatos e ele muda conforme o cargo?
4. A participação feminina muda entre as regiões do país?

## Principais achados
- 64,9% dos candidatos são homens e 35,1% mulheres.
- Brancos (50,2%) e pardos (34,8%) somam 85% dos candidatos.
- 58,7% têm superior completo; no Executivo são 76,0%, entre deputados 57,6%.
- A participação feminina fica entre 34% e 36% em todas as regiões, pouco acima da cota de 30%.

## Estrutura
```
├── README.md
├── .gitignore
├── dados/
│   └── consulta_cand_2026_BRASIL.csv
└── notebooks/
    └── analise.ipynb
```

## Como reproduzir
1. Instale o Python 3.10 ou superior.
2. Instale as bibliotecas:
   ```
   pip install pandas numpy matplotlib pyarrow jupyter
   ```
3. Clone o repositório e abra `notebooks/analise.ipynb` no VS Code ou Jupyter.
4. Clique em **Executar Tudo**. O notebook grava a base limpa em `dados/candidatos_2026_limpo.parquet`.
