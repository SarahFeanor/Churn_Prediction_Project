[![Python 3.7+](https://img.shields.io/badge/python-3.7+-blue.svg)](https://www.python.org/downloads/release/python-360/) [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0) 

<sub> 📂 Projeto - Data Science - Sarah F. Rezende

# **Projeto** - **Previsão de Rotatividade de Clientes (Churn Prediction)** 

[PROJETO (COLAB)]()

Bem-vindos(as). Este repositório foi criado com o propósito de estudo. Vale ressaltar que todos os dados são exclusivamente para fins de demonstração, garantindo total privacidade e conformidade ética.

<p align="center">
  <a href="https://github.com/SarahFeanor?tab=repositories">
    <img src="https://cdn.discordapp.com/attachments/1063559719291199599/1202653476228960306/download.jpg?ex=65ce3d54&is=65bbc854&hm=7c1cf49f358872342bf602e94c3ec8c85c0013939848c33a5d8da859ced3e92e&" alt="capa" width="600" height="300">
  </a>
</p> <p align="center"> <sup> Previsão de Rotatividade de Clientes — Foto de Imagge </sup> </p>

## **Churn Prediction (Previsão de Rotatividade de Clientes)**

A **Churn Prediction**, também conhecida como previsão de rotatividade de clientes, é uma técnica que utiliza análise de dados para antecipar quais **clientes** têm **maior probabilidade** de **cancelar** um **serviço** ou **deixar de adquirir um produto**. Essa abordagem é extensamente empregada por empresas de diversos setores, como telecomunicações, varejo, serviços financeiros e tecnologia. Seu objetivo é evitar a perda de clientes, bem como aprimorar a satisfação e a fidelização dos mesmos.

A previsão de churn é de extrema importância, visto que a rotatividade de clientes pode acarretar diversos prejuízos para uma empresa. Esses impactos podem incluir diminuição das receitas, redução da parcela de mercado e aumento dos custos relacionados à aquisição de novos clientes. Adicionalmente, a perda de clientes pode servir como um indicativo de problemas nos processos de atendimento ao cliente ou nos produtos ofertados. Essas questões podem ser endereçadas e resolvidas para melhorar a qualidade global da empresa.

A aplicação da previsão de churn possibilita que as empresas identifiquem os clientes com maior probabilidade de deixar de fazer negócios com elas. Isso, por sua vez, permite a adoção de estratégias direcionadas para reter esses clientes, o que pode envolver a oferta de benefícios especiais, promoções ou melhorias nos produtos e serviços oferecidos. Dessa forma, a previsão de churn não somente contribui para a manutenção de receitas e a ampliação da base de clientes, mas também auxilia na construção de um relacionamento mais duradouro e satisfatório com os consumidores.

## **Origem dos Dados**

Os dados utilizados neste projeto foram originalmente disponibilizados na plataforma educacional da [IBM Developer](https://developer.ibm.com/technologies/data-science/patterns/predict-customer-churn-using-watson-studio-and-jupyter-notebooks/#). Esses dados representam um cenário típico em uma empresa de telecomunicações. O conjunto de dados completo está acessível [aqui](https://raw.githubusercontent.com/carlosfab/dsnp2/master/datasets/WA_Fn-UseC_-Telco-Customer-Churn.csv).

## **Conclusão**

Com base nas análises realizadas, podemos concluir que a escolha do modelo de classificação, o pré-processamento dos dados e a técnica de balanceamento de classes são fundamentais para obter um bom desempenho na resolução do problema de Churn.

Observou-se um desempenho consistente tanto no conjunto de testes quanto no conjunto de validação. A técnica de balanceamento de classes por meio de undersampling foi aplicada, removendo apenas dados da classe majoritária. A métrica de recall foi escolhida como prioridade, uma vez que prever o cancelamento de clientes permite à empresa intervir e retê-los. Nesse contexto, prever um cancelamento incorretamente possui menos impacto do que não prever um cancelamento real. Os classificadores de Regressão Logística e SVM se destacaram nesse cenário. Para evitar overfitting, utilizou-se a validação cruzada com a técnica 5x2 CV, recomendada pela literatura.

Entre os algoritmos de machine learning testados, o SVM alcançou a maior métrica de recall, atingindo 0.81 no conjunto de teste balanceado e 0.77 no conjunto de teste desbalanceado. No entanto, o Logistic Regression também apresentou resultados semelhantes e satisfatórios. Além disso, foi possível observar a importância do pré-processamento de dados, incluindo a transformação de variáveis categóricas usando o label encoder e a criação de variáveis dummy. A padronização também se mostrou essencial para se obter um modelo com desempenho eficaz.

Em resumo, a combinação de técnicas de pré-processamento, balanceamento de classes e a escolha adequada de métricas e algoritmos permitiu a construção de modelos de machine learning capazes de prever o cancelamento de clientes com desempenho satisfatório, o que pode ser extremamente valioso para as empresas que desejam reter seus clientes e melhorar sua eficiência operacional.


