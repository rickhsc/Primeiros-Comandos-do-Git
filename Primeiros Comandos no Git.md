## Primeiros Comandos no Git

Indo para nosso projeto no terminal, daremos um comando que vai “configurar” o projeto para que ele funcione com o **git**. Basta digitar o seguinte:

```
git init
```

Isso criará alguns arquivos próprios do **git**, entre eles o mais importante é o **gitignore**, pois nele está tudo o que se deve ignorar ao realizar o **commit**. É aqui onde vamos colocar diretórios e arquivos grandes, que podemos  gerar facilmente, ou arquivos que não queremos que fiquem visíveis no  repositório.

Ao usar o **git init**, provavelmente, ele irá configurar tudo corretamente, mas é sempre bom dar uma olhada e verificar que está tudo certo.

![Git Init](https://blog.cod3r.com.br/wp-content/uploads/2021/01/gitignore.png)

Após confirmar que os arquivos corretos estão no **gitignore,** vamos subir o projeto. Para isso, o primeiro comando que precisamos é o seguinte:

```
git status
```

Com ele podemos verificar quais arquivos ainda não adicionamos no  repositório local da máquina. Como mostrado na imagem abaixo, são os  arquivos marcados em vermelho:

![GitIgonre](https://blog.cod3r.com.br/wp-content/uploads/2021/01/status_vermelho.png)

Para seguirmos corretamente temos que adicionar esses arquivos ao repositório local, então vamos precisar desse comando aqui:

```
git add .
```

Esse comando fará com que todos os arquivos fiquem prontos para o  Github, por isso ele é indispensável. É importante observar que usei o **git add .** porque quero adicionar todos os arquivos do projeto, mas caso você queira adicionar apenas algum arquivo específico, basta usar **git add <nome_do_arquivo>**.

No fim desse processo, ao digitar novamente o **git status**, vamos ver o seguinte:

![Commit Git Hub](https://blog.cod3r.com.br/wp-content/uploads/2021/01/status_verde.png)

Isso significa que estamos prontos para continuar.

## Primeiro Commit

Agora faremos o primeiro **commit** do projeto. Basta utilizar o seguinte comando:

```
git commit -m "meu primeiro commit"
```

A flag **-m** indica que vamos adicionar uma mensagem para aquele **commit**. Isso é muito importante, pois dessa forma conseguiremos identificar o  que foi feito naquele commit. Por exemplo, você acabou de adicionar um  Header na aplicação, então na mensagem você sinaliza que criou o header  para a aplicação.

O próximo comando será:

```
git branch -M main
```

Aqui vamos criar a **branch main**, que é a principal  branch do repositório. Mas como falei anteriormente, você não precisa se preocupar com esse detalhe nesse tutorial.

Agora vamos linkar os 2 repositórios, ou seja, o repositório do **Github** com o da nossa máquina. Para isso, usaremos o comando:

```
git remote add origin <link_para_o_seu_repositorio>
```

O link fica disponível na página em branco do **Github** que mostrei mais acima.

Por fim, vamos enviar esse projeto com o seguinte comando:

```
git push -u origin main
```

