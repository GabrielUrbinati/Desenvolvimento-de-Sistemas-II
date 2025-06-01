# Desenvolvimento-de-Sistemas-II
Repositório para os arquivos do projeto de Desenvolvimento de Sistemas II
 
 Professor:
 Aluno: Gabriel Branco Urbinati
 RA: 10443760
 Turma: 3J
 Projeto : Sistema de Gerenciamento de Manutenção de Veículos.

# TG1 - Cenário de Negócio, Concepção do Sistema e Modelo de Caso de Uso

# INTRODUÇÃO
Sistema simples para auxiliar oficinas mecânicas a organizar atendimentos, permitindo cadastrar clientes, veículos, serviços, facilitando e registrando toda a operação.

Cenário de Negócio / Concepção
# 1.	Problema ou Oportunidade Percebida:
	As oficinas mecânicas enfrentam dificuldades na organização de atendimentos e na gestão de agendamentos, o que pode resultar em perda de clientes e ineficiência operacional.
# 2.	Justificativa para a Demanda:
	Um sistema de gerenciamento pode otimizar o fluxo de atendimentos, melhorar a comunicação com clientes e facilitar o controle de manutenções e serviços prestados.
# 3.	Descrição do Produto de Software:
	O sistema será uma plataforma que permite às oficinas mecânicas cadastrar clientes e veículos, agendar serviços e gerenciar o status das manutenções, proporcionando maior eficiência e transparência nas operações.



# 4.	Clientes e Usuários Envolvidos:
	Clientes: Proprietários de veículos que buscam serviços de manutenção.
	Usuários: Atendentes da oficina mecânica que realizam cadastros, agendamentos e atualizações.
	Impactados: O proprietários da oficina, que se beneficiarão de um sistema mais organizado e eficiente.
# 5.	Critérios de Qualidade:
	Usabilidade: O sistema deve ser fácil de usar para todos os tipos de usuários.
	Desempenho: O sistema deve responder rapidamente às solicitações.
	Escalabilidade: O sistema deve suportar a adição de novos clientes e veículos sem perda de desempenho.
	Segurança: Proteção das informações pessoais dos clientes e registros de manutenção.
________________________________________

# Casos de Uso Resumidos:

1	Atendente - Cadastrar Cliente - Sistema: Registrando informações do cliente.

2	Atendente - Cadastrar Veículo - Sistema: Associando o veículo ao cliente.

3	Atendente - Agendar Manutenção - Sistema: Planejando data e horário do serviço.

4	Atendente - Atualizar Status do Serviço - Sistema: Mudando status da manutenção.

5	Atendente - Listar Agendamentos - Sistema: Visualizando agendamentos.

6	Atendente - Consultar Manutenção - Sistema: Acessando informações detalhadas sobre serviços.

7	Atendente - Consultar Histórico de Manutenções - Sistema: Verificando registros anteriores.

8	Atendente - Cancelar ou Reagendar - Sistema: Alterando datas ou cancelando serviços.

# Diagrama de casos de uso:

![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/diagramacasosdeuso.png "Logo Title Text 1 " )


________________________________________

# Caso de Uso Crítico:
	  Nome: Agendar Manutenção
   
	  Ator Principal: Atendente
   
	  Descrição: O atendente seleciona um cliente e um veículo, escolhe uma data e hora, e define o tipo de serviço para registrar a manutenção a ser realizada.
   
	  Pré-condição: O cliente e o veículo devem estar cadastrados no sistema.
   
# Fluxo Principal:

1.	O atendente acessa a funcionalidade de agendamento.
   
2.	O atendente seleciona um cliente.
   
3.	O atendente seleciona um veículo associado ao cliente.
   
4.	O atendente escolhe data e horário para o serviço.

5.	O atendente seleciona o tipo de serviço necessário.
    
6.	O sistema registra o agendamento e confirma para o atendente.
    
7.	Pós-condição: A manutenção está agendada e registrada no sistema.


# TG2 - Modelagem de negócio e prototipação

Modelagem de Domínio:


![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/classes.png)




