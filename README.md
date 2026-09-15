# deploy_wordpress_ansible
project of deploy of wordpress using Ansible for implemetantion

# Deploy WordPress com Ansible

Projeto criado para automatizar a instalação e configuração de um ambiente WordPress, usando um banco de dados MySQL, em outro servidor, utilizando Ansible para implementação da estrtuta.

> Observação: este projeto foi desenvolvido como estudo e prática de automação com Ansible.

## Estrutura

A organização do projeto foi dividida para separar inventário, variáveis, templates e tarefas, facilitando manutenção e reutilização.

```text
deploy_wordpress_ansible/
├── inventory/          # Hosts e grupos gerenciados pelo Ansible
├── group_vars/         # Variáveis dos grupos
├── roles/
│   ├── common/         # Configurações básicas do servidor
│   ├── nginx/          # Instalação e configuração do Nginx
│   ├── php/            # Instalação e configuração do PHP
│   ├── mysql/          # Banco de dados MySQL/MariaDB
│   └── wordpress/      # Deploy e configuração do WordPress
├── templates/          # Arquivos Jinja2 utilizados nas configurações
├── files/              # Arquivos estáticos copiados para os hosts
├── playbook.yml        # Playbook principal
└── README.md
