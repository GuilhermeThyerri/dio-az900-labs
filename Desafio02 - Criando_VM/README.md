# Guia para Criar uma VM na Azure

Guia que vai te ajudar a criar uma Virtual Machine (Máquina Virtual) dentro do portal da azure.


---
## 1 - Acessar o portal

Primeiro acesse o [Portal Azure](https://portal.azure.com/) com suas credenciais.

## 2 - Criar a VM
1. Na barra de pesquisa digite "Máquinas Virtuais" ou "Virtual Machines" e clique no resultado.
2. No canto superior esquedo da página clique em "+ Criar" para abrir a guia de criação de VMs.


## 3 - Configurações Básicas
* **Nome da VM**: Defina um nome para identificar a VM
* **Região**: Defina a região ideal para sua VM
* **Opções de disponibilidade**: Escolha a opção de disponibilidade, essa opção ajuda a sua VM a ser mais reliente.
* **Opções de zona**: Escolha entre Selecionar manualmente uma zona ou deixar que o Azure selecione para você.
* **Zona de disponibilidade**: Escolha entre a Zona 1, Zona 2 ou Zona 3, ou entao duas, ou 3 dessas zonas.
* **Tipo de segurança**: Dentre as opções temos o "Padrão" e "Computadores virtuais de inicialização confiável".
* **Imagem**: Selecione a imagem desejada, isso é o Sistema operacional da sua VM. Dentre as imagens disponíveis, temos Ubuntu Server, Windows Server, Windows 11 pro e Windows 10 pro.
* **Arquitetura de VM**: Escolha entre Arm64 e x64.
* **Tamanho da VM**: O tamanho da VM se refere a especificação tecnica dela, escolha uma de acordo com sua necessidade de trabalho.
* **Nome de Usuário e Senha**: Configure um nome de usuário e senha para acessar sua VM.
* **Porta de entrada**: Selecione a porta de entrada da sua VM. SSH para Linux e RDP para Windows.

## 4 - Configuração de disco:
* **Tamanho do disco do SO**: Selecione o tamanho do disco da VM. De 30Gb a 2Tb.
* **Tipo de disco de SO**: Selecione o tipo de disco, as opções sao HDD, SSd e SSD premium.
* **Discos de dados**: Se necessário, adicione discos adicionais.

## 5 - Configuração de Rede:
* **Rede virtual**: Crie uma nova rede ou escolha uma já existente.
* **Sub-rede**: Escolha a sub-rede a qual sua VM será conectada.
* **IP público**: Selecione o Ip público para sua VM se comunicar fora da rede virtual.
* **Grupo de segurança de rede do adaptador de rede**: Configure regras de firewall.
