# 📚 Atividade Prática – Engenharia de Requisitos ( Projeto/Atividade)

## Estudo de Caso: Sistema de Atendimento e Agendamento da Clínica Vida+ Saúde

**Disciplina:** Engenharia de Requisitos
**Curso:** Engenharia de Software
**Modalidade:** Trabalho
**Aluno:** Marco Antônio Nista Popovidis, Nicolle Da Silva Coelho, Victor Gabriel, João Pedro Pimentel

---

# Etapa 1 – Identificação do Processo

### 1. Qual é o nome do processo?

**Processo de Atendimento e Agendamento de Consultas da Clínica Vida+ Saúde.**

### 2. Qual é o objetivo do processo?

O objetivo é realizar o atendimento ao paciente de forma organizada, desde a solicitação de uma consulta, passando pelo cadastro, consulta de disponibilidade, agendamento e confirmação, até a realização da consulta e registro do atendimento.

O processo também deve possibilitar o controle de cancelamentos, faltas e alterações na agenda dos médicos.

### 3. Quem é o cliente do processo?

O principal cliente é o **paciente**, que necessita conseguir uma consulta de maneira rápida, organizada e confiável.

A clínica também é beneficiada, pois busca melhorar a utilização das agendas, reduzir retrabalho e melhorar a qualidade do atendimento.

### 4. Quem executa as atividades?

* Paciente;
* Recepcionista;
* Médico;
* Equipe administrativa;
* Gerente da clínica;
* Equipe de TI, quando relacionada ao sistema.

### 5. Quem gerencia o processo?

A gerência e a direção da Clínica Vida+ Saúde são responsáveis pelo gerenciamento do processo e pelo acompanhamento dos resultados.

### 6. Qual evento inicia o processo?

O processo começa quando o paciente solicita uma consulta por telefone, WhatsApp ou presencialmente.

### 7. Qual evento encerra o processo?

Para o processo completo, o encerramento ocorre após a realização da consulta e o registro do atendimento pelo médico.

### 8. Qual valor é entregue ao cliente?

O paciente recebe como valor um atendimento médico agendado e organizado, com informações corretas sobre médico, especialidade, data e horário.

Para a clínica, o processo gera valor por meio da melhor utilização dos horários disponíveis, redução de conflitos, redução de retrabalho e melhoria da gestão.

---

# Etapa 2 – Identificação dos Stakeholders

| Stakeholder            | Interesse no processo                              | Participação                                             | Necessidades                                     |
| ---------------------- | -------------------------------------------------- | -------------------------------------------------------- | ------------------------------------------------ |
| Paciente               | Conseguir uma consulta de forma rápida e confiável | Solicita, confirma, cancela e comparece                  | Agendamento simples, confirmação e lembretes     |
| Recepcionista          | Realizar os agendamentos corretamente              | Cadastra pacientes, consulta agenda e confirma consultas | Sistema rápido, centralizado e fácil de utilizar |
| Médico                 | Organizar sua agenda e realizar consultas          | Disponibiliza horários e realiza atendimentos            | Agenda atualizada e informações dos pacientes    |
| Gerente                | Garantir eficiência do processo                    | Acompanha operação e indicadores                         | Relatórios e indicadores confiáveis              |
| Direção                | Melhorar os resultados da clínica                  | Define objetivos e acompanha resultados                  | Redução de custos, faltas e conflitos            |
| Equipe administrativa  | Apoiar a organização da clínica                    | Manipula e consulta informações                          | Dados centralizados e atualizados                |
| Equipe de TI           | Garantir funcionamento do sistema                  | Implanta, mantém e presta suporte                        | Segurança, disponibilidade e manutenção          |
| Responsável financeiro | Acompanhar impactos financeiros                    | Analisa custos e resultados                              | Informações confiáveis para análise              |

---

# Etapa 3 – Análise do Processo Atual

## Quem?

**Cliente:** paciente.

**Executores:** recepcionistas e médicos.

**Gestores:** gerente e direção.

**Fornecedores de informações:** pacientes, médicos e equipe administrativa.

**Participantes das decisões:** gerência, direção e médicos.

## O quê?

### Entradas

