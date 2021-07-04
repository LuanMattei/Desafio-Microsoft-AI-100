# 		Trilha engenheiro de IA- Microsoft-Testes Finais :computer:

------

**Bom dia, Boa tarde , Boa noite!!!**

**Este foi um desafio proposto pelo grupo Anima, utilizando as funcionalidades de Machine Learning e Inteligência artificial com problemas reais para testar conhecimento.** :black_heart:

## Exercício 1  Analise de dados do Enem de 2019. 

## É possível  prever a nota de ciências da natureza , caso se saiba a nota de Matemática?

Resposta: Sim , podemos prever a nota de um estudante na disciplina de ciências da natureza apenas com sua nota de matemática ,quem tira uma nota inferior a 500 em Matemática pode  tirar uma maior em Ciências da natureza e o inverso caso a nota for superior a 500.

| Nu_Nota_MT | Nu_Nota_Cn(Prevista) |
| :--------: | :------------------: |
|    100     |      272,47451       |
|    345     |      395,94522       |
|    500     |      475,62002       |
|    600     |      520,54008       |
|   752,9    |       605,2594       |
|   799,9    |      631,63247       |

#### Passo a passo :arrow_down:

1.  Utilizando o conjunto de dados dentro do Azure machine , foi adicionado nossa base de dados referente ao Enem de 2019 e enquanto a base de dados é criada , criamos uma instancia  e um cluster de computação.

2.  Cria-se um pipeline, nele adicionamos nossa base de dados.

   1.  Utilizamos a **Select Columns in Dataset**  e selecionamos as colunas Nu_NOTA_CN e NU_NOTA_MT.
   2. Utilizamos a **CLEAN MISSING DATA** e vamos limpar as colunas por inteiro da coluna  NU_NOTA_MT
   3. Utilizamos o **NORMALIZE DATA**.
   4. Enviamos o  **pipeline**.
   5. Mensagem de sucesso.:next_track_button: :happy:

3. Criação do pipeline de treinamento:arrow_down:

   1. Utilizamos a ferramenta **Split Data**.
   2. Utilizamos a ferramenta linear **regression** que avalia as variáveis linearmente.
   3. Utilizamos a ferramenta **train model** que pega 70% dos dados divididos.
   4. Utilizamos a ferramenta **Score model** que pega os 30% restantes dos dados
   5. Utilizamos a ferramenta **Evaluate model** que avalia as condições do treinamento e sua eficiência.

4. Criação do pipeline de interferência :arrow_down:

   1. Agora vemos uma nova tela.

   2. Apagamos aquela base de dados inseridas no inicio e o **Evaluate model**.

   3. Utilizamos a ferramenta de entrada de serviços Web.

   4. Utilizamos a ferramenta de Enter Data Manually e nele colocamos algumas notas para a matéria de matemática que se encontra na coluna da esquerda da Tabela superior

   5. Utilizamos a ferramenta Execute Python Script com código semelhante ao desse [tutorial](https://docs.microsoft.com/pt-br/learn/modules/create-regression-model-azure-machine-learning-designer/inference-pipeline).

      #### 																										Concluído desafio 1.

      ------

      

