 Trabalhando com Machine Learning
Criando modelo de previsão - Passo a passo

Para trabalhar no machine learn é essencial que você possua um workspace e esta é a tarefa inicial, criar o seu workspace para assim poder criar o seu trabalho automatizado.

Depois que nosso worlspace estiver pronto temos que entrar no ML studio para criar um "novo trabalho de ML automatizado", seguindo o passo a passo da documentação do Learning para melhor entendimento e para que tudo dê certo: 

![Alt text](image-18.png)

Vamos criar um aprendizado de maquina para a previsão de aluguel de bicicletas:

![Alt text](image-17.png)


O tipo de tarefa é regressão e onome de ativo de dados e aluguel de bicicletas, com fonte de dados da WEB. 


![Alt text](image-16.png)


![Alt text](image-15.png)


![Alt text](image-14.png)


Adocumentação do Learning é bem didática e traz todos os valores e configurações para que o trabalho automatizado seja criado: 

![Alt text](image-13.png)

![Alt text](image-12.png)

![Alt text](image-11.png)

![Alt text](image-10.png)

![Alt text](image-9.png)


![Alt text](image-8.png)


![Alt text](image-7.png)





Chegando na opção "examinar" basta enviar o seu trabalho de treinamento: 

![Alt text](image-6.png)














Após envio seu trabalho irá passar pelo proxesso de configuração das execuções e após 15, podendo o tempo ser menor, estará concluído: 

![Alt text](image-5.png)

![Alt text](image-4.png)







Pipeline com as etapas do processo de aprendizado e os testes realizados 
![Alt text](image-3.png)


Teste do modelo



Na página do modelo, cliquei na aba "Pontos de extremidade". Também é possível acessar pelo menu lateral em "Pontos de extremidade". Cliquei no ponto correspondente ao modelo gerado. Em seguida, acessei a aba "Testar".

Para o teste, utilizei o json abaixo:


![Alt text](image-2.png)



A previsão gerada foi: 361.95

![Alt text](image-1.png)


