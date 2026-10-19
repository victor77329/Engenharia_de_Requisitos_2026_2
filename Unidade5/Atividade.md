Perguntas sobre especificação de requisitos e modelagem
Estudo do artigo Um Jogo Acessível para o Ensino de UML
Estudante: Victor Gabriel Madeiro Brito Marques  Turma: B
Orientações: responda às 30 questões com base no artigo de Irvin Ken Xavier Tavares e Maria Amelia Eliseo. A atividade pode ser realizada em equipe. Fundamente as análises nas seções, tabelas ou figuras pertinentes. Nas atividades de especificação e modelagem, diferencie evidências do artigo, inferências e propostas suas. Registre as respostas e os diagramas em documento separado.
Análise do problema e elicitação
01. Qual problema educacional e de acessibilidade motivou o desenvolvimento do U.C. Battle e como esse problema pode ser traduzido em uma necessidade de negócio e em dois objetivos verificáveis do produto?  Nicolle Da Silva Coelho respondeu.
02. Quais partes interessadas devem participar da elicitação dos requisitos de um jogo como o U.C. Battle? Identifique seus interesses e diferencie as partes mencionadas no artigo daquelas que você propõe incluir.   Nicolle Da Silva Coelho respondeu.
03. Como você delimitaria o escopo do U.C. Battle a partir do ensino de casos de uso, do combate, do modo treino e do book? Indique três funcionalidades do escopo descrito e duas possíveis ampliações que ficariam fora da versão estudada.   Nicolle Da Silva Coelho respondeu.
04. Quais técnicas de elicitação você combinaria para compreender as necessidades de estudantes com deficiência visual e de docentes de Engenharia de Requisitos? Justifique a escolha e formule três perguntas para uma entrevista com esses estudantes.  Nicolle Da Silva Coelho respondeu.
05. Como a revisão bibliográfica e o estudo de diretrizes contribuíram para descobrir requisitos no artigo? Que necessidades de uso ainda exigiriam investigação direta com o público-alvo?   Nicolle Da Silva Coelho respondeu.
06. Que informações faltam para especificar a continuidade do progresso entre sessões, a repetição de charadas e o funcionamento da narração? Formule uma pergunta de esclarecimento para cada lacuna, sem presumir funcionalidades não descritas.   Nicolle Da Silva Coelho respondeu.
 
Especificação de requisitos e regras de negócio
Estudo de caso U.C. Battle
07. Como você reescreveria três requisitos funcionais apresentados na seção 3 para torná-los atômicos, claros e verificáveis? Atribua identificadores e indique a entrada, o comportamento esperado e o resultado de cada requisito. Nicolle Da Silva Coelho respondeu
08. Como você distinguiria requisitos funcionais, requisitos de qualidade, regras de negócio e decisões de implementação no artigo? Apresente um exemplo de cada categoria e justifique, considerando que um recurso de acessibilidade também pode exigir comportamento funcional. Nicolle Da Silva Coelho respondeu.

09. Como especificar a regra da habilidade do herói, considerando o limite de uma utilização por batalha e a condição de possuir dois pontos de vida ou menos? Redija a regra e dois requisitos funcionais que a operacionalizem. Nicolle Da Silva Coelho respondeu.

10. Como transformar a descrição do combate em regras de negócio para os pontos de vida iniciais, o efeito de acertos e erros e o encerramento da batalha? Explicite também como determinar a vida inicial de cada um dos cinco vilões. Nicolle Da Silva Coelho respondeu.

11. Como você especificaria o desbloqueio de fases após uma vitória e a possibilidade de enfrentar novamente um vilão após uma derrota? Indique condições, resultados esperados e uma ambiguidade que exigiria confirmação com as partes interessadas.
    Ao avançar em uma fase, a fase seguinte é desbloqueada. Quando o jogador passa de fase e de um vilão, a fase e vilão anterior passa a ficar disponível novamente para ser jogada, quando ele repete a fase nenhum desbloqueio de fase ocorre, porém as recompensas são resgatadas novamente. E existe possibilidade de revanche, onde o jogador pode retornar onde morreu e refazer a fase novamente e enquanto não cumprir os requisitos para passar, a fase seguinte permanecerá bloqueada.
12. Que diferenças devem existir entre o modo treino e a batalha quanto a erros e penalidades? Escreva dois requisitos para o treino e proponha critérios de aceitação que permitam verificar a ausência de penalização.
    Na batalha o erro pode ser fatal, o jogador irá perder vida, podendo ser derrotado, gasta seus recursos, e isso afeta seu progresso e ranking. No treino o erro pode e deve ocorrer, não afetará seu progresso e poderá treinar suas habilidades. RQ01 – No treino o jogador não poderá perder vida e recursos, e se a vida chegar a zero o treino e reiniciado automáticamente. RQ02 – O treino não afeta o progresso da história.
 
Acessibilidade e qualidade da especificação
Estudo de caso U.C. Battle
13. Como transformar a diretriz de operação completa por teclado, apresentada na Tabela 1, em um requisito verificável? Defina o escopo da navegação, o comportamento do foco e um procedimento de teste, identificando os detalhes que você está propondo.
14. Como especificar a narração de perguntas, alternativas, dicas e conteúdo do book, descrita nos resultados? Proponha critérios de aceitação para ativação e desativação e identifique comportamentos que ainda precisariam ser esclarecidos. 
   Essa função é necessária para pessoas com deficiencia conseguirem jogar, e ter a opção de ativar e desativar, para atender individualmente cada usuário.
