# Integração Contínua com Travis - Projeto Integrador

[![Build Status](https://travis-ci.org/CarlosTWMF/travis-example.png)](https://travis-ci.org/CarlosTWMF/travis-example)

Da instalação à construção
===========

GitHub
---------

01 - O primeiro passo é instalar e configurar o Git:
* $ sudo aptitude install git-core
* $ git config -- global user.name "Seu Nome"
* $ git config -- global user.email "seu@email.com"




02 - Gerando uma nova chave SSH:
* $ ssh-keygen -t rsa -b 4096 -C "seu@email.com"




03 - Utilize a configuração padrão quando for questionado um arquivo para salvar a chave, simplesmente pressionando Enter para continuar:
* Enter file in which to save the key (/Users/you/.ssh/id_rsa): [Pressione Enter]




04 - Defina uma frase de segurança para as operações no repositório.




05 - Adicione a chave ao seu agente SSH:
* $ ssh-add ~/.ssh/id_rsa




[06 - Associe a sua chave SSH à sua conta no GitHub](https://help.github.com/articles/generating-ssh-keys/#step-4-add-your-ssh-key-to-your-account)




07 - Teste a conexão:
* $ ssh -T git@github.com
* Digite "yes"




Travis
---------
01 - Autentique-se no Travis utilizando a sua conta do GitHub




02 - Permita que o Travis acompanhe as alterações do seu repositório através do seu perfil no Travis




03 - Crie um arquivo .travis.yml especificando a matriz de execução do seu projeto juntamente com as variáveis de ambiente e adicione este arquivo à raíz do seu projeto. Para mais detalhes [acesse a documentação do Travis para a construção de matrizes](http://docs.travis-ci.com/user/build-configuration/#The-Build-Matrix)




[04 - Exiba o status de Build do Travis no seu projeto do GitHub](http://stackoverflow.com/questions/19810386/showing-travis-build-status-in-github-repo)




05 - Seu projeto já está pronto para ser acompanhado. Siga as instruções a seguir para enviar os arquivos para o GitHub. Assim que você mandar os arquivos para o seu repositório já poderá visualizar o Travis trabalhando =)




Enviando o projeto para o GitHub e acompanhando o Build
---------
01 - Veja quais o status do seu repositório:
* $ git status




02 - Adicione os arquivos ao projeto:
* $ git add .




03 - Informe quais as alterações você está realizando:
* $ git commit -m "Mensagem de Informação do commit"




04 - Envie as alterações do seu projeto para o seu repositório no GitHub:
* $ git push origin master




05 - Observe o Travis funcionar =)



Fontes
---------
[GitHub](https://help.github.com/articles/generating-ssh-keys/#step-4-add-your-ssh-key-to-your-account)
[Travis](http://docs.travis-ci.com/user/build-configuration/#The-Build-Matrix)

