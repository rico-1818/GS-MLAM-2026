# 🚀 Análise Estatística de Missões Espaciais (1957–2020)

**Global Solution — Estatística e Análise de Dados**  
**Tema:** Nova Economia Espacial

---

## 📌 Descrição da Solução Desenvolvida

Este projeto realiza uma **análise estatística completa** do dataset *All Space Missions from 1957*, disponível publicamente no Kaggle. A base contém **4.324 registros reais** de lançamentos espaciais realizados entre 1957 e 2020, abrangendo 56 empresas e agências espaciais de todo o mundo.

O objetivo foi transformar dados históricos da exploração espacial em **informações úteis para apoio à tomada de decisão**, aplicando conceitos de estatística descritiva, visualização de dados e análise exploratória — diretamente alinhados ao contexto da Nova Economia Espacial.

A solução foi desenvolvida inteiramente em **Python**, seguindo as 5 etapas exigidas pela avaliação:

| Etapa | Descrição | Pontos |
|---|---|---|
| 1 | Seleção e justificativa da base de dados | 2,0 |
| 2 | Tabelas de distribuição de frequências (discreta e contínua) | 2,0 |
| 3 | Construção de gráficos estatísticos (histograma e barras) | 2,0 |
| 4 | Análises univariadas com estatística descritiva completa | 2,0 |
| 5 | Relatório técnico final em PDF | 2,0 |

---

## 🗃️ Base de Dados

| Atributo | Valor |
|---|---|
| **Nome** | All Space Missions from 1957 |
| **Fonte** | Kaggle |
| **Link** | https://www.kaggle.com/datasets/agirlcoding/all-space-missions-from-1957 |
| **Arquivo** | `Space_Corrected.csv` |
| **Total de registros** | 4.324 lançamentos |
| **Período coberto** | 1957 – 2020 (63 anos) |
| **Empresas/agências** | 56 operadoras |

### Variáveis analisadas

| Variável | Tipo | Descrição |
|---|---|---|
| `ano` | Quantitativa Discreta | Ano do lançamento |
| `custo_milhoes` | Quantitativa Contínua | Custo do foguete em milhões de USD |
| `pais` | Qualitativa Nominal | País de lançamento |
| `status_missao` | Qualitativa Nominal | Resultado: Success / Failure |
| `empresa` | Qualitativa Nominal | Operadora responsável |

---

## 📁 Estrutura do Repositório

```
Projeto-Estatistica/
│
├── README.md                          # Este arquivo
│
├── dados/
│   └── Space_Corrected.csv            # Base de dados original (Kaggle)
│
├── codigo/
│   └── analise_espacial_v2.ipynb      # Notebook principal com as 5 etapas
│   └── gerar_relatorio_v2.py          # Script gerador do relatório PDF
│
├── graficos/
│   ├── grafico1_histograma_custo.png  # Histograma — Custo dos foguetes
│   └── grafico2_barras_pais.png       # Barras — Lançamentos por país
│
├── relatorio/
│   └── relatorio_espacial_v2.pdf      # Relatório técnico final
│
└── entrega.txt                        # Nome, matrícula e link do GitHub
```

---

## 🔍 Principais Resultados

### Etapa 2 — Tabelas de Frequência
- A **década de 1970–1979** concentrou o maior volume de lançamentos (**23,42%**), auge da corrida espacial
- **56,86%** de todos os lançamentos históricos ocorreram antes de 1990
- A distribuição de custos é **bimodal**: 39,41% das missões custaram menos de US$50M e 15,49% custaram entre US$350–450M

### Etapa 3 — Gráficos
- **Gráfico 1 (Histograma):** evidencia forte assimetria positiva na distribuição de custos
- **Gráfico 2 (Barras):** Rússia (1.395) e EUA (1.344) dominam com 64% dos lançamentos históricos

### Etapa 4 — Estatística Descritiva
| Medida | Custo (US$ M) | Ano |
|---|---|---|
| Média | 129,80 | 1987 |
| Mediana | 62,00 | 1985 |
| Moda | 450,00 | 2018 |
| Desvio Padrão | 143,22 | 18,09 anos |
| Q1 | 40,00 | 1972 |
| Q3 | 164,00 | 2002 |

### Insights estratégicos
- 🎯 A **mediana (US$62M)** é o referencial de custo mais confiável — a média é distorcida por missões caríssimas
- ✅ Taxa de sucesso global de **89,7%** — risco operacional historicamente baixo
- 📈 **2018 foi o pico histórico** de lançamentos, marcando a era de foguetes reutilizáveis (SpaceX)
- 💡 O mercado está **polarizado** entre lançamentos baratos (<US$50M) e premium (>US$350M)

---

## ⚙️ Como Executar

### Pré-requisitos
```bash
pip install pandas numpy matplotlib scipy reportlab
```

### Opção 1 — Google Colab (recomendado, sem instalar nada)
1. Acesse [colab.research.google.com](https://colab.research.google.com)
2. Faça upload do arquivo `analise_espacial_v2.ipynb`
3. Faça upload do `Space_Corrected.csv` na aba de arquivos (ícone de pasta)
4. Execute célula por célula com o botão ▶

### Opção 2 — Jupyter local
```bash
# Na pasta do projeto
jupyter notebook analise_espacial_v2.ipynb
```

### Opção 3 — Gerar apenas o PDF
```bash
# Certifique-se de que os gráficos .png estão na mesma pasta
python gerar_relatorio_v2.py
```

---

## 🛠️ Tecnologias Utilizadas

| Biblioteca | Versão | Finalidade |
|---|---|---|
| Python | 3.x | Linguagem principal |
| pandas | latest | Carregamento e manipulação dos dados |
| numpy | latest | Cálculos numéricos |
| matplotlib | latest | Construção dos gráficos |
| scipy | latest | Cálculo de moda e estatísticas |
| reportlab | latest | Geração do relatório PDF |

---

## 📄 Licença

Uso acadêmico. Dataset original disponível no Kaggle sob licença pública de uso não-comercial.