A modelagem do domínio foi realizada com base nos casos de uso e estruturada seguindo boas práticas e padrões de análise de sistemas. Aqui está um detalhamento do processo:

# 1. Identificação das Entidades Principais (Baseada nos Casos de Uso)

A partir dos casos de uso, foram identificadas as entidades principais que representam os conceitos do sistema:

	•	Cliente: necessário para o cadastro e agendamentos.
 
	•	Veículo: vinculado ao cliente e essencial para a manutenção.
 
	•	Agendamento: criado ao agendar uma manutenção.
 
	•	Manutenção: contém detalhes sobre os serviços realizados.
 
	•	Histórico de Manutenção: permite consultar serviços anteriores.



# 2. Aplicação de Padrões de Análise

Para estruturar melhor, foi aplicado alguns padrões de análise comuns em modelagem de domínio:

	•	Associação entre classes: Cliente e Veículo possuem uma relação “um-para-muitos” (um cliente pode ter vários veículos).
 
	•	Agregação: O Histórico de Manutenção armazena várias manutenções associadas a um cliente.
 
	•	Encapsulamento: Os atributos e métodos das classes foram definidos para garantir que cada entidade tenha um papel claro no sistema.

# 3. Ajustes e Melhorias

Durante a modelagem, foram feitos alguns ajustes:
	•	Inicialmente, Histórico de Manutenção não existia como entidade separada, mas foi criado para facilitar consultas.
 
	•	O relacionamento entre Agendamento e Manutenção foi refinado para garantir que cada manutenção esteja sempre associada a um agendamento válido.
 
	•	O atributo status foi adicionado em Agendamento e Manutenção para permitir o rastreamento do progresso dos serviços.



 # Frames ( telas principais): 

 # Login:
 
![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/Login.jpg "Logo Title Text 1 " )

# Inicio
Após logar o usuário tem essas opções para navegar no sistema, no protótipo : 

![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/Inicio.jpg "Logo Title Text 1 " )

# Cadastrar Cliente

No cadastrar cliente, temos os campos de nome, email, telefone e email.

![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/CadastrarCliente.jpg "Logo Title Text 1 " )

# Cadastrar Veículo

Aqui podemos cadastrar as informações necessárias do veículo e associar a apenas um cliente.

![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/CadastrarVeiculo.jpg "Logo Title Text 1 " )

# Agendar Manutenção

Aqui o atendente pode agendar uma manutenção com as informações do cliente e veiculo.

![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/AgendManut.jpg "Logo Title Text 1 " )

# Status

O atendente pode consultar as manutenções por status e mudar o status delas (em outra página Status por Cliente)



![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/status.jpg "Logo Title Text 1 " )

link interativo do protótipo : https://www.figma.com/design/w8zd6e34MCzkzNq1xp9fCW/Figma-basics?node-id=601-871&t=KX8kKaOyYAMytcop-1


# Especificação de Requisitos - Sistema de Gerenciamento de Manutenção de Veículos

## Introdução

### Propósito
O presente documento tem como objetivo descrever detalhadamente os requisitos do Sistema de Gerenciamento de Manutenção de Veículos, garantindo que todas as funcionalidades essenciais e regras de negócio sejam compreendidas e implementadas corretamente.

### Escopo
O sistema visa facilitar o gerenciamento de oficinas mecânicas, permitindo o cadastro de clientes, veículos e agendamentos de manutenções, além de acompanhar o status dos serviços e manter um histórico de manutenções.

### Definições, Acrônimos e Abreviações
- **Usuário**: Atendente da oficina mecânica que utiliza o sistema.
- **Cliente**: Proprietário do veículo que solicita serviços de manutenção.
- **Agendamento**: Registro de uma manutenção futura para um veículo.
- **Histórico de Manutenção**: Lista de serviços realizados em um determinado veículo.

## Desempenho

- O sistema deve garantir que a consulta de agendamentos e a alteração de status das manutenções sejam realizadas em no máximo 3 segundos, independentemente do número de registros no banco de dados.
- O sistema deve suportar até 100 usuários simultâneos (atendentes) sem degradação de desempenho, mesmo quando vários atendimentos estão sendo realizados ao mesmo tempo.

