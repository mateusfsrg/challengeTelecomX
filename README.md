# 📊 Análise de Evasão de Clientes (Churn)

---

## 1. Introdução

Nesta análise, o **objetivo principal** foi investigar o fenômeno da *evasão de clientes* (**Churn**) e identificar os principais fatores que levam ao cancelamento do serviço.  
A compreensão desses fatores é crucial para que a empresa possa desenvolver **estratégias de retenção eficazes** e reduzir perdas financeiras.

O dataset utilizado contém informações detalhadas sobre a base de clientes, incluindo:

- Dados demográficos
- Serviços contratados
- Faturamento
- Status de evasão de cada cliente

---

## 2. Limpeza e Tratamento de Dados

Antes da análise, o dataset passou por um processo de **limpeza e tratamento** para garantir a qualidade dos dados.

**Principais passos realizados:**
1. **Achatamento das colunas aninhadas**  
   - Colunas como `customer`, `phone`, `internet` e `account` continham dados em formato de dicionário e foram "achatadas" em colunas individuais.

2. **Padronização da coluna Churn**  
   - Valores vazios (`''`) foram substituídos por `Unknown` para garantir consistência.

3. **Criação de `Contas_Diarias`**  
   - Nova coluna para visão mais granular dos gastos dos clientes ao longo do tempo.

> 📊 **Visualização:** A distribuição de clientes por status de evasão foi mostrada em um gráfico de barras, exibindo a proporção de clientes que **permaneceram**, **evadiram** ou tiveram **status desconhecido**.

---

## 3. Análise Exploratória e Recomendações

A análise exploratória revelou **padrões significativos** associados à evasão.  
Abaixo, os principais insights e recomendações:

### 🔹 Evasão por Tipo de Contrato
- Clientes com contratos **"Mês a Mês"** apresentam taxa de evasão **significativamente maior**.

**Recomendação:**  
> Criar campanhas de incentivo para migração para contratos de maior duração, oferecendo **descontos** ou **benefícios exclusivos**.

---

### 🔹 Evasão por Tempo de Contrato (*tenure*)
- A maioria dos clientes que evadem são **novos**, com tempo de serviço consideravelmente menor.

**Recomendação:**  
> Focar em ações de **onboarding** e suporte nos primeiros meses.  
> Implementar programas de acompanhamento e ofertas exclusivas para novos clientes.

---

### 🔹 Evasão por Faturamento Mensal
- Clientes que pagam contas mais altas têm **maior tendência** a cancelar.

**Recomendação:**  
> Avaliar a **competitividade** dos planos de maior valor.  
> Oferecer pacotes de benefícios adicionais ou descontos para clientes de alto custo.

---

## 4. Conclusões e Insights
  Temos 25.7% de clientes em evasão de acordo com o nosso levantamento, sendo o sue gênero irrelevante para dizer se eles se mantém conosco ou não acabamos focando em outros fatores. Chama a atenção o número de contratos do tipo **MENSAL** que perdemos sendo a sua grande maioria da fatia desses contratos que apesar de ser a maioria de nossos clientes se tornou um potencial problema por conta da sua evasão.
  <br>
<div align="center">
  <a href="https://raw.githubusercontent.com/mateusfsrg/challengeTelecomX/refs/heads/main/imagens/1.png" target="_blank">
  <img src="https://raw.githubusercontent.com/mateusfsrg/challengeTelecomX/refs/heads/main/imagens/1.png" 
       alt="Gráfico de Distribuição de Clientes" 
       width="500">
</a>
</div>
<br>
<div align="center">
  <a href="https://raw.githubusercontent.com/mateusfsrg/challengeTelecomX/refs/heads/main/imagens/3tipocontrato.png" target="_blank">
  <img src="https://raw.githubusercontent.com/mateusfsrg/challengeTelecomX/refs/heads/main/imagens/3tipocontrato.png" 
       alt="Evasão por Tipo de Contrato" 
       width="500">
</a>
</div>
<br>

  Um ponto de atenção é a evasão de clientes que realizaram transferência eletrônica que no caso é nomeado de e-check ou Eletronic Check. como vamos ver no gráfico todos os tipos de pagamentos são equivalentes em sua quantidade de permanência do nosso serviço, porém em sua grande maioria a evasão vem do pagamento citado acima, o que pode nos dar um alerta para efetuar alguma ação e entender as motivações dessa evasão. 

  <br>
<div align="center">
  <a href="https://raw.githubusercontent.com/mateusfsrg/challengeTelecomX/refs/heads/main/imagens/4metodopaga.png" target="_blank">
  <img src="https://raw.githubusercontent.com/mateusfsrg/challengeTelecomX/refs/heads/main/imagens/4metodopaga.png" 
       alt="Evasão por Método de Pagamento" 
       width="500">
</a>
</div>
<br>
  Outro dado levantado é a evasão pela quantidade de tempo que o cliente tem a assinatura e tivemos outro dado curioso. Em sua grande maioria nossa evasão vem nos primeiros meses de uso, além de notar um crescente aumento recente nesses mesmo tipo de cliente. Uma notícia boa é a quantidade que não evadiu em um processo de contrato de longo prazo. Tendo uma curva crescente de quantidade de usuários conforme a fidelidade em meses aumenta, podendo ser um indicativo de se realizar alguma ação nesse ponto. 

<br>
<br>
<div align="center">
  <a href="https://raw.githubusercontent.com/mateusfsrg/challengeTelecomX/refs/heads/main/imagens/5tempocontrato.png" target="_blank">
  <img src="https://raw.githubusercontent.com/mateusfsrg/challengeTelecomX/refs/heads/main/imagens/5tempocontrato.png" 
       alt="Distribuição de tempo de contrato(tenure) por Evasão" 
       width="700">
</a>
</div>
<br>




  

## ✅ Conclusão

Com este relatório, a análise está **consolidada** e as visualizações sustentam as **conclusões e recomendações** apresentadas.
