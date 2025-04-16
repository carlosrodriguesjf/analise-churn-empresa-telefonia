# ANÁLISE DE CHURN

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
- Qual o impacto das interações com o call center nos cancelamentos?
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
**Identificamos que os clientes cancelaram seus planos de acordo com as situações abaixo:**
- Todos os clientes do plano Mensal cancelaram
- Clientes com a partir de 51 anos, cancelaram
- Clientes que realizaram, a partir de 5 ligações para o Call Center, cancelaram
- Clientes que tiveram a partir de 21 dias de atraso, cancelaram
    
**Taxas de cancelamento:**
- Taxa de cancelamento = 56,7 %
- Taxa de cancelamento excluindo os clientes do plano mensal = 46 %
- Taxa de cancelamento excluindo todos os clientes que ligaram mais de 5 vezes = 40,8 %
- Taxa de cancelamento excluindo os clientes que atrasaram o pagamento mais de 20 dias ou com idade acima de 50 anos = 46 %
- Taxa de cancelamento excluindo todos os clientes do plano mensal e que ligaram mais de 5 vezes = 30,5 %
- Taxa de cancelamento excluindo os clientes do plano mensal, os que atrasaram o pagamento mais de 20 dias e que ligaram mais de 5 vezes = 21,8 %

**Recomendação para redução do Churn:**
- Condições melhores para os planos Mensais ou exclusão desses
- Redução da necessidade de muitas ligações para o Call Center
- Acompanhamento próximo das pessoas que atrasarem o pagamento