* Solicitação de consulta;
* Nome;
* CPF;
* Telefone;
* Data de nascimento;
* E-mail;
* Especialidade;
* Médico;
* Data desejada;
* Horário desejado;
* Disponibilidade da agenda.

### Saídas

* Cadastro ou atualização do paciente;
* Agendamento;
* Confirmação;
* Atendimento realizado;
* Registro da consulta;
* Cancelamento;
* Atualização da agenda.

### Recursos utilizados

* Recepcionistas;
* Médicos;
* Computadores;
* Planilhas;
* Telefone;
* WhatsApp;
* Sistema utilizado pelo médico.

### Problemas

* Conflitos de horários;
* Informações desatualizadas;
* Duplicidade de cadastros;
* Retrabalho;
* Falhas de comunicação;
* Ausência de lembretes;
* Controle manual de cancelamentos;
* Dificuldade para alterar agendas;
* Falta de indicadores centralizados.

### Pontos positivos

* A clínica possui um processo definido;
* Existem profissionais responsáveis;
* Existem diferentes canais de atendimento;
* Os médicos já utilizam um sistema para registrar atendimentos;
* A direção reconhece a necessidade de melhoria.

## Quando?

O processo começa quando o paciente solicita uma consulta.

As atividades são executadas durante o contato com a recepção, antes da consulta e durante o atendimento médico.

O processo termina após a realização e registro da consulta.

## Onde?

O processo pode ser iniciado por:

* Telefone;
* WhatsApp;
* Atendimento presencial.

As atividades são realizadas principalmente na recepção e nos consultórios.

Atualmente, as informações são registradas em planilhas e sistemas diferentes.

## Por quê?

O processo existe para possibilitar que pacientes sejam atendidos pelos médicos da clínica de maneira organizada.

Para o paciente, entrega praticidade e acesso ao atendimento.

Para a clínica, permite organizar recursos, médicos, horários e pacientes.

## Como?

Atualmente, o paciente solicita a consulta. A recepcionista identifica o paciente, consulta a agenda em uma planilha, verifica a disponibilidade, registra o agendamento e confirma a consulta.

Posteriormente, o paciente comparece, a recepcionista confirma seus dados e o médico realiza o atendimento.

Cancelamentos e alterações de agenda são tratados manualmente.

---

# Etapa 4 – Identificação das Atividades

| Atividade                 | Responsável            | Entrada                    | Saída                           | Regra                                 |
| ------------------------- | ---------------------- | -------------------------- | ------------------------------- | ------------------------------------- |
| Solicitar consulta        | Paciente               | Necessidade de consulta    | Solicitação                     | Deve informar médico ou especialidade |
| Identificar paciente      | Recepcionista          | Dados do paciente          | Paciente identificado           | Deve verificar cadastro existente     |
| Solicitar dados           | Recepcionista          | Dados cadastrais           | Dados registrados               | Informações devem ser conferidas      |
| Consultar agenda          | Recepcionista          | Médico/especialidade       | Agenda consultada               | Deve consultar a agenda correta       |
| Verificar disponibilidade | Recepcionista          | Agenda                     | Horário disponível/indisponível | Não pode haver conflito               |
| Escolher horário          | Paciente               | Horários disponíveis       | Horário escolhido               | Deve ser um horário disponível        |
| Registrar agendamento     | Recepcionista          | Dados da consulta          | Agendamento                     | Horário deve estar livre              |
| Confirmar consulta        | Recepcionista          | Agendamento                | Confirmação                     | Paciente deve receber informações     |
| Aguardar atendimento      | Paciente               | Agendamento                | Paciente aguardando             | Deve comparecer                       |
| Confirmar presença        | Recepcionista          | Paciente presente          | Presença registrada             | Deve existir agendamento              |
| Realizar consulta         | Médico                 | Paciente                   | Atendimento                     | Médico realiza consulta               |
| Registrar atendimento     | Médico                 | Informações da consulta    | Registro                        | Atendimento deve ser registrado       |
| Cancelar consulta         | Paciente/Recepcionista | Solicitação                | Cancelamento                    | Horário deve ser liberado             |
| Alterar agenda            | Médico/Recepcionista   | Mudança de disponibilidade | Agenda alterada                 | Pacientes afetados devem ser avisados |
| Encerrar atendimento      | Clínica                | Registro                   | Processo encerrado              | Atendimento deve estar registrado     |

