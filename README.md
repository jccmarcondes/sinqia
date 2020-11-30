![Sinqia](https://www.sinqia.com.br/wp-content/themes/mziq_sinqia_insti/img/logotipo-laranja.png)





# Teste de Android Developer Sinqia

Seja bem vindo à seleção para a vaga de Android Developer da Sinqia

Este desafio é usado para avaliar os seus quesitos técnicos.



### O Desafio

Seu objetivo é criar um app com duas telas seguindo o modelo abaixo: uma que exibe uma listagem de tarefas e outra que adiciona itens nesta listagem de tarefas atráves de uma API.



### Telas



![Tarefas](https://raw.githubusercontent.com/jccmarcondes/sinqia/master/images/Tarefas.png)




![NovaTarefa](https://raw.githubusercontent.com/jccmarcondes/sinqia/master/images/NovaTarefa.png)



Temos o protótipo no Figma para visualizar melhor os componentes: [Developer/Android](https://www.figma.com/file/tj9EOuijFs5JZ3ZNNktLYD/Developer?node-id=0%3A1)



Ao acessar o link acima, clique no botão de comentário (formato de balão) para visualizar as dicas que foram deixadas em cada componente e deixe selecionado a página Android, conforme a figura abaixo

![FigmaTips](https://raw.githubusercontent.com/jccmarcondes/sinqia/master/images/FigmaTips.png)



## Consumindo o serviço de tarefas

A API que realiza a listagem e a adição das tarefas se encontra publicada neste link [aqui](https://documenter.getpostman.com/view/438724/TVmJjfHV).

> Dicas: 
>
> - Todas as palavras que contém um sublinhado são um hiperlink que ajudará de alguma forma seu desenvolvimento deste app.



Abaixo seguem algumas informações sobre como utilizar esse serviço.



Listagem das tarefas

 - **URL**:  https://9g1borgfz0.execute-api.sa-east-1.amazonaws.com/beta/task

 - **Method**: GET

 - **QueryString**: opcional

```ini
email=teste@sinqia.com.br
```

 - **Response**
   
    ```json
    {
     tasks: [
       {
         "_id": "372efad7-9c69-4753-bf9b-ee7741aaed0c",
         "description": "lorem ipsum",
         "email": "teste@sinqia.com.br",
         "when": "2020-12-15T15:41:49.074693",
         "title": "tarefa 1"
       },
       {
         "_id": "15893f63-17b4-4ef3-bc69-019fda35c339",
         "description": "lorem ipsum",
         "email": "teste@sinqia.com.br",
         "when": "2020-12-15T15:39:19.126486",
         "title": "tarefa 2"
       }
     ] 
    }
    ```





Adicionar nova tarefa

 - **URL**:  https://9g1borgfz0.execute-api.sa-east-1.amazonaws.com/beta/task

 - **Method**: POST

 - **Headers**:

   ```ini
   Content-Type: "application/json"
   ```

 - **Body**:

   ```json
   {
     "title": "tarefa 2",
     "email": "teste@sinqia.com.br",
     "description": "lorem ipsum"
   }
   ```

 - **Response**

   ```json
   {
    "success": true,
    "data": {
      "_id": "15893f63-17b4-4ef3-bc69-019fda35c339",
      "description": "lorem ipsum",
      "email": "teste@sinqia.com.br",
      "when": "2020-12-15T15:39:19.126486",
      "title": "tarefa 2"
    } 
   }
   ```



### Pré-requisitos:
 
 - [Utilizar Kotlin](https://kotlinlang.org/docs/reference/android-overview.html);
 - [Versão mínima do SDK: 21](https://developer.android.com/about/dashboards);
 - Capricho nos tratamentos e validações dos campos;
 - Tela deve ajustar em devices de resolução pequena, acima de 4 polegadas.



### Diferenciais:

 - [Android Dagger2] (https://developer.android.com/training/dependency-injection/dagger-android);
 - [Android Coroutines] (https://developer.android.com/kotlin/coroutines);
 - [Android Room] (https://developer.android.com/topic/libraries/architecture/room);
 - [Android Jetpack](https://developer.android.com/jetpack);
 
 
 
### Permitido:

 - [Utilização de bibliotecas de terceiros](https://developer.android.com/studio/build/dependencies?hl=pt-br);




### O que esperamos:

 - [Boa organização do código-fonte](https://developer.android.com/guide);
 - Boas práticas de Orientação a Objetos;
 - Tempo de entrega do app dentro do aceitável;
 - Código limpo e de fácil manutenção.





### Ao terminar o desafio:

- Caso o upload do projeto for feito no Github ou Bitbucket, envie o link para nós por e-mail: julio.costa@ext.sinqia.com.br

 
- Caso não tenha conta no Github, envie o zip do projeto para julio.costa@ext.sinqia.com.br


Desejamos uma boa sorte!!