## Usabilidade

- O sistema deve ter uma interface simples e intuitiva, permitindo que atendentes inexperientes realizem tarefas como cadastro de clientes, veículos e agendamentos de manutenção em até 2 minutos após o primeiro contato com o sistema.
- A navegação deve ser clara e o fluxo de tarefas (como agendar manutenção e consultar histórico de serviços) deve seguir uma sequência lógica e fácil de entender.

## Segurança

- Todos os dados pessoais dos clientes (nome, telefone, e-mail) e informações dos veículos devem ser armazenados com criptografia de ponta a ponta para garantir a proteção contra acessos não autorizados.
- O sistema deve autenticar todos os atendentes por meio de login e senha, garantindo que apenas usuários autorizados possam acessar informações sensíveis, como detalhes de clientes e status de manutenções.
- O sistema deve estar em conformidade com a Lei Geral de Proteção de Dados (LGPD), garantindo que os dados pessoais sejam tratados de acordo com as regulamentações legais.

## Confiabilidade

- O sistema deve garantir uma disponibilidade mínima de 99,5% durante o horário de operação das oficinas (de segunda a sábado, das 8h às 18h). Isso significa que o sistema pode estar fora do ar no máximo 12 horas por ano.
- O sistema deve implementar backup automático diário de todos os dados (clientes, veículos, manutenções e histórico), com armazenamento em uma solução de backup segura. Em caso de falha, o sistema deve ser capaz de restaurar os dados até o ponto do último backup realizado, sem perda de informações importantes.
- Mecanismos de recuperação devem ser implementados, de modo que, em caso de falha de algum componente (como banco de dados ou servidor), o sistema consiga retornar à operação normal em no máximo 30 minutos.
- O sistema deve ter uma auditoria de logs para registrar todas as operações críticas, como alterações de status de manutenções e agendamentos. Esses logs devem ser armazenados por pelo menos 6 meses para rastreamento e solução de problemas.

## Requisitos

### 2.1. Requisitos Funcionais



RF-001	O sistema deve permitir o cadastro de clientes, armazenando nome, e-mail e telefone.

RF-002	O sistema deve permitir o cadastro de veículos, vinculando-os a um cliente específico.

RF-003	O sistema deve possibilitar o agendamento de manutenções, registrando a data, hora e serviço a ser realizado.

RF-004	O sistema deve permitir que o atendente atualize o status de uma manutenção ("Pendente", "Em Andamento", "Concluído").

RF-005	O sistema deve permitir a listagem de todos os agendamentos de manutenção.

RF-006	O sistema deve permitir a consulta de detalhes de uma manutenção específica.

RF-007	O sistema deve fornecer um histórico de manutenções realizadas para cada cliente.

RF-008	O sistema deve permitir que o atendente cancele ou reagende uma manutenção.

RF-009	O sistema deve permitir a autenticação dos usuários com login e senha.

RF-010	O sistema deve exibir os serviços disponíveis para manutenção.


### 2.2. Requisitos Não Funcionais



RNF-001	O sistema deve ser acessível via navegador web.

RNF-002	O tempo de resposta para carregamento de qualquer página não deve ultrapassar 3 segundos.

RNF-003	O sistema deve armazenar senhas de usuários de forma segura, utilizando criptografia.

RNF-004	O sistema deve seguir os princípios de usabilidade.

RNF-005	O banco de dados deve suportar pelo menos 1.000 registros de clientes e veículos sem perda de desempenho.

RNF-006	O sistema deve impedir o cadastro de veículos sem um cliente associado.

RNF-007	O sistema deve permitir múltiplos acessos simultâneos sem degradação perceptível de desempenho.

RNF-008	O sistema deve registrar logs de atividade.

RNF-009	A interface do sistema deve ser responsiva para dispositivos móveis e desktops.

RNF-010	O sistema deve ter proteção contra injeção de SQL.