---

# Etapa 5 – Regras de Negócio

| Código | Regra de Negócio                                                                         | Origem                  |
| ------ | ---------------------------------------------------------------------------------------- | ----------------------- |
| RN01   | O paciente deve possuir cadastro antes de realizar um agendamento.                       | Processo atual          |
| RN02   | Um médico não pode possuir dois pacientes agendados no mesmo horário.                    | Processo atual          |
| RN03   | Uma consulta somente pode ser agendada em horário disponível.                            | Processo atual          |
| RN04   | O cancelamento deve liberar o horário da consulta.                                       | Processo atual          |
| RN05   | Os dados do paciente devem ser confirmados no atendimento.                               | Processo atual          |
| RN06   | Todo agendamento deve estar associado a paciente, médico, especialidade, data e horário. | Processo proposto       |
| RN07   | Alterações na agenda devem gerar comunicação aos pacientes afetados.                     | Problema identificado   |
| RN08   | O sistema deve registrar o status da consulta.                                           | Necessidade de controle |
| RN09   | Somente horários disponíveis podem ser utilizados em novos agendamentos.                 | Processo proposto       |
| RN10   | O sistema deve manter histórico dos agendamentos e alterações.                           | Rastreabilidade         |

---

# Etapa 6 – Identificação dos Problemas

| Problema                   | Causa provável                | Impacto                             | Prioridade |
| -------------------------- | ----------------------------- | ----------------------------------- | ---------- |
| Conflito de horários       | Planilhas independentes       | Agendamentos duplicados             | Alta       |
| Retrabalho                 | Informações espalhadas        | Perda de produtividade              | Alta       |
| Cadastro duplicado         | Dados solicitados novamente   | Inconsistência de informações       | Alta       |
| Falha de confirmação       | Comunicação manual            | Paciente pode ficar sem confirmação | Alta       |
| Ausência de lembretes      | Falta de automação            | Aumento das faltas                  | Alta       |
| Cancelamentos manuais      | Controle pela recepção        | Horários podem permanecer vazios    | Média      |
| Alteração manual da agenda | Comunicação individual        | Falhas de comunicação               | Alta       |
| Falta de indicadores       | Informações não centralizadas | Dificuldade de gestão               | Média      |
| Sistemas separados         | Fragmentação das informações  | Retrabalho                          | Média      |
| Dados desatualizados       | Atualização manual            | Decisões incorretas                 | Alta       |

---

# Etapa 7 – Modelagem AS-IS

O processo atual pode ser representado da seguinte maneira:

**INÍCIO**

↓

**Paciente solicita consulta**

↓

**Recepcionista identifica paciente**

↓

**Paciente possui cadastro?**

**Não** → Solicitar/cadastrar dados → Continuar

**Sim** → Confirmar dados → Continuar

↓

**Consultar agenda na planilha**

↓

**Existe horário disponível?**

**Não** → Informar indisponibilidade → Oferecer outro horário

**Sim** → Selecionar horário

↓

**Registrar agendamento na planilha**

↓

**Confirmar consulta**

↓

**Paciente compareceu?**

**Não** → Registrar falta → **FIM**

**Sim** → Confirmar presença

↓

**Médico realiza consulta**

↓

**Médico registra atendimento em sistema separado**

↓

**FIM**

### Fluxos alternativos

**Cancelamento:**

Paciente solicita cancelamento → Recepcionista procura o agendamento → Atualiza planilha → Libera horário → Procura manualmente outro paciente.

**Alteração da agenda médica:**

Médico altera agenda → Recepcionista identifica pacientes afetados → Entra em contato individualmente → Reagenda ou cancela.

---

# Etapa 8 – Proposta de Melhorias

