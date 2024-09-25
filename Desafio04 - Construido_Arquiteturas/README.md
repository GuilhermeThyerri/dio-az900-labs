# Guia de Criação e Gerenciamento de Infraestrutura no Azure

Este guia vai te ajudar a planejar, construir e gerenciar sua infraestrutura no Azure, com foco em organização, segurança e otimização.

---

## 1. Planejamento da Arquitetura

Antes de começar a criação dos recursos no Azure, o planejamento da arquitetura é essencial para garantir que a infraestrutura atenda às necessidades da sua aplicação. Considere:

- Quais **serviços do Azure** serão necessários (máquinas virtuais, bancos de dados, etc.)?
- Como os componentes da arquitetura irão se comunicar?
- Alta disponibilidade e escalabilidade serão necessárias?
- Quais são os requisitos de segurança e conformidade com regulamentos?
- Utilize o [Azure Well-Architected Framework](https://learn.microsoft.com/pt-br/azure/architecture/framework/) para guiar o planejamento e otimização da sua arquitetura.

---

## 2. Criação do Grupo de Recursos

O Grupo de Recursos no Azure é uma maneira de organizar e gerenciar todos os componentes da sua infraestrutura. Facilitando a visualização e o monitoramento dos recursos relacionados, além de melhorar a gestão de custos.

### Passos para criação:

1. No Portal do Azure, busque por "Grupos de Recursos" ou "Resource Groups".
2. Clique em "+ Criar".
3. Preencha as informações:
   - Nome do Grupo de Recursos: Escolha um nome claro e que descreva bem o propósito do grupo.
   - Região: Escolha a região mais próxima para reduzir a latência e otimizar custos.
4. Clique em "Revisar + Criar" e por fim clique em "Criar".

---

## 3. Criação da Rede Virtual

A Rede Virtual (VNet) serve para conectar os recursos internos da sua infraestrutura, permitindo a comunicação entre vários serviços.

### Como criar a Rede Virtual:

1. No Portal do Azure, busque por "Redes Virtuais" ou "Virtual Networks".
2. Clique em "+ Criar" e preencha os seguintes dados:
   - Nome da Rede Virtual: Um nome que identifique facilmente a VNet.
   - Grupo de Recursos: Selecione um grupo de recursos o qual a Vnet será alocado.
   - Região: Escolha uma região para o recurso.
   - Intervalo de Endereços IP: Defina o espaço de IP para a rede virtual.
3. Adicione uma sub-rede inicial e associe os recursos que necessitam de comunicação.
4. Clique em "Revisar + Cria" em seguida em "Criar".

Pronto, agora você tem um grupo de recursos com um recurso dentro, lembrando que pode adicionar muitos outros recursos ao grupo, como recursos de segurança entre outros.
