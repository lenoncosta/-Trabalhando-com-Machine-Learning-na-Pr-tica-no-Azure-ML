Para trabalhar no machine learn é essencial que você possua um workspace e esta é a tarefa inicial, criar o seu workspace para assim poder criar o seu trabalho automatizado.

Depois que nosso worlspace estiver pronto temos que entrar no ML studio para criar um "novo trabalho de ML automatizado", seguindo o passo a passo da documentação do Learning para melhor entendimento e para que tudo dê certo: 

![Screenshot_1](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/7308b899-dfd5-435f-be25-7aac8a150a5d)


O tipo de tarefa é regressão e onome de ativo de dados e aluguel de bicicletas, com fonte de dados da WEB. 

![Screenshot_2](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/c4ad5fc0-7750-484f-ab1b-ea5ee9b1ded4)


Vamos criar um aprendizado de maquina para a previsão de aluguel de bicicletas:

![Screenshot_3](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/2f9c754c-e0ab-4065-b7b2-5520453b858a)


Adocumentação do Learning é bem didática e traz todos os valores e configurações para que o trabalho automatizado seja criado: 
![Screenshot_4](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/a522adc4-2bed-49e9-a130-113041f43938)
![Screenshot_5](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/791bffc6-2312-4207-bdaa-045d14b5729f)
![Screenshot_6](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/a371cd65-0c21-4456-9ff2-7f0365e6fa1e)
![Screenshot_7](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/55c269b1-d5d0-4075-beb3-39f469d9f6ea)
![Screenshot_8](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/c03d4765-d630-4432-8b84-1ff1f01d84cd)
![Screenshot_9](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/4dcd0dbf-4ed2-4428-8d47-659d62d6ec23)

Chegando na opção "examinar" basta enviar o seu trabalho de treinamento:

![Screenshot_10](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/82349b80-b11b-4463-bbc9-4b9ed0668cf0)
![Screenshot_11](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/127d7b8e-8922-4ce0-9d75-b7901935595d)
![Screenshot_12](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/30243641-9a95-470c-be36-7cfeaf4632fa)
![Screenshot_13](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/4fee0864-2db9-4f35-91a2-e9607366e141)


Após envio seu trabalho irá passar pelo proxesso de configuração das execuções e após 15, podendo o tempo ser menor, estará concluído: 


![Screenshot_14](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/7d48cb8a-839d-476a-9886-5ff69eb9a4e9)
![Screenshot_15](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/a52db6bf-122f-4dd1-98f5-6de9003deea5)

Na página do modelo, cliquei na aba "Pontos de extremidade". Também é possível acessar pelo menu lateral em "Pontos de extremidade". Cliquei no ponto correspondente ao modelo gerado. Em seguida, acessei a aba "Testar".

Para o teste, utilizei o json abaixo:
{
  "input_data": {
    "data": [
       {
         "day": 1,
         "mnth": 1,   
         "year": 2022,
         "season": 2,
         "holiday": 0,
         "weekday": 1,
         "workingday": 1,
         "weathersit": 2, 
         "temp": 0.3, 
         "atemp": 0.3,
         "hum": 0.3,
         "windspeed": 0.3 
       }
     ]
  }
}

A previsão gerada foi: 361.95

![Screenshot_16](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/e4a35386-877f-4a8f-a8e8-77a0a95601ca)
![Screenshot_17](https://github.com/lenoncosta/-Trabalhando-com-Machine-Learning-na-Pr-tica-no-Azure-ML/assets/44075745/c85d7c8a-c056-4dc6-bdbf-5e5069b9dec4)
