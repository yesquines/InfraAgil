**Infraestrutura Ágil**
=======================

INTRODUÇÃO
----------

Esse repositório tem como objetivo armazenar alguns procedimentos comuns.

O Curso abrange ferramentas diversas e cada aula tende a conectar as ferramentas entre si.

Por isso, esses procedimentos devem ser utilizados em **caso de ausência em aula**, para que seja possivel acampanhar as aulas subsequentes sem maiores problemas.

EMENTA
------

Inicialmente na Branch **MASTER** temos os arquivos para criação da Infraestrutura do Curso.

Sendo que o Curso está dividido em **10 Aulas**. A Agenda _sugerida_ para esses 10 dias irá contemplar os seguintes assuntos:

AULA   | MATÉRIA
------ | --------------------------------------------------
Aula01 | Teoria sobre DevOPS
Aula02 | Introdução Ansible
Aula03 | Ansible - Roles
Aula04 | Introdução Puppet
Aula05 | Puppet - Modulos
Aula06 | Introdução Docker 
Aula07 | Docker - Docker Compose e DockerFile / Git-GitLab
Aula08 | Rundeck
Aula09 | Jenkins
Aula10 | BlueGreen Deployment / Introdução a AWS

PASTAS
-------

Cada PASTA é referente a uma técnologia, procedimentos, links,  ou informações da aula.

* **Ansible**: Contempla o procedimento de Instalação do Ansible e Imagem sobre as camadas de uma playbook.
* **Docker**: Contempla o procedimento de Instalação do Docker, Imagens de explicação da sua estrutura e aplicação simples para utilização em sala de aula.
* **GitLab**: Contempla o procedimento de Instalação do GitLab e Imagem de exemplo sobre GitFlow
* **Puppet**: Contempla os procedimentos de Instalação do Puppet Agent e Server e Imagens de explicação da sua estrutura.
* **Rundeck**: Contempla o procedimento de Instalação do Rudenck e Imagem de explicação da sua estrutura.
* **Jenkins**: Contempla o procedimento de Instalação do Jenkins.

VAGRANT
-------
Ferramenta para criar e gerenciar ambientes virtualizados (baseado em inumeros providers) com foco em automação.

Comandos                      | Descrição
----------------------------- |------------------
vagrant init                  | Gera o VagrantFile
vagrant box add <box>         | Baixar imagem do sistema
vagrant box status            | Verificar o status dos boxes criados
vagrant up                    | Cria/Liga as VMs baseado no VagrantFile
vagrant up --provision        | Sobe a máquina com as alterações feitas no VagrantFile
vagrant provision             | Provisiona mudanças logicas nas VMs
vagrant status                | Verifica se VM estão ativas ou não.
vagrant ssh 'vm'              | Acessa a VM
vagrant ssh 'vm' -c 'comando' | Executa comando via ssh
vagrant reload 'vm'           | Reinicia a VM
vagrant halt                  | Desliga as VMs
