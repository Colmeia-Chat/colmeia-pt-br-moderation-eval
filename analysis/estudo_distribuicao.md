# Distribuição das categorias

O conjunto contém 3.764 textos: 1.665 traduzidos, 1.921 com anotação manual e 178 sintéticos. A contagem por categoria considera rótulos positivos. Um registro pode receber mais de um rótulo.

| Categoria | Traduzidos | Anotação manual | Sintéticos | Total |
|---|---:|---:|---:|---:|
| hate | 162 | 132 | 0 | 294 |
| hate/threatening | 41 | 120 | 0 | 161 |
| sexual | 230 | 19 | 0 | 249 |
| sexual/minors | 83 | 0 | 117 | 200 |
| illicit | 0 | 172 | 61 | 233 |
| illicit/violent | 0 | 48 | 61 | 109 |
| violence | 21 | 362 | 26 | 409 |
| self-harm | 51 | 230 | 0 | 281 |
| self-harm/instructions | 0 | 100 | 0 | 100 |
| self-harm/intent | 0 | 79 | 0 | 79 |
| harassment | 75 | 162 | 0 | 237 |
| harassment/threatening | 0 | 116 | 0 | 116 |

## Interpretação

Intenção de autolesão apresenta o menor suporte positivo, com 79 textos. Ilícitos violentos apresenta 109 positivos, dos quais 61 são sintéticos. Assédio com ameaça apresenta 116 positivos.

A contagem total não garante exemplos independentes nem equilíbrio de subtipos. A interpretação do desempenho deve considerar a origem e a cobertura de anotação.

Na configuração sem_ambiguos_marcados, os suportes positivos são 68 para intenção de autolesão, 68 para ilícitos violentos e 78 para assédio com ameaça. A marcação de ambiguidade não abrange todo o conjunto.

A seleção dirigida não representa a prevalência de conteúdo nocivo na aplicação. O resultado por categoria deve apresentar precisão, recall, F1 e suporte. A comparação por origem deve distinguir textos sintéticos de textos não sintéticos.

## Convenção dos rótulos

As colunas de categoria usam apenas 0 e 1. A conversão de valores nulos para 0 não amplia a cobertura de anotação. O cálculo das métricas considera apenas as categorias presentes em annotated_categories.

## Limitações de anotação

Algumas ofertas de armas dependem de contexto para caracterizar ilicitude. Relatos passados de autolesão podem diferir de intenção atual. Ironia e hipérbole podem alterar a interpretação.

Textos com pendência explícita de revisão não integram os splits de avaliação. A ausência de pendência não equivale a adjudicação independente de todo o conjunto.
