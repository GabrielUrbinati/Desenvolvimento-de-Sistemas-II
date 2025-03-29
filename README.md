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


![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/classes.png "Logo Title Text 1 " )




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

ID	Descrição

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

ID	Descrição

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



### Regras de Negócio