15. Como verificar o requisito de não utilizar apenas cores para transmitir informação? Proponha uma solução para comunicar acerto, erro, vitória e derrota e descreva como testar se as mensagens continuam compreensíveis sem distinguir as cores.
   As mensangem podem ser escritas por texto, ícone, padrão, posição ou som. Porém o ideal e as cores aparecem junto ao texto para fácil compreensão e visualização rápida.
16. Por que expressões como “contraste adequado” e “progressão natural de dificuldade” são insuficientes para uma especificação verificável? Reescreva cada uma com condições e critérios mensuráveis propostos, sem atribuir seus valores ao artigo.
   Elas são subjetivas pois, depende de quem avalia essas expressões, do contexto e expereincia de cada usuário. Reescritas de maneira adequada o contraste seria: Em todas as telas do escopo, texto e elementos gráficos informativos devem atingir razão de contraste mínima em relação ao fundo imediato, medida com ferramenta de contraste. Em progressão: A dificuldade das fases deve crescer de forma gradual e sem saltos bruscos, medida por indicadores de desempenho dos jogadores em cada fase, dentro de faixas-alvo e com limite para variação entre fases consecutivas.
17. Como os princípios perceptível, operável, compreensível e robusto Como os princípios perceptível, operável, compreensível e robusto podem orientar a revisão dos requisitos do jogo? Relacione um requisito da Tabela 1 a cada princípio e explique a evidência necessária para verificá-lo.
      Aplicados separadamente, os princípios revisam o requisito pelo ângulo de um só critério. Juntos, eles revisam a experiencia do jogador, do momento em que a informação chega até o momento em que ele age e entende o resultado.
    
18. Como registrar e analisar a redução de 29 diretrizes inicialmente consideradas para 21 estudadas e implementadas? Proponha os campos de um registro de decisão e explique como avaliar o impacto das exclusões sobre a acessibilidade e o escopo.
 
Modelagem de casos de uso
Estudo de caso U.C. Battle
19. Como você definiria a fronteira do sistema e os atores no diagrama de casos de uso do U.C. Battle? Explique por que herói, mestre e vilões da narrativa não devem ser automaticamente tratados como atores externos.
     A fronteira separa o que o sistema controla (o que será construído e testado). Um ator é um papel que interage com o sistema para obter um resultado. Ele é definido por quem inicia ou recebe valor de uma interação. Herói, mestre e vilões pertencem à narrativa. Um ator de caso de uso representa quem está fora do sistema e interage com ele. O herói é o avatar que o jogador controla: quem age é o jogador, e o herói é a forma como o sistema representa essa ação.
20. Como o diagrama da Figura 2 representa os objetivos do jogador? Compare-o com os requisitos funcionais da seção 3 e identifique duas funcionalidades ou condições que precisam de detalhamento textual, justificando onde documentá-las.
21. Como você escreveria a especificação textual do caso de uso “Responder charada”? Inclua objetivo, ator principal, gatilho, precondições, fluxo principal, alternativas para acerto e erro e pós-condições.
22. Como você especificaria o caso de uso “Usar habilidade”? Descreva o fluxo de sucesso e os tratamentos para vida acima do limite permitido e tentativa de segunda utilização na mesma batalha.
23. Como você avaliaria a relação «include» entre “Render-se” e “Voltar ao menu principal” na Figura 2? Justifique sua manutenção ou alteração com base no significado de «include» e na possibilidade de registrar o retorno como passo do fluxo.
24. Como você remodelaria os casos de uso de consultar temas do book, treinar e enfrentar um vilão para expressar objetivos do jogador? Desenhe um diagrama e justifique as associações e eventuais relações «include» ou «extend», sem usá-las apenas para indicar ordem de navegação.
 
Modelagem complementar e validação
Estudo de caso U.C. Battle
25. Como um diagrama de atividades pode representar uma batalha do U.C. Battle? Modele seleção de resposta, atualização dos pontos de vida, solicitação de dica e encerramento, com decisões e guardas coerentes com as regras descritas.
26. Como você representaria o ciclo de uma batalha em um diagrama de estados? Defina estados, eventos e guardas para início, espera por resposta, vitória, derrota e rendição, distinguindo eventos de condições.
27. Como você elaboraria um diagrama de sequência para o cenário em que o jogador acerta uma charada? Proponha participantes e mensagens para registrar a resposta, verificar o acerto, atualizar a vida do vilão e apresentar o resultado; identifique os elementos de projeto que não estão definidos no artigo.
28. Como você construiria uma matriz de rastreabilidade para quatro requisitos do jogo, incluindo dois de acessibilidade? Relacione cada requisito à origem no artigo, ao caso de uso ou elemento do modelo pertinente e a um teste de aceitação.
29. Até que ponto os questionários aplicados aos 26 estudantes demonstram atendimento aos requisitos de acessibilidade? Diferencie percepção dos participantes, verificação técnica e participação de pessoas com deficiência visual; proponha verificações adicionais sem presumir que esse perfil foi confirmado na amostra.
30. Como você organizaria uma revisão final de consistência entre requisitos, regras de negócio, casos de uso e demais modelos? Apresente um exemplo de inconsistência que procuraria e analise o impacto de uma mudança hipotética que permitisse usar a habilidade duas vezes por batalha.
Fonte das questões: TAVARES, Irvin Ken Xavier; ELISEO, Maria Amelia. Um Jogo Acessível para o Ensino de UML. Artigo fornecido para a atividade, especialmente seções 2.2, 2.3, 3 e 4, Tabela 1 e Figura 2.
