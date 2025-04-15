# Trabalho-Atividade-Teste-Caixa-Branca-e-Caixa-Preta

"Este trabalho tem como objetivo aplicar testes do tipo Caixa Branca e Caixa Preta no projeto disponível em https://github.com/cleberleao/oficina-spring-boot, além de documentar os testes diretamente no repositório."

Os objetivos do trabalho eram:

1-Fazer testes de caixa preta e identificar quais são os problemas existentes no cadastro de usuário

2-Fazer testes de caixa branca para as classes ("Service") do projeto.

Nesse trabalho fomos apresentados ao:
Teste de Caixa Branca: é uma técnica de teste de software que analisa o código fonte e a estrutura interna de um aplicativo. O objetivo é garantir que o software funcione corretamente.
Teste de Caixa Preta: é uma metodologia de teste de software que avalia a funcionalidade de um aplicativo sem conhecer a sua estrutura interna. É também conhecido como teste funcional.

Entre as varias partes desse trabalho posso destacar a reestruturaçao de codigo usando o *IntelliJ*:
![image](https://github.com/user-attachments/assets/2b7bb752-0982-403c-9e09-67a95146d5ee)

outra ferramenta que serviu pra testar a funçao adicionar o usuario foi o site disponibilizado pelo professor: Swagger Ui, nele nos tivemos  acesso as opçoes de adicionar o usuario com email, id, email e senha. Osite só iria fucnionar caso os alunos reestruturassem o codigo realizando assim uma conecxao com o servidor do site.

*IMAGEM DO SITE COM O CODIGO ORIGINAL(Navegador OperaGX):*
![image](https://github.com/user-attachments/assets/dd72e011-add8-40ac-89f7-1866c729fa8e)

*CODIGO CORRETO E FUNCIONANDO:*
![image](https://github.com/user-attachments/assets/2ff0133a-2e14-4aab-94bf-7051ec7d93ab)

*IMAGEM DO SITE APOS A EXECUÇAO DO CODIGO:*
![image](https://github.com/user-attachments/assets/c277f457-ee0f-43d0-bfec-c94ee2a6c208)

Como dito anteriormente, nesse site os alunos tiveram wue ultilizar as opçoes de /auth/user(POST) para criar um usuario como mostra a imagem a baixo:
![image](https://github.com/user-attachments/assets/d7525c4e-d7d6-448b-8f37-d05677516a62)

Alterando a parte de AutentificacaoViaTokenFilter.java no codigo foi possivel adicionar um Token na pagina disponibilizada que é representado por:

![image](https://github.com/user-attachments/assets/4b062930-6661-4d5b-a98f-9a03fbb80079)

Alterando a parte de SwaggerConfiguration que estava originalmente codificada errada propositalmente foi possivel alterar e adicionar o usuario no site disponibilizado e conecta-lo ao banco de dados do professor.

MENSAGEM DE (OK) DO SITE DIZENDO QUE FOI POSSIVEL "UPAR" O USUARIO:
 ![image](https://github.com/user-attachments/assets/f2d8743d-2a50-46b7-89b3-3ed787ab8602)

Para vizualizar o banco de dados foi usado a ferramenta DBeaver, que junto das informaçoes disponibilizadas pelo professor sobre o banco de dados (url: cleberleao.com, usuario: cleberleao_oficina, senha: mysql123oficina, nome da instancia: cleberleao_oficina) foi possivel estabelecer a conecxao com o banco podendo vizualizar o usuario como mostra a imagem:
![image](https://github.com/user-attachments/assets/c0b1fab6-5950-4137-8e97-75407abb8595)
