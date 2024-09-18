# Configurando um Banco de Dados SQL no Azure

Este guia irá te ajudar a configurar uma instância de banco de dados no **Azure SQL Database**.

---

## 1. Acessando o Portal do Azure

Acesse o [Portal do Azure](https://portal.azure.com). No painel principal, pesquise por **"SQL Database"** na barra de pesquisa no topo da página. Nos resultados, selecione a opção **"Banco de Dados SQL"** ou **"SQL Database"**. Em seguida, clique em **"+ Criar"** para entrar na guia de configuração do banco de dados.

---

## 2. Informações Básicas

- **Nome do Banco de Dados**: Escolha um nome para identificar seu banco de dados.
- **Assinatura**: Selecione a assinatura do Azure que deseja utilizar. Caso esteja testando, utilize a assinatura gratuita, caso disponível.
- **Grupo de Recursos**: Selecione um grupo de recursos já existente ou crie um novo. Os grupos de recursos ajudam a organizar seus recursos no Azure.
- **Servidor**: Você pode escolher um servidor existente ou criar um novo:
  - **Nome do Servidor**: Escolha um nome exclusivo para seu servidor SQL.
  - **Localização**: Selecione a região mais próxima para hospedar o servidor.
  - **Login de Administrador**: Insira um nome de usuário para o administrador do servidor.
  - **Senha**: Crie uma senha forte para o login do administrador.

---

## 3. Plano de Serviço

Escolha o plano de serviço que melhor atenda às suas necessidades. 

- **Camadas de Serviço**:
  - **Basic**: Ideal para bancos de dados pequenos e uso leve.
  - **Standard**: Equilibrado para cargas de trabalho moderadas.
  - **Premium**: Para bancos de dados críticos com altas exigências de desempenho.
  - **Hiperescala**: Para bancos de dados extremamente grandes que precisam de escalabilidade rápida.
  
  Você pode escolher entre o modelo de consumo baseado em **DTUs** (medição de desempenho em unidades de transações de dados) ou **VCore** (núcleos virtuais), dependendo da previsibilidade de sua carga de trabalho.

---

## 4. Rede

Agora você precisará configurar como o banco de dados será acessado:

- **Método de Conexão**:
  - **Ponto de Extremidade Público**: Permite conexões de fora do Azure (acesso via internet).
  - **Ponto de Extremidade Privado**: Restringe o acesso apenas à sua rede virtual no Azure.
  
- **Firewall do Servidor**: 
  - **Adicionar IP**: Clique em **"Adicionar meu IP atual"** para permitir que seu endereço IP tenha acesso ao banco de dados.
  - **Regras de Firewall**: Adicione outros IPs ou configure regras para permitir ou restringir o acesso conforme necessário.

---

## 5. Segurança

É crucial garantir que seu banco de dados esteja seguro. Aqui estão as principais opções de segurança:

- **Autenticação do Azure Active Directory (AAD)**: Integre com o Azure AD para gerenciar quem pode acessar o banco de dados.
- **Azure Defender for SQL**: Habilite para detecção avançada de ameaças e proteção contra atividades suspeitas no banco de dados.
- **Auditoria e Monitoramento**: Ative auditoria para registrar o acesso ao banco de dados e acompanhar o uso e mudanças feitas nele.

---

## 6. Backup e Redundância de Dados

Configure as opções de backup para proteger seus dados:

- **Backup Geo-Redundante**: Habilite esta opção para garantir que backups do banco de dados sejam replicados em diferentes regiões geográficas. Isso oferece maior resiliência em casos de falhas regionais.
- **Redundância Local**: Para backups dentro da mesma região, garantindo recuperação em caso de falhas locais.

---

## 7. Revisar e Criar

Agora que todas as configurações foram feitas, clique em **"Revisar e Criar"**. Revise cuidadosamente todos os detalhes, como nome do banco de dados, servidor, plano de serviço e configurações de segurança. Se tudo estiver correto, clique em **"Criar"** e aguarde enquanto o Azure provisiona sua instância de banco de dados. Esse processo pode levar alguns minutos.
