# 👋💻😅 Bem-vindo(a) ao code test da Energié

A entrevista foi bem, certo? Estamos entusiasmados em recebê-lo(a) na próxima etapa - você mereceu. Agora é hora de começar a escrever algum código.

## 🐕 Rusky Vet

A Rusky Vet LTDA é a empresa número 1 em saúde canina no mundo, oferecendo soluções em saúde e bem-estar para todas as raças de cachorro.

Atualmente, a especialidade da empresa é garantir a saúde desses animais através de consultas veterinárias. Hoje o processo todo é feito por telefone e consultório, mas pedimos a sua ajuda para desenvolver uma solução tecnológica que permita que parte desse processo seja feito online.

### 🤹 Suas tarefas

* O cadastro de cachorros está incompleto. Fazer possível adicionar uma foto ao cadastro.
* A tela de agendar consultas existe, mas ao clicar em "Agendar" nada acontece. Implementar a funcionalidade de agendar consultas, e mostrar as consultas do usuário cliente.
* Mostrar todas as consultas agendadas para o usuário veterinário. Ao abrir uma consulta, o veterinário deve ser capaz de adicionar observações e salvar, marcando a consulta como finalizada automaticamente.
* No momento, o estilo do sistema não está com a cara da empresa. Os designers da Rusky Vet sugeriram algo como [este estilo de UI](https://i.ibb.co/C1WgBgV/rusky-ui-concept.png).
* Como o projeto ainda está incompleto, podem haver bugs e/ou problemas de segurança. Pedimos que conserte o que puder encontrar.

### 👉 Recomendações técnicas

Para manter as coisas simples, aqui vão algumas recomendações técnicas:

* Não é necessário adicionar nenhum tipo de dependência extra (composer ou npm).
* Ao se cadastrar um cachorro, todos os campos são obrigatórios.
* Idealmente, a tela de agendamento de consultas deve mostrar os horários disponíveis via AJAX ao selecionar uma data. Para manter o funcionamento simples, a empresa realiza somente uma consulta por hora em período comercial, exceto finais de semana. Uma vez agendada a consulta, o cliente não pode excluir nem alterar a mesma.
* Qualquer veterinário tem acesso à todas as consultas, mas fica registrado o veterinário que realizou a consulta (fazendo observações e finalizando).
* Não é necessário criar cadastro para veterinários. Contas de cliente são convertidas manualmente em contas de veterinário através do banco de dados.

### ✅ Entrega

<!-- A entrega final deve ser um [pull request](https://help.github.com/articles/creating-a-pull-request/) neste repositório, contendo na descrição quaisquer informações que achar relevante passar para a empresa e para quem vai revisar seu código.

Quando tiver finalizado, fale com a gente. -->
A entrega final deve ser um **repositório do github**, contendo na **README** quaisquer informações que achar relevante passar para a empresa e para quem vai revisar seu código. O repositório precisa ser público , e deve nos encaminhar o link para o e-mail **contato@energienutricao.com.br** com assunto: **Teste Estágio TI**

### ⏳ Tempo

Pedimos para que você trabalhe em torno de 5 horas nesse teste (sem contar qualquer necessidade de pesquisa ou setup), e que complete em até uma semana da data em que o teste foi lhe enviado. Para ser claro, não gaste uma semana inteira de trabalho nisso. Nós não queremos tomar todo o seu tempo.

Se você achar que o teste está tomando mais tempo do que o sugerido, aqui vão algumas dicas:

### Dicas importantes para não perder tempo

* Não gaste tempo procurando a melhor solução para um problema. Faça do jeito que já conhece.
* Não gaste tempo tentando entender todo o código fonte. Recomendamos que teste o sistema, faça um "scan" rápido e em seguida parta para as alterações.
* Planeje alocar um tempo para cada passo do desafio antes de iniciar, e adote uma ideia de "timeboxing". Para explicar, timeboxing é a ideia de você cronometrar suas tarefas, e se uma tarefa estiver tomando mais tempo do que o esperado inicialmente, você começa a focar em outra coisa e evita ficar estagnado em um único trecho do código.
* Priorize suas tarefas, faça o mais importante primeiro e deixe os pontos "legais de se ter" pra caso sobre tempo.
* Recomendamos que faça os commits diretamente neste repositório para evitar trabalho duplicado. Não é necessário "ensaiar" os commits em um fork ou em seu local. Commits descritivos e significativos são importantes, mas também queremos ver como você chega lá.
* Pensamos esse desafio para que você possa chegar lá com simplicidade. Lembre-se que esse é um projeto fictício. Ao mesmo tempo que é importante levar em conta situações e problemas reais no seu código, não é necessário gastar tempo com soluções muito complexas.

## 🙋 FAQ

**1. Eu tenho dúvidas sobre a solução, devo fazer deste jeito ou deste outro jeito?**

Parte da avaliação é ver como você lida com uma especificação como esta. Implemente uma solução que atenda ao problema e documente suas decisões no pull request.

**2. Não estou familiarizado com todas as tecnologias. O que fazer?**

Assumimos que você esteja familiarizado com um projeto Laravel e com JavaScript. Se você não conseguir encontrar a resposta para alguma dúvida técnica no Google, sinta-se à vontade para nos perguntar 😉.

**3. Precisarei de mais tempo, o que fazer?**

Entendemos que imprevistos podem acontecer, e se você precisar de mais um prazo, fale com a gente.

## 💻 Como executar o projeto

Faça o clone do projeto, renomeie o arquivo `.env.example` para `.env`, e altere este arquivo com as credenciais do seu banco de dados MySQL local.

Em seguida, execute os seguintes comandos na pasta raíz do projeto:

1. Para instalar as dependências do projeto:
```
composer install
```
```
npm install
```

2. Carregar o arquivo .env no cache:
```
php artisan config:cache
```

3. Para criar o banco de dados e registros de teste:
```
php artisan migrate
```
```
php artisan db:seed
```

4. Para executar o projeto:
```
php artisan serve
```

5. Em outra aba do terminal, utilize o comando:
```
npm run watch
```

O comando `watch` vai assistir a pasta do seu projeto e recarregar automaticamente o navegador em `localhost:3000` quando houver alguma alteração, além de compilar os arquivos JavaScript e SCSS para dentro de public.

Após rodar o comando `db:seed`, você será capaz de fazer o login com o usuário cliente joaodasilva@gmail.com, e com o usuário veterinário mariovet@gmail.com, ambos com senha `123123123`.
