#  Análise de Churn - Telecom

Este projeto tem como objetivo identificar padrões que influenciam o cancelamento de clientes (churn) em uma empresa de telecomunicações. A análise foi realizada com Python e Jupyter Notebook, utilizando bibliotecas como `pandas`, `numpy`, `seaborn`, `matplotlib`, `plotly`, `scipy` e `scikit-learn`. 
---
##  Etapas da Análise

### 1️⃣ Leitura da Base
- Arquivo: `CHURN_TELECON_MOD08_V2_TAREFA_MOD15.csv`
- Leitura com `pandas`
- Verificação de tipos de variáveis e valores nulos

### 2️⃣ Análise Univariada
- Estatísticas descritivas com `describe()`
- Detecção de outliers com `zscore`
- Gráficos exploratórios:
  - `MonthlyCharges` vs `Churn`
  - `tenure`
  - `Contract`
  - `InternetService`
  - Verificação de balanceamento em variáveis booleanas

### 3️⃣ Tratamento de colunas com churn
Identificar e tratar as colunas com Churn
Identificar colunas com outliers e tratar como convém para preservar o DataFrame , sem comprometer a amostra
Uso do método apropriado para suavização dos outliers com o z-score nas colunas numéricas de Datframe: Pagamento_Mensal, Total_Pago, Tempo_como_Cliente, Qtd_Servicos ,  deixando as colunas  livres de valores extremos que poderiam distorcer análises estatísticas ou modelos preditivos
---
## 4️⃣ Análise Bivariada

 Gráficos revelam padrões  usados para prever churn , segmentar clientes e criar estratégias
As 10 variáveis mais importantes para prever o Churn usando o modelo RandomForest.
---
## #Salvando o arquivo analizado e tratado
df_tratado.to_csv('CHURN_TELECON_MOD15_ANALIZADO.csv', index=False)

---
## Tecnologias Utilizadas

Ambientes de desenvolvimento : Jupyter Notebook 
Linguagem de programação: PyThon 3.x

## Instalação das Dependências

**Versões utilizadas em setembro de 2025. Podem ser ajustadas conforme atualizações futuras**

Para garantir que o projeto funcione corretamente, instale as bibliotecas listadas no arquivo requirements.txt.
Se estiver usando o Jupyter, execute este comando em uma célula: **%pip install -r requirements.txt**.
Esse **%pip** é um comando que funciona dentro do Jupyter e faz exatamente o mesmo que no terminal.**
**Instala todas as bibliotecas com as versões mínimas definidas:**  
Os sinais **>=**  instala a versão utilizada nesse projeto ou superior (versão atualizada).

pandas>=2.2.3
numpy>=2.2.4
seaborn>=0.13.2
matplotlib>=3.10.6
plotly>=6.3.0
scipy>=1.16.1
scikit-learn>=1.7.1

##  Licença
Este projeto foi desenvolvido exclusivamente para fins educacionais como parte do curso Ciência de Dados em formação pela EBAC – Escola Britânica de Artes Criativas e Tecnologia.

O conteúdo pode ser utilizado para aprendizado, estudo e referência. Não há intenção de uso comercial ou distribuição oficial.