| Problema                    | Melhoria proposta            | Benefício esperado            |
| --------------------------- | ---------------------------- | ----------------------------- |
| Conflito de horários        | Agenda centralizada          | Redução de conflitos          |
| Cadastro duplicado          | Cadastro único               | Redução de retrabalho         |
| Falta de confirmação        | Confirmação automática       | Maior confiabilidade          |
| Falta de lembretes          | Lembretes automáticos        | Redução de faltas             |
| Cancelamentos manuais       | Cancelamento integrado       | Liberação rápida dos horários |
| Alteração de agenda         | Notificação automática       | Melhor comunicação            |
| Falta de indicadores        | Dashboard gerencial          | Melhor tomada de decisão      |
| Informações fragmentadas    | Banco de dados centralizado  | Dados consistentes            |
| Consulta manual de horários | Agenda digital em tempo real | Agendamento mais rápido       |
| Sistemas separados          | Integração das informações   | Redução da fragmentação       |

---

# Etapa 9 – Modelagem TO-BE

O processo futuro será:

**INÍCIO**

↓

**Paciente solicita consulta**

↓

**Sistema identifica paciente**

↓

**Paciente possui cadastro?**

**Não** → Realizar cadastro

**Sim** → Recuperar dados

↓

**Selecionar médico/especialidade**

↓

**Consultar agenda centralizada**

↓

**Existe horário disponível?**

**Não** → Apresentar outras opções

**Sim** → Selecionar horário

↓

**Sistema valida disponibilidade**

↓

**Registrar agendamento**

↓

**Enviar confirmação**

↓

**Enviar lembrete automático**

↓

**Paciente compareceu?**

**Não** → Registrar falta

**Sim** → Confirmar presença

↓

**Médico realiza consulta**

↓

**Registrar atendimento**

↓

**Atualizar indicadores**

↓

**FIM**

### Cancelamento TO-BE

Paciente solicita cancelamento → Sistema identifica consulta → Registra cancelamento → Libera horário → Atualiza indicador → Horário volta a ficar disponível.

### Alteração de agenda TO-BE

Médico altera disponibilidade → Sistema identifica pacientes afetados → Envia notificações → Apresenta opções de reagendamento → Atualiza agenda.

---

# Etapa 10 – Requisitos Funcionais

| Código | Requisito Funcional                                                       | Prioridade  |
| ------ | ------------------------------------------------------------------------- | ----------- |
| RF01   | O sistema deverá permitir cadastrar pacientes.                            | Must Have   |
| RF02   | O sistema deverá permitir consultar e atualizar pacientes.                | Must Have   |
| RF03   | O sistema deverá permitir cadastrar médicos.                              | Must Have   |
| RF04   | O sistema deverá permitir cadastrar especialidades.                       | Must Have   |
| RF05   | O sistema deverá permitir cadastrar horários de atendimento dos médicos.  | Must Have   |
| RF06   | O sistema deverá permitir consultar horários disponíveis.                 | Must Have   |
| RF07   | O sistema deverá permitir realizar agendamentos.                          | Must Have   |
| RF08   | O sistema deverá impedir dois agendamentos para o mesmo médico e horário. | Must Have   |
| RF09   | O sistema deverá permitir cancelar consultas.                             | Must Have   |
| RF10   | O sistema deverá permitir reagendar consultas.                            | Should Have |
| RF11   | O sistema deverá enviar confirmação do agendamento.                       | Must Have   |
| RF12   | O sistema deverá enviar lembretes das consultas.                          | Should Have |
| RF13   | O sistema deverá permitir registrar presença ou falta.                    | Must Have   |
| RF14   | O sistema deverá permitir ao médico registrar o atendimento.              | Must Have   |
| RF15   | O sistema deverá disponibilizar indicadores de desempenho.                | Should Have |

---

# Etapa 11 – Requisitos Não Funcionais

