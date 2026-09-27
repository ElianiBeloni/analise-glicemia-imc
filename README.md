# Análise de Associação entre Glicemia e IMC

> **Contexto:** Trabalho desenvolvido para a disciplina **MD32 - Modelos Estatísticos** ministrada pelo professor Dr. Leonardo Soares Bastos no IMPA Tech.

Este repositório contém a análise estatística desenvolvida para quantificar a relação de dependência (associação) entre o nível de glicemia em jejum no sangue e o Índice de Massa Corpórea (IMC) numa amostra de 142 adultos. 

##  Objetivo do Estudo

Quantificar a associação entre o IMC e os níveis de glicemia em jejum, considerando e ajustando o modelo estatístico para variáveis demográficas, clínicas e de estilo de vida.

## Estrutura do Banco de Dados (`glicemia_h.csv`)

* **Variável Resposta (Dependente):**
  * `glicemia`: Nível de glicemia em jejum (mg/dL).
* **Variável Explicativa Principal:**
  * `imc`: Índice de Massa Corpórea ($\text{kg/m}^2$).
* **Covariáveis de Ajuste:**
  * `idade`: Idade do participante (em anos).
  * `atividade_fisica`: Tempo médio semanal de atividade física moderada (em minutos).
  * `sexo`: Sexo biológico (*Feminino* ou *Masculino*).
  * `historico_familiar`: Histórico familiar de *Diabetes Mellitus* (*Sim* ou *Não*).
  * `hipertensao`: Diagnóstico prévio de hipertensão (*Sim* ou *Não*).

## Conteúdo do Repositório

* `me.qmd`: Código-fonte em Quarto contendo a importação, análise descritiva, modelagem estatística, diagnósticos de resíduos e interpretação dos resultados.
* `me.pdf`: Relatório final completo compilado a partir do ficheiro Quarto.
* `glicemia_h.csv`: Conjunto de dados utilizado no estudo.
* `t1.qmd` / `t1.pdf`: Documento com as orientações originais do trabalho acadêmico.

##  Tecnologias e Pacotes Utilizados

* **Linguagem:** R
* **Relatórios Dinâmicos:** Quarto (`.qmd`)
* **Principais Pacotes:**
  * `tidyverse` (leitura, manipulação de dados e geração de gráficos com `ggplot2`)
  * `patchwork` (composição e arranjo dos painéis de gráficos)


##  Como Executar o Projeto

1. Certificar-se de ter o **R** e o **Quarto** instalados no seu ambiente.
2. Clona este repositório:
   ```bash
   git clone [https://github.com/SEU_USUARIO/analise-glicemia-imc.git](https://github.com/SEU_USUARIO/analise-glicemia-imc.git)
3. Abre a pasta do projeto no VS Code ou RStudio, por exemplo.
4. Renderiza o relatório executando no terminal:
   ```bash
   quarto render me.qmd --to pdf

## Créditos e Transparência

   * **Material de Apoio:** As práticas e a estrutura de código em R foram baseadas nas orientações disponibilizadas pelo professor no repositório [lsbastos/md32](https://github.com/lsbastos/md32/tree/main/praticas) .

   * **Uso de Inteligência Artificial:** Este trabalho contou com o auxílio de Inteligência Artificial Generativa como ferramenta de suporte à aprendizagem (pair programming e tutoria). A IA foi utilizada para o esclarecimento de dúvidas conceituais sobre estatística, auxílio no desenvolvimento dos códigos em R e formatação do relatório final em Quarto/Markdown.