### 2.3. Requisitos Suplementares
![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/id1.png "Logo Title Text 1 " )
![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/req1.png "Logo Title Text 1 " )
![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/re2.png "Logo Title Text 1 " )

### Regras de Negócio
![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/regras1.png "Logo Title Text 1 " )
![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/rg2.png "Logo Title Text 1 " )


# TG4 - Diagrama de sequência do caso de uso principal

![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/diagramasequencia.png "Logo Title Text 1 " )





O ator Atendente inicia o processo chamando o controlador de agendamento, que é o responsável por coordenar a execução da funcionalidade.
Em seguida, o sistema busca os dados do cliente e do veículo, utilizando os respectivos identificadores (CPF e placa).
Após isso, o atendente informa os dados do agendamento (data, hora e tipo de serviço), e o sistema realiza as seguintes etapas:

Criação de um novo objeto de agendamento contendo o cliente e veículo.

Instanciação de um objeto de manutenção, com o status inicial "Pendente".

Associação da manutenção ao agendamento.

Confirmação da operação para o atendente.

# Aplicação dos Padrões GRASP
Durante a modelagem do diagrama, foram aplicados os seguintes padrões GRASP para garantir um design orientado a objetos de qualidade:

Controlador: A classe AgendamentoController atua como controlador do caso de uso, sendo responsável por coordenar as interações e decisões necessárias para completar a operação. Esse padrão favorece o encapsulamento da lógica de aplicação.

Especialista em Informação: As responsabilidades de criação e associação foram atribuídas às classes que possuem as informações necessárias (como Agendamento e Manutencao). Isso promove um design coeso e distribuído adequadamente.

Baixo Acoplamento: As interações entre os objetos seguem o princípio de baixo acoplamento, garantindo que cada classe dependa minimamente de outras para executar suas funções.

Alta Coesão: As operações são mantidas dentro de classes que têm motivos claros para existir, aumentando a legibilidade e facilidade de manutenção do sistema.




# 📦 TG5 – Diagrama de Componentes

Este diagrama representa uma **visão de alto nível da arquitetura modular** do sistema de gerenciamento de manutenção de veículos. A modularização proposta segue princípios de baixo acoplamento, alta coesão e responsabilidade única.

---
![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/diagramaFinal.png "Logo Title Text 1 " )



# 📐 Arquitetura Geral

O sistema está dividido em **três camadas lógicas**:

- **Apresentação**: onde o atendente interage com a interface.
- **Controle e Domínio**: onde ocorre o gerenciamento das regras de negócio.
- **Infraestrutura**: onde estão os dados persistidos, a segurança e os registros de log.

---

## 🔧 Componentes e Responsabilidades

| Componente              | Responsabilidade                                                                 |
|-------------------------|----------------------------------------------------------------------------------|
| `InterfaceWeb`          | Tela e navegação para o atendente realizar ações no sistema.                     |
| `AgendamentoController` | Controlador principal, intermedia a interface e os demais módulos do domínio.    |
| `CadastroVeiculo`       | Gerencia o registro de veículos e associação com clientes.                       |
| `GerenciadorAgdm`       | Responsável por criar, editar e consultar agendamentos de manutenção.           |
| `Autenticador`          | Garante que apenas usuários autorizados possam acessar o sistema.               |
| `BancoDedados`            | Armazena os dados estruturados do sistema.                                      |
| `GeradorLogs`          | Registra todas as ações críticas do sistema para auditoria e rastreabilidade.   |
| `Relatório`             | Produz relatórios baseados nos dados de agendamentos e histórico.               |
| `Persistência`          | Responsável pela gravação e leitura de dados do sistema.                        |
| `FabricaDeServicos` | Cria instâncias de serviços usados por diversos componentes, via padrão Factory. |

---

## 🔗 Justificativa das Conexões

- `InterfaceWeb` conecta-se ao `AgendamentoController`, que orquestra as operações.
- O `AgendamentoController` se comunica diretamente com `Autenticador`, `GerenciadorAgdm` e `CadastroVeiculo`.
- Cada módulo de domínio conecta-se a seus respectivos serviços de suporte:
  - `Autenticador` → `BancoDedao` (validação de credenciais)
  - `GerenciadorAgdm` → `GeradorLogss` e `Relatório`
  - `CadastroVeiculo` → `Persistência`