| Código | Categoria       | Requisito                                                                                |
| ------ | --------------- | ---------------------------------------------------------------------------------------- |
| RNF01  | Desempenho      | O sistema deverá apresentar os horários disponíveis em até 3 segundos.                   |
| RNF02  | Segurança       | O sistema deverá exigir autenticação para usuários administrativos.                      |
| RNF03  | Usabilidade     | As operações principais deverão possuir interface simples e intuitiva.                   |
| RNF04  | Disponibilidade | O sistema deverá estar disponível durante o horário de funcionamento da clínica.         |
| RNF05  | Confiabilidade  | O sistema deverá evitar perda de dados durante operações de cadastro e agendamento.      |
| RNF06  | Privacidade     | Os dados pessoais dos pacientes deverão ser protegidos contra acesso não autorizado.     |
| RNF07  | Desempenho      | O processamento de um agendamento deverá ocorrer em até 3 segundos em condições normais. |
| RNF08  | Segurança       | O sistema deverá controlar o acesso conforme o perfil do usuário.                        |
| RNF09  | Usabilidade     | O sistema deverá apresentar mensagens claras de erro e confirmação.                      |
| RNF10  | Compatibilidade | O sistema deverá funcionar nos principais navegadores utilizados pela clínica.           |

---

# Etapa 12 – Indicadores de Desempenho

| Indicador                          | Objetivo                         | Forma de cálculo                               | Meta                       |
| ---------------------------------- | -------------------------------- | ---------------------------------------------- | -------------------------- |
| Taxa de ocupação                   | Medir utilização da agenda       | Horários ocupados ÷ horários disponíveis × 100 | ≥ 85%                      |
| Taxa de cancelamento               | Medir cancelamentos              | Cancelamentos ÷ agendamentos × 100             | ≤ 10%                      |
| Taxa de faltas                     | Medir não comparecimentos        | Faltas ÷ agendamentos × 100                    | ≤ 5%                       |
| Tempo médio de atendimento         | Medir duração dos atendimentos   | Tempo total ÷ atendimentos                     | Conforme especialidade     |
| Tempo médio de agendamento         | Medir eficiência do agendamento  | Tempo total de agendamento ÷ agendamentos      | ≤ 5 minutos                |
| Quantidade de consultas realizadas | Acompanhar volume de atendimento | Total de consultas realizadas                  | Acompanhar evolução mensal |

---

# Etapa 13 – Priorização dos Requisitos

## Must Have – Obrigatórios

* RF01 – Cadastro de pacientes;
* RF02 – Consulta e atualização de pacientes;
* RF03 – Cadastro de médicos;
* RF04 – Cadastro de especialidades;
* RF05 – Cadastro de horários;
* RF06 – Consulta de disponibilidade;
* RF07 – Agendamento;
* RF08 – Prevenção de conflitos;
* RF09 – Cancelamento;
* RF11 – Confirmação;
* RF13 – Registro de presença;
* RF14 – Registro do atendimento.

## Should Have – Importantes

* RF10 – Reagendamento;
* RF12 – Lembretes;
* RF15 – Indicadores.

## Could Have – Desejáveis

* Aplicativo para pacientes;
* Pesquisa de satisfação;
* Lista de espera automatizada;
* Integração com outros sistemas.

## Won't Have – Não será implementado inicialmente

* Gestão financeira completa;
* Controle de estoque;
* Integração com planos de saúde;
* Prontuário eletrônico completo com funcionalidades avançadas.

### Justificativa de cinco decisões

**1. RF07 – Agendamento → Must Have**
É uma das principais funções do sistema e atende diretamente ao problema central da clínica.

**2. RF08 – Prevenção de conflitos → Must Have**
Resolve diretamente um dos principais problemas atuais.

**3. RF11 – Confirmação → Must Have**
Reduz falhas de comunicação com os pacientes.

**4. RF12 – Lembretes → Should Have**
É importante para reduzir faltas, mas o processo básico pode funcionar sem essa funcionalidade na primeira versão.

**5. RF15 – Indicadores → Should Have**
É importante para a gestão e melhoria contínua, mas pode ser implementado após as funcionalidades essenciais.

---

# Etapa 14 – Desafio: Transformando Necessidades em Requisitos

### Necessidade

A recepcionista afirma:

> “Precisamos de um sistema que seja rápido e fácil de usar.”

Essa afirmação é vaga porque os termos “rápido” e “fácil de usar” podem ter interpretações diferentes.

### Requisito verificável

**RNF01 – O sistema deverá apresentar os horários disponíveis de um médico em no máximo 3 segundos após a solicitação do usuário, em condições normais de operação.**

### O requisito está claro?

Sim. O requisito define qual operação será realizada e o tempo máximo esperado.

