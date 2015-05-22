# Integração Contínua com Travis - Projeto Integrador

[![Build Status](https://travis-ci.org/CarlosTWMF/travis-example.png)](https://travis-ci.org/CarlosTWMF/travis-example)

Da instalação à construção
===========

01 - O primeiro passo é instalar e configurar o Git:

$ sudo aptitude install git-core
$ git config -- global user.name "Seu Nome"
$ git config -- global user.email "seu@email.com"


02 - Gerando uma nova chave SSH:

$ ssh-keygen -t rsa -b 4096 -C "seu@email.com"


03 - Utilize a configuração padrão quando for questionado um arquivo para salvar a chave, simplesmente pressionando Enter para continuar:

Enter file in which to save the key (/Users/you/.ssh/id_rsa): [Pressione Enter]


04 - Defina uma frase de segurança para as operações no repositório.


05 - Adicione a chave ao seu agente SSH:

$ ssh-add ~/.ssh/id_rsa


[06 - Associe a sua chave SSH à sua conta no GitHub](https://help.github.com/articles/generating-ssh-keys/#step-4-add-your-ssh-key-to-your-account)


07 - Teste a conexão:

$ ssh -T git@github.com
Digite "yes"