- `FabricaDeServicos ` é usada por `BancoDedao`, `GeradorLogss`, `Relatório` e `Persistência` como fábrica para instanciar objetos.

---

## ✅ Benefícios da Arquitetura Modular

- **Coesão**: cada módulo realiza uma função clara e específica.
- **Reuso**: componentes como `CadastroVeiculo` ou `Relatório` podem ser reutilizados em outros sistemas.
- **Escalabilidade**: novos componentes podem ser acoplados facilmente.
- **Baixo acoplamento**: dependências controladas por interfaces explícitas.
- **Aderência a GRASP e SOLID**: facilita manutenção, expansão e entendimento do sistema.


---

## 💡 Observação Técnica: Por que `CadastroVeiculo` usa `Persistência`?

O componente `CadastroVeiculo` não deve se conectar diretamente ao banco de dados, pois isso violaria o princípio da **separação de responsabilidades (SRP)**.

A responsabilidade do `CadastroVeiculo` é aplicar regras de negócio, como:
- Validar dados do veículo
- Associar veículos a clientes
- Verificar duplicidade de registros

Já o componente `Persistência` cuida do *como* os dados são armazenados:
- Interação com o banco de dados
- Comandos SQL ou ORMs
- Estratégias de leitura/escrita

### ✅ Vantagens dessa separação:

- **Desacoplamento**: facilita a troca da tecnologia de banco de dados.
- **Testabilidade**: o módulo de persistência pode ser simulado em testes.
- **Organização**: cada componente faz uma coisa só — domínio decide *o quê*, persistência cuida do *como*.
- **Reuso**: outros componentes, como `HistoricoManutencao` ou `Agendamento`, também podem usar a mesma `Persistência`.

Essa prática segue os princípios do **Clean Architecture**, **GRASP** e **SOLID**, tornando o sistema mais robusto e evolutivo.


# TG6 - Diagrama de Pacotes: Arquitetura em Camadas do Sistema

![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/pacotes.png "pacotes " )

Este documento apresenta o **Diagrama de Pacotes** do nosso sistema de gerenciamento de manutenção de veículos. Este diagrama é fundamental para compreender a **arquitetura modular e em camadas** do projeto, demonstrando a organização lógica do código e as dependências entre os diferentes componentes do sistema.

A modularização adotada segue princípios de **baixo acoplamento, alta coesão e responsabilidade única**, buscando facilitar a manutenção, o desenvolvimento e a escalabilidade do sistema.

## Visão Geral do Diagrama de Pacotes

O diagrama está organizado em quatro camadas principais, que representam diferentes níveis de abstração e responsabilidade dentro da aplicação:

1.  **Apresentação:** Responsável pela interface com o usuário.
2.  **Aplicação:** Gerencia o fluxo de trabalho e orquestra as operações de negócio.
3.  **Negócio:** Contém a lógica de negócio principal do sistema.
4.  **Persistência:** Lida com o armazenamento e recuperação de dados.

### Detalhes das Camadas e Pacotes

Abaixo, detalhamos cada camada e os pacotes que a compõem, juntamente com suas principais responsabilidades e as dependências observadas:

#### 1. Camada de Apresentação

Esta camada é a mais externa e interage diretamente com o usuário.

* **`UILogin`**: Pacote responsável pela interface de login do sistema. Inicia o processo de autenticação.
* **`UIAgendarManutencao`**: Pacote para a interface de agendamento de manutenções. Permite ao usuário solicitar e configurar agendamentos.
* **`UICadastrarVeiculo`**: Pacote dedicado à interface de cadastro de veículos.
* **`UIConsultarAgendamento`**: Pacote para a interface de consulta de agendamentos existentes.

**Dependências:** Os pacotes da camada de Apresentação dependem dos controladores na camada de Aplicação para realizar suas operações.