### É mensurável?

Sim. O tempo de resposta pode ser medido em segundos.

### É testável?

Sim. Pode ser realizado um teste de desempenho para verificar se o resultado está dentro do limite estabelecido.

### Existe alguma ambiguidade?

A expressão “condições normais de operação” pode ser detalhada posteriormente, especificando quantidade de usuários simultâneos e infraestrutura utilizada.

### Como validar?

O requisito pode ser validado por meio de testes de desempenho, medindo o tempo necessário para consultar os horários disponíveis.

---

# Etapa 15 – Relação com o Ciclo BPM

| Etapa BPM                | Aplicação na atividade                                                          |
| ------------------------ | ------------------------------------------------------------------------------- |
| Planejamento             | Definição do objetivo da análise e identificação do processo                    |
| Análise                  | Identificação de stakeholders, atividades, entradas, saídas, regras e problemas |
| Desenho e Modelagem      | Criação dos modelos AS-IS e TO-BE                                               |
| Implementação            | Implantação do sistema de atendimento e agendamento                             |
| Monitoramento e Controle | Acompanhamento dos indicadores de desempenho                                    |
| Refinamento              | Identificação de novos problemas e implementação de melhorias                   |

---

# Etapa 16 – Entregáveis: Análise do Negócio

A análise realizada contempla:

* Descrição do processo;
* Objetivo;
* Stakeholders;
* Entradas;
* Saídas;
* Recursos;
* Regras de negócio;
* Problemas identificados.

## Modelagem

Foram definidos:

* Processo AS-IS;
* Gargalos;
* Propostas de melhoria;
* Processo TO-BE.

## Engenharia de Requisitos

Foram levantados:

* Requisitos funcionais;
* Requisitos não funcionais;
* Regras de negócio;
* Priorização;
* Indicadores.

---

# Etapa 17 – Apresentação

Para uma apresentação de aproximadamente 10 minutos, a sequência recomendada é:

### 1. O problema

A clínica utiliza processos parcialmente manuais e informações distribuídas em diferentes ferramentas.

### 2. Processo atual

Apresentação do modelo AS-IS.

### 3. Principais problemas

* Conflitos de horários;
* Retrabalho;
* Cadastro duplicado;
* Falhas de comunicação;
* Faltas;
* Dificuldade de gestão.

### 4. Processo proposto

Apresentação do modelo TO-BE.

### 5. Principais requisitos

* Cadastro;
* Agenda centralizada;
* Agendamento;
* Cancelamento;
* Confirmação;
* Lembretes;
* Indicadores.

### 6. Melhorias esperadas

* Redução de conflitos;
* Redução de retrabalho;
* Redução de faltas;
* Melhor comunicação;
* Melhor utilização da agenda;
* Maior controle gerencial.

---

# Etapa 18 – Questões para Discussão

## 1. Qual é a diferença entre uma função e um processo de negócio?

Uma função é uma atividade ou capacidade específica desempenhada por uma pessoa, setor ou sistema. Um processo de negócio é um conjunto de atividades relacionadas que possui início, execução e fim e entrega valor a um cliente ou à organização.

## 2. Por que o processo de agendamento deve ser analisado de forma ponta a ponta?

Porque os problemas podem ocorrer em diferentes etapas. Uma análise ponta a ponta permite observar desde a solicitação da consulta até o atendimento, incluindo confirmação, cancelamento, falta e registro.

## 3. Quais atividades atualmente geram maior retrabalho?

* Solicitação repetida dos dados;
* Consulta manual das planilhas;
* Atualização das agendas;
* Confirmações;
* Comunicação de alterações;
* Controle de cancelamentos.

## 4. Quais atividades poderiam ser automatizadas?

* Cadastro;
* Consulta de horários;
* Agendamento;
* Confirmação;
* Lembretes;
* Cancelamento;
* Reagendamento;
* Notificações;
* Indicadores;
* Relatórios.

## 5. Quais regras precisam obrigatoriamente ser implementadas?

Principalmente:

* Impedir dois pacientes no mesmo horário para o mesmo médico;
* Permitir agendamento somente em horários disponíveis;
* Liberar horário após cancelamento;
* Registrar o status da consulta;
* Manter histórico das alterações.

