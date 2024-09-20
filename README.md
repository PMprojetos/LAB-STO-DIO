# Armazenamento - Lab

## Storage Accounts

### 1. Subscription
Para este laboratório, foi selecionada uma assinatura já existente na conta do Azure.

### 2. Resource Group
Um **Resource Group** dedicado ao laboratório foi criado para organizar os recursos de armazenamento.

### 3. Region
Escolhemos uma região próxima para reduzir a latência e otimizar o desempenho, considerando que se trata de um ambiente de laboratório.

### 4. Primary Service
O **Primary Service** configurado foi o **Blob Storage**, por ser o mais adequado para armazenar grandes volumes de dados não estruturados no laboratório.

---

## Nível de performance

### 1. Standard vs Premium
- **Standard**:
  - Modelo de pagamento conforme o uso.
  - Apresenta desempenho mais lento em comparação com a camada Premium.
  
- **Premium**:
  - Paga por toda a camada de alocação, independentemente do uso.
  - Oferece desempenho mais rápido, sendo indicado para cenários críticos.

Neste laboratório, optamos pelo nível **Standard**, pois a performance extrema da Premium não é necessária para este ambiente de testes.

---

## Redundancy

Para este laboratório, selecionamos o modelo **LRS (Locally Redundant Storage)**. Embora o LRS forneça redundância dentro de um único datacenter, sabemos que ele não é recomendado para cenários de produção, onde opções como **GRS (Geo-Redundant Storage)** ou **ZRS (Zone-Redundant Storage)** seriam mais adequadas para maior resiliência.

---

## Security

A configuração de **Security** foi mantida nas definições **Default**, já que o foco era explorar funcionalidades básicas. Em cenários reais, seria importante realizar ajustes avançados de segurança, como criptografia personalizada e controle de acesso mais restrito.

---

## Armazenamento de Blobs

### 1. Camada de Acesso
Optamos pela **camada quente (hot tier)** para os Blobs, ideal para dados acessados frequentemente, garantindo melhor custo-benefício para este tipo de uso no laboratório.

---

## Proteção de Dados

Durante o laboratório, desabilitamos a opção de **excluir Blobs automaticamente após 7 dias**, garantindo que os dados persistam para exploração posterior. Se tivesse sido habilitada, a exclusão seria irreversível e não poderia ser modificada após a criação.

---

## Migrações para o Azure

O laboratório também permitiu uma visão prática sobre os mecanismos de migração para o Azure. Exploramos cenários simulados de movimentação de dados, compreendendo como é possível integrar soluções on-premises com a nuvem através de diferentes métodos de migração, como o uso de **Azure Migrate**, **AzCopy**, e dispositivos como o **Data Box**.