#### 2. Camada de Aplicação

Atua como um intermediário entre a camada de Apresentação e a camada de Negócio. É responsável por gerenciar as requisições da interface do usuário e coordenar as interações com a lógica de negócio.

* **`AgendamentoController`**: Gerencia as operações relacionadas a agendamentos, como criação, consulta e atualização.
* **`LoginController`**: Controla o fluxo de autenticação e autorização de usuários.
* **`CadastroVeiculoController`**: Responsável pelas operações de cadastro de veículos.

**Dependências:** Os `Controllers` nesta camada dependem da lógica de negócio na camada de Negócio para executar suas funcionalidades.

#### 3. Camada de Negócio (ou Domínio)

Esta é a camada central do sistema, onde reside toda a lógica de negócio e as regras de negócio.

* **`Agendamento`**: Contém a lógica e as entidades relacionadas a agendamentos de manutenção.
* **`Login`**: Contém a lógica para o processo de autenticação e gestão de usuários.
* **`Cadastro`**: Contém a lógica e as entidades relacionadas ao cadastro de veículos e outras informações relevantes.

**Dependências:** Os pacotes de Negócio podem depender de outros pacotes de Negócio (para reutilização de lógica) e da camada de Persistência para acessar e manipular dados.

#### 4. Camada de Persistência

Responsável por todas as operações de acesso a dados, isolando a lógica de negócio dos detalhes de armazenamento (banco de dados, arquivos, etc.).

* **`DAOAgendamento`**: Data Access Object para as entidades de agendamento. Responsável por salvar, recuperar, atualizar e deletar dados de agendamento no banco de dados.
* **`DAOLogin`**: Data Access Object para as entidades de login/usuário.
* **`DAOCadastro`**: Data Access Object para as entidades de cadastro (veículos, etc.).

**Dependências:** Esta camada não deve ter dependências de camadas superiores. As dependências são sempre no sentido de baixo para cima (ou seja, Negócio depende de Persistência, Aplicação depende de Negócio, Apresentação depende de Aplicação).

## Comparativo com TG4 e TG5 (Correções e Evolução)

É importante notar a evolução da arquitetura desde as entregas anteriores.

* **Comparado ao TG4 (Estrutura Inicial)**: No TG4, nossa abordagem inicial pode ter sido mais simplificada. O Diagrama de Pacotes para o TG6 reflete uma **clara separação de responsabilidades em camadas**, o que pode não ter sido tão explícito ou rigidamente aplicado no TG4. A transição para um modelo em camadas mais robusto visa melhorar a manutenibilidade e a escalabilidade.
* **Comparado ao TG5 (Diagrama de Componentes)**: Enquanto o TG5 focou nos **Componentes** (como `AgendamentoController`, `BancoDeDados`, etc.) e suas interações a um nível mais granular e tecnológico, o TG6, através do Diagrama de Pacotes, apresenta uma **visão mais estratégica e lógica da organização do código em termos de domínios e responsabilidades**. O Diagrama de Pacotes complementa o Diagrama de Componentes ao agrupar esses componentes em estruturas lógicas maiores e definir as dependências entre elas.

**Principais Correções e Melhorias na Abordagem para o TG6:**

* **Reforço da Coesão e Acoplamento:** A estrutura de pacotes agora visa garantir que cada pacote tenha uma responsabilidade bem definida (alta coesão) e que as dependências entre eles sejam mínimas e bem controladas (baixo acoplamento).
* **Clara Separação de Preocupações:** As camadas de Apresentação, Aplicação, Negócio e Persistência estão mais bem definidas e isoladas, o que facilita a modificação de uma camada sem afetar as outras, desde que a interface de comunicação seja mantida.
* **Consistência nas Nomenclaturas:** As nomenclaturas dos pacotes e seus conteúdos estão mais padronizadas, seguindo convenções claras para cada camada.

Esta estrutura em camadas é um pilar para o desenvolvimento de um sistema robusto e de fácil manutenção, garantindo que a lógica de negócio esteja desacoplada da interface do usuário e dos detalhes de persistência.