## 6. Quais informações são essenciais?

* Dados do paciente;
* Médico;
* Especialidade;
* Data;
* Horário;
* Status da consulta;
* Informações do atendimento.

## 7. Qual é o principal gargalo?

O principal gargalo é o **controle descentralizado das agendas em planilhas**, que provoca conflitos, desatualização e retrabalho.

## 8. Quais requisitos surgiram diretamente da análise?

* Agenda centralizada;
* Consulta de disponibilidade;
* Prevenção de conflitos;
* Confirmação;
* Lembretes;
* Cancelamento;
* Reagendamento;
* Notificações;
* Indicadores.

## 9. Quais requisitos não funcionais são críticos?

Os mais críticos são:

* Segurança;
* Privacidade;
* Desempenho;
* Disponibilidade;
* Confiabilidade;
* Usabilidade.

## 10. Como os indicadores auxiliam na melhoria contínua?

Os indicadores permitem medir os resultados do processo, identificar problemas e apoiar decisões. Por exemplo, uma taxa elevada de faltas pode indicar a necessidade de melhorar os lembretes das consultas.

---

# Etapa 19 – Síntese do Resultado Esperado

A análise realizada permite representar a transformação do processo da seguinte forma:

**PROCESSO ATUAL – AS-IS**

↓
Informações distribuídas
↓
Planilhas independentes
↓
Conflitos de horários
↓
Retrabalho
↓
Falhas de comunicação
↓
Cancelamentos e faltas
↓
Dificuldade de gestão

**IDENTIFICAÇÃO DOS PROBLEMAS**

↓

**ANÁLISE DOS STAKEHOLDERS**

↓

**IDENTIFICAÇÃO DAS REGRAS DE NEGÓCIO**

↓

**PROPOSTA DE MELHORIAS**

↓

**PROCESSO FUTURO – TO-BE**

↓
Agenda centralizada
↓
Cadastro único
↓
Agendamento integrado
↓
Confirmações automáticas
↓
Lembretes
↓
Controle de cancelamentos
↓
Indicadores

↓

**REQUISITOS FUNCIONAIS**

↓

**REQUISITOS NÃO FUNCIONAIS**

↓

**MELHORIA CONTÍNUA**

---

# Etapa 20 – Reflexão Final sobre o Ciclo BPM

A análise da Clínica Vida+ Saúde demonstra a importância de compreender o processo de negócio antes de iniciar o desenvolvimento de um sistema.

O ciclo BPM permite observar o processo de maneira estruturada, começando pelo planejamento, passando pela análise e modelagem, chegando à implementação, monitoramento e posterior refinamento.

No estudo de caso, a análise do processo AS-IS permitiu identificar problemas relacionados às planilhas, à comunicação, aos cadastros e ao controle dos horários.

A partir desses problemas foi possível elaborar um processo TO-BE, utilizando uma solução centralizada para apoiar o atendimento e o agendamento.

O monitoramento por meio de indicadores permite verificar se as mudanças realmente produziram os resultados esperados. Caso os resultados não sejam satisfatórios, o processo pode ser novamente analisado e refinado.

Assim, o ciclo BPM pode ser aplicado da seguinte maneira:

**Planejamento**
↓
Definição do objetivo e escopo

**Análise**
↓
Compreensão do processo atual e identificação dos problemas

**Desenho e Modelagem**
↓
Construção dos modelos AS-IS e TO-BE

**Implementação**
↓
Implantação da solução proposta

**Monitoramento e Controle**
↓
Acompanhamento dos indicadores

**Refinamento**
↓
Identificação de novas oportunidades de melhoria

---

# Conclusão

A análise da Clínica Vida+ Saúde demonstrou que o principal problema do processo atual está na fragmentação das informações e na dependência de atividades manuais.

A utilização de planilhas independentes favorece conflitos de horários, retrabalho, informações desatualizadas e falhas de comunicação com os pacientes.

A proposta de um sistema centralizado permite melhorar o processo por meio de uma agenda única, cadastro integrado, agendamento, cancelamento, confirmação, lembretes e indicadores.
