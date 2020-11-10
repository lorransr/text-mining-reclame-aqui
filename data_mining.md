---
marp: true
theme: uncover
_class: invert
_backgroundColor: DarkSlateBlue
---
<!-- 
header: 'IME - Instituto Militar de Engenharia'
footer: 'Apresentação: Lorran Santos Rodrigues | Email: lorran.rodr@gmail.com | Professor: Dr. Marcos dos Santos' 
-->

![bg left:33%](res/albert-hyseni-qq8eWIreIgg-unsplash.jpg)

##### Mineração de Dados 🎲⛏️

---
<!-- 
header: ''
footer: '' 
-->

### Sobre o Autor:
* 🎓 Formado em Engenharia Mecânica pelo CEFET-RJ
* 👨‍🔬 4 anos de experiência com apoio a decisão (Data Science)
* ✏️ Data Scientist na Eleva Educação
---
![bg](darkslateblue)
![](white)
# Objetivo Geral 🎯
---

* Elucidar os principais conceitos relacionados a mineração de dados
* Técnica de Clusterização K-Médias
* Aplicação prática em um problema de classificação

---
![bg](darkslateblue)
![](white)
# Estrutura da Aula
---
![bg](#dd6e42)
![](white)
- ## 📝 Contextualização
- ## 🎱 K-Médias
- ## 🧠 Mão na Massa
- ## ✅ Conclusão

---
![bg](darkslateblue)
![](white)
# 📝 Contextualização

---

>Informação é o petróleio do século 21, e 'analytics' é o seu motor de combustão

###### ***Peter Sondergaard, senior vice president, Gartner Research.***

---

* Explosão da quantidade de dados disponíveis
  *  coleta e disponibilidade
* submersos em dados, porém sem informação
* Necessidade de Analise em escala
---
<!-- header: '' -->
![bg](#B5D6B2)
![](white)
## O que é Mineração de Dados?

---
<!-- footer: 'Han, J., Pei, J., & Kamber, M. (2011). Data mining: concepts and techniques. Elsevier.' -->
> Extração de padrões interessantes (não triviais, implicitos, previamente desconhecidos e potencialmente úteis) ou conhecimento de porções de dados massivas
---
<!-- footer: '' -->
![bg](#B5D6B2)
![](white)
## O que **não** é Mineração de Dados?
---

* **Sistemas Especialistas**
  - Ex.: Sistema Especialista em Detecção de falhas de veículos
  - baseado na experiência
* **Buscas em Bancos** 
  * SQL

---
![bg](#dd6e42)
![](white) 
# Aplicações

---
* #### 🔐 Detecção de Fraude
* #### 👷 Detecção de Falha
* #### 👨 👩 🧓 👶  Segmentação de Clientes
* #### :chart_with_upwards_trend: Analise de Risco
* #### 📖 Mineração de Texto
...

---
![bg](#dd6e42)
![](white)
## Como Funciona a Mineração de Dados?
---
<!-- footer: 'Fig.1: Diagrama do Processo CRISP-DM para mineração de dados' -->
![w:600](res/crisp_diagram.png)

---
<!-- footer: '' -->
![bg](#dd6e42)
![](white)
## Propositos da Mineração de Dados

---
* ## Descritivo
  * Contrastar e Sumarizar caracteristicas no conjunto de dados

---
![w:900](res/cat_1.png)

---

* Associativo
  * Correlações e Causalidade
* Classificação
  * Constroi modelos que descriminam classes
---

* ## Análise de Tendências
  * regressão
  * Periodicidade, Padrão sequencial

---

## Analise de Outliers
  * Encontrar as classes que não se comportam como o esperado para maioria

---

## Análise de Clusters
  * Classes são desconhecidas
  * Maximiza similaridade intra-classes e minimiza a similiridade inter-classe 

---
![bg](darkslateblue)
![](white)
# K-Médias

---
![w:600](res/before_kmeans.png)

---
![w:600](res/after_kmeans.png)

---
![bg](#B5D6B2)
![](white)
## Como Funciona?
---
![w:500](res/intuition.png)

---
![w:600](res/step2-1.png)

---
![w:600](res/step2-2.png)

---
![w:600](res/step3-1.png)

---
![w:600](res/step3-2.png)

---
![w:600](res/step3-3.png)

---
![w:600](res/step4-1.png)

---
![w:600](res/step4-2.png)

---
![w:600](res/step5.png)


---
 $$J = \sum^k_{j=1}\sum^n_{i=1} \|x^{(j)}_i - c_j \|^2 $$

--

 $$\min J$$

---
![w:1200](res/objective_function_explained.png)

---
![w:1000](res/kmeans.gif)

---
# ⛑️ Cuidados

---
![bg](#FFFACC)
> Todos os Modelos estão **errados** mas alguns são úteis

###### **George E. P. Box**

---

* ### Dados Normalizados
  -  Distância euclidiâna é fortemente afetada pela unidade de medida

---
* ### Variavéis Categóricas

---
* ### Dependência do K
  - Decisão Subjetiva
---
![w:600](res/before_kmeans.png)

---
![w:600](res/before_kmeans_messi.png)

---
* ### Dependência do K
  - Decisão Subjetiva
  - Método do cotovelo
---
![w:700](res/elbow.png)

---
* ### Dependência do ponto de inicialização
  -  A solução encontrada é fortemente dependente dessa condição inicial
  - K-means ++

---
![bg](darkslateblue)
![](white)

# 🧠 Mão Na Massa

---

![bg](#dd6e42)
![](white)

# ✅ Conclusão
---
![bg](darkslateblue)
![](white)
# Referências

---
<style scoped>
section {
  font-size: 20px;
}
</style>

* Han, J., Pei, J., & Kamber, M. (2011). Data mining: concepts and techniques. Elsevier.

* JAIN, Anil K. Data clustering: 50 years beyond K-means. Pattern recognition letters, v. 31, n. 8, p. 651-666, 2010.

* Romesburg, Charles. Cluster analysis for researchers. Lulu. com, 2004.

* SEEJA, K. R.; ZAREAPOOR, Masoumeh. FraudMiner: A novel credit card fraud detection model based on frequent itemset mining. The Scientific World Journal, v. 2014, 2014.

* Thiprungsri, S., & Vasarhelyi, M. A. (2011). Cluster Analysis for Anomaly Detection in Accounting Data: An Audit Approach. International Journal of Digital Accounting Research, 11.
---
![bg](darkslateblue)
![](white)
# Obrigado 🚀
---

<!-- palette: #B5D6B2(green),darkslateblue,#dd6e42(orange),#FFFACC(cream) -->