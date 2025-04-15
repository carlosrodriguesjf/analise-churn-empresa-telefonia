# TÍTULO DO PROJETO

## 👤 Autor e Contato
- **Nome**: Carlos Rodrigues
- **E-mail**: carlosrodriguesjf@gmail.com
- **LinkedIn**: www.linkedin.com/in/carlosrodriguesjf
- **GitHub**: https://github.com/carlosrodriguesjf/

## 📌 Descrição
A retenção de clientes é um dos desafios mais críticos para empresas que operam em mercados competitivos. O churn, ou taxa de cancelamento de clientes, representa a proporção de clientes que deixam de utilizar um serviço dentro de um determinado período. Compreender os fatores que influenciam o churn é essencial para que as empresas desenvolvam estratégias eficazes de retenção, reduzindo perdas e maximizando a receita.

Neste projeto, realizaremos uma análise detalhada do comportamento dos clientes com base em um conjunto de dados contendo informações como idade, tempo de contrato, frequência de uso, total gasto, interações com o call center e outras variáveis relevantes. O objetivo é identificar padrões que diferenciam clientes que permanecem dos que cancelam, permitindo a criação de estratégias para minimizar o churn.


## 🔍 Considerações Iniciais
A base de dados cancelamentos.csv foi adquirida através de uma uma aula gratuita da Hashtag Treinamentos. Para facilitar o nosso trabalho, crie o dicionário de dados abaixo:

**Dicionário de dados** para a sua tabela:  

| Nome da Variável            | Tipo       | Descrição |
|-----------------------------|-----------|-----------|
| **CustomerID**              | Inteiro    | Identificação única do cliente. |
| **idade**                   | Inteiro    | Idade do cliente (em anos). |
| **sexo**                    | Categórico | Gênero do cliente (ex.: "M" para masculino, "F" para feminino). |
| **tempo_como_cliente**       | Inteiro    | Tempo total (em meses) que o cliente está com a empresa. |
| **frequencia_uso**           | Numérico   | Frequência média de uso do serviço pelo cliente. |
| **ligacoes_callcenter**      | Inteiro    | Número de ligações realizadas para o call center. |
| **dias_atraso**             | Inteiro    | Número de dias que o cliente já atrasou pagamentos. |
| **assinatura**               | Categórico | Tipo de plano/assinatura do cliente (ex.: "Pré-pago", "Pós-pago", "Controle"). |
| **duracao_contrato**         | Inteiro    | Duração total do contrato do cliente (em meses). |
| **total_gasto**              | Numérico   | Valor total gasto pelo cliente durante o período com a empresa. |
| **meses_ultima_interacao**   | Inteiro    | Tempo (em meses) desde a última interação do cliente com a empresa. |
| **cancelou**                 | Binário    | Indica se o cliente cancelou o serviço (1 = Sim, 0 = Não). |

## 🎯 Objetivos

Por meio de estatísticas descritivas, visualizações de dados e modelagem preditiva, buscamos responder às seguintes perguntas-chave:
- Quais características dos clientes estão mais associadas ao churn?
- Clientes com maior tempo de contrato têm menor probabilidade de cancelar?
- Qual o impacto das interações com o call center na retenção?
- O valor total gasto influencia a decisão de cancelar o serviço?
- Ao final da análise, apresentaremos insights e recomendações práticas para reduzir o churn e melhorar a experiência do cliente.


## 📂 Estrutura do Projeto
```
📁 analise-churn-empresa-telefonia
│── 📂 dados                  # Conjunto de dados brutos e processados
│── 📂 relatórios             # Relatórios e visualizações geradas
│── 📂 scripts                # Scripts de automação e pré-processamento
│── README.md                 # Documentação do projeto
│── requirements.txt          # Dependências do projeto
```


## 🛠️ Tecnologias e Ferramentas
- **Python**
- **Pandas**
- **Plotly**
- **Jupyter Notebook**



## 🚀 Como Executar o Projeto
1. Clone este repositório:
   ```bash
   git clone https://github.com/carlosrodriguesjf/analise-churn-empresa-telefonia
   cd analise_cancelamento
   ```
2. Crie um ambiente virtual e instale as dependências:
   ```bash
   python -m venv venv
   source venv/bin/activate  # No Windows: venv\Scripts\activate
   pip install -r requirements.txt
   ```
3. Execute os notebooks ou scripts:
   ```bash
   jupyter notebook
   ```
4. Para executar a automação via Selenium:
   ```bash
   python scripts/analise-de-churn.ipynb
   ```

## 📈 Resultados e Insights
- **Principais motivos de cancelamento**: [Descreva]
- **Distribuição por campus e curso**: [Descreva]
- **Correlação entre ingresso e evasão**: [Descreva]
- **Evolução ao longo dos anos**: [Descreva]

## 🔮 Objetivos Futuros
- **Melhoria na coleta de dados**: [Explique melhorias planejadas na obtenção dos dados]
- **Automatização de análises**: [Descreva melhorias para tornar o processo mais eficiente]
- **Expansão da base de dados**: [Incluir mais períodos, cursos ou fatores]
- **Publicação dos resultados**: [Compartilhar insights em artigos ou dashboards interativos]


