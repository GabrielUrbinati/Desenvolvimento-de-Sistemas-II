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

<img src="https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/diagramacasosdeuso.png" alt="IMAGE ALT TEXT HERE" width="5600" height="auto" border="10" />
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



![alt text](https://github.com/GabrielUrbinati/Desenvolvimento-de-Sistemas-II/blob/main/diagramacasosdeuso.png "Logo Title Text 1")

