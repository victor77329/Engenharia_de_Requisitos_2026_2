# Perguntas sobre especificação de requisitos e modelagem

## Estudo do artigo Um Jogo Acessível para o Ensino de UML

## Estudante: Victor Gabriel Madeiro Brito Marques  Turma: B

Orientações: responda às 30 questões com base no artigo de Irvin Ken Xavier Tavares e Maria Amelia Eliseo. A atividade pode ser realizada em equipe. Fundamente as análises nas seções, tabelas ou figuras pertinentes. Nas atividades de especificação e modelagem, diferencie evidências do artigo, inferências e propostas suas. Registre as respostas e os diagramas em documento separado.
Análise do problema e elicitação

01. Qual problema educacional e de acessibilidade motivou o desenvolvimento do U.C. Battle e como esse problema pode ser traduzido em uma necessidade de negócio e em dois objetivos verificáveis do produto?
  O  probelma foi que muitos jogos não acessíveis e acabam gerando dificuldades para deficientes visuais. A necessidade de negócio é desenvolver um jogo que seja educativo e acessível. Dois objetivos verificáveis: levantar questionário para que os usuários respondam com base nas expêriencias de acessibilidade, implementar requisitos de acessibilidade.

02. Quais partes interessadas devem participar da elicitação dos requisitos de um jogo como o U.C. Battle? Identifique seus interesses e diferencie as partes mencionadas no artigo daquelas que você propõe incluir.
As partes interessadas são estudantes de engenharia de software, os desenvolvedores, professores e deficientes visuais. Os alunos querem aprender sem barreiras, os professores querem poder adaptar o conteúdo e os desenvolvedores querem critérios claros.

03. Como você delimitaria o escopo do U.C. Battle a partir do ensino de casos de uso, do combate, do modo treino e do book? Indique três funcionalidades do escopo descrito e duas possíveis ampliações que ficariam fora da versão estudada.
O escopo é um jogo web em que o jogador enfrenta 5 vilões respondendo charadas de múltipla escolha sobre casos de uso, com um modo treino sem penalidade e um book para revisar conceitos. Três funcionalidades são o combate com pontos de vida e habilidade de dica, o modo treino e o book com histórias sobre cenários, diagrama, generalização e include/extend. Duas ampliações fora da versão estudada, citadas como trabalhos futuros, são os professores adicionarem suas próprias perguntas e histórias, e a criação de uma narrativa para o jogo.

04. Quais técnicas de elicitação você combinaria para compreender as necessidades de estudantes com deficiência visual e de docentes de Engenharia de Requisitos? Justifique a escolha e formule três perguntas para uma entrevista com esses estudantes.Eu combinaria entrevistas com os estudantes, questionário com os docentes e prototipação com testes. As entrevistas captam o que as pessoas dizem e a observação mostra o que elas realmente fazem. Perguntas para os estudantes: que recursos você usa hoje para estudar UML e que dificuldades encontra? Como você prefere receber informações em um jogo, por narração, sons ou texto? Que tipo de desafio faria você querer continuar jogando?

05. Como a revisão bibliográfica e o estudo de diretrizes contribuíram para descobrir requisitos no artigo? Que necessidades de uso ainda exigiriam investigação direta com o público-alvo?
A revisão bibliográfica e o estudo de diretrizes (Cheiran e Pimenta e WCAG 2.1) deram ao artigo os conceitos de UML e jogos sérios e os requisitos de acessibilidade da Tabela 1, como teclado, narração, sem limite de tempo e tutorial. Ainda exigiriam investigação direta com o público-alvo o uso real por pessoas com deficiência visual, já que o teste foi com 26 alunos de computação, em sua maioria sem deficiência, além do contraste, dos títulos de página e das preferências de narração.

06. Que informações faltam para especificar a continuidade do progresso entre sessões, a repetição de charadas e o funcionamento da narração? Formule uma pergunta de esclarecimento para cada lacuna, sem presumir funcionalidades não descritas.
O artigo não esclarece três pontos. Sobre o progresso entre sessões, ele só diz que os vilões são desbloqueados ao vencer: o progresso é salvo ao fechar o jogo e, se for, como o jogador retoma? Sobre as charadas, diz apenas que “é feita outra charada”: como elas são escolhidas e a mesma podere aparecer na mesma batalha ou ao enfrentar o vilão de novo? Sobre a narração, só há a opção de ligar e desligar: ela usa voz própria ou o leitor de tela do sistema, e o jogador pode ajustar velocidade, pausar ou repetir?
 
Especificação de requisitos e regras de negócio
Estudo de caso U.C. Battle

07. Como você reescreveria três requisitos funcionais apresentados na seção 3 para torná-los atômicos, claros e verificáveis? Atribua identificadores e indique a entrada, o comportamento esperado e o resultado de cada requisito.
RF01 - O software deverá decrementar um ponto de vidado vilão quando o usuário acertar uma charada na batalha. (Entrada: o jogador escolhe a alternativa correta; Comportamento: o sistema reduz em 1 ponto a vida do vilão; Resultado: a vida do vilão exibida éa anterior menos 1.) RF02 - O software deverá decrementar um ponto de vida do herói quando o usuário errar uma charada na batalha. (Entrada: o jogador escolhe uma alternativa incorreta;Comportamento: o sistema reduz em 1 ponto a vida do herói; Resultado: a vida do herói exibida é a anterior menos 1.) RF03 - O software deverá apresentar uma nova charada após o usuário escolher uma resposta na batalha. (Entrada: o jogador escolhe qualquer alternativa; Comportamento: o sistemasubstitui a charada atual por outra; Resultado: a nova charada aparece na tela com pergunta e quatroalternativas.)

08. Como você distinguiria requisitos funcionais, requisitos de qualidade, regras de negócio e decisões de implementação no artigo? Apresente um exemplo de cada categoria e justifique, considerando que um recurso de acessibilidade também pode exigir comportamento funcional.
Requisitos funcionais são as ações do sistemas a partir das interações do usuário. Requisito de qualidade é uma propriedade de como o sistema opera, que não depende de uma ação específica do usuário. Regra de negócio é a regra do jogo que define as condições e os valores. Decisão de implementação é uma escolha técnica sobre como o sistema é construído, e não sobre o que ele faz ou com que qualidade.

09. Como especificar a regra da habilidade do herói, considerando o limite de uma utilização por batalha e a condição de possuir dois pontos de vida ou menos? Redija a regra e dois requisitos funcionais que a operacionalizem.
O herói pode usar a habilidade uma única vez por batalha, apenas se tiver 2 ou menos pontos de vida, eo efeito é receber uma dica sobre a charada atual. RF-A: ao acionar a habilidade (entrada), o Sistema verifica a vida do herói e, se ela for menor ou igual a 2 e a habilidade ainda não tiver sido usada na batalha, exibe a dica da charada atual e marca a habilidade como usada. RF-B:se a vida for maior que 2 ou a habilidade já tiver sido usada, o sistema não exibe a dica e informa o motivo.

10. Como transformar a descrição do combate em regras de negócio para os pontos de vida iniciais, o efeito de acertos e erros e o encerramento da batalha? Explicite também como determinar a vida inicial de cada um dos cinco vilões.
O herói começa cada batalha com 4 pontos de vida; cada acerto reduz 1ponto do vilão e cada erro reduz 1 ponto do herói, seguidos de nova charada; batalha termina quando a vida de um dos dois chega a zero. A vida inicial do vilão é 3 para o primeiro e aumenta 1 a cada novo vilão.

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

17. Como os princípios perceptível, operável, compreensível e robusto podem orientar a revisão dos requisitos do jogo? Relacione um requisito da Tabela 1 a cada princípio e explique a evidência necessária para verificá-lo.
   Aplicados separadamente, os princípios revisam o requisito pelo ângulo de um só critério. Juntos, eles revisam a experiencia do jogador, do momento em que a informação chega até o momento em que ele age e entende o resultado.

18. Como registrar e analisar a redução de 29 diretrizes inicialmente consideradas para 21 estudadas e implementadas? Proponha os campos de um registro de decisão e explique como avaliar o impacto das exclusões sobre a acessibilidade e o escopo.
 
Modelagem de casos de uso
Estudo de caso U.C. Battle

19. Como você definiria a fronteira do sistema e os atores no diagrama de casos de uso do U.C. Battle? Explique por que herói, mestre e vilões da narrativa não devem ser automaticamente tratados como  atores externos.
   A fronteira separa o que o sistema controla (o que será construído e testado). Um ator é um papel que interage com o sistema para obter um resultado. Ele é definido por quem inicia ou recebe valor de uma interação. Herói, mestre e vilões pertencem à narrativa. Um ator de caso de uso representa quem está fora do sistema e interage com ele. O herói é o avatar que o jogador controla: quem age é o jogador, e o herói é a forma como o sistema representa essa ação.

20. Como o diagrama da Figura 2 representa os objetivos do jogador? Compare-o com os requisitos funcionais da seção 3 e identifique duas funcionalidades ou condições que precisam de detalhamento textual, justificando onde documentá-las.

21. Como você escreveria a especificação textual do caso de uso “Responder charada”? Inclua objetivo, ator principal, gatilho, precondições, fluxo principal, alternativas para acerto e erro e pós-condições.
Objetivo: permitir que o jogador possa responder as charadas do vilão e que resultado afete a batalha.
Ator principal: Jogador.
Gatilho: O sistema apresenta uma charada no turno do jogador durante a batalha.
Precondições: Há uma batalha em andamento, e o turno do jogador, existe uma charada não respondida
ainda.
Fluxo principal: O sistema mostra o enunciado das charadas e as opções, o jogador seleciona ou
responde as questões, o sistema compara as respostas com gabarito, o sistema identifica se a resposta
está correta, o sistema aplica o efeito, o sistema atualiza o estado da batalha e encerra o turno do
jogador.
Acerto e erro e pós-condições:(Acerto): o sistema exibe o acerto e aplica o efeito.
(Erro): o sistema informa o erro e mostra a resposta correta.
(Pós-condição): (Acerto): a pontuação ou a vida do vilão e atualizada e o turno foi encerrado
(Erro): a vida do jogador foi atalizada e o turno foi encerrado

22. Como você especificaria o caso de uso “Usar habilidade”? Descreva o fluxo de sucesso e os tratamentos para vida acima do limite permitido e tentativa de segunda utilização na mesma batalha.
O jogador seleciona a opção “Usar habilidade”, o sistema verifica se a vida atual está dentro do limite
permitido, o sistema verifica se a habilidade foi usada nesta batalha, o sistema aplica o efeito, o sistema
marca habilidade como usada nesta batalha, o sistema atualiza o estado da batalha e exibe o resultado.
Vida fora do limite: o sistema informa que a habilidade não pode ser usada nessas condições, mostrando
a vida atual e o limite. A habilidade não é consumida e o jogador volta ao menu de ações do turno.
Habilidade ja utilizada: o sistema informa que a habilidade só pode ser usada uma vez por batalha. Nada
é alterado e o jogador volta ao menu de ações.

23. Como você avaliaria a relação «include» entre “Render-se” e “Voltar ao menu principal” na Figura 2? Justifique sua manutenção ou alteração com base no significado de «include» e na possibilidade de registrar o retorno como passo do fluxo.
O «include» expressa um comportamento obrigatório, coeso e reutilizável, que o caso de uso base
incorpora para cumprir seu objetivo. Costuma ser usado para evitar repetição entre vários casos de uso.
“Voltar ao menu principal” não é um objetivo do jogador com valor próprio. É só a consequência de
navegação após a rendição.
Quando manteria um «include»: apenas se vários casos de compartilhassem um comportamento mais
rico, como “Encerrar batalha e registrar resultado”. Nesse caso o «include» apontaria para esse
comportamento coeso, e não para a simples navegação.

24. Como você remodelaria os casos de uso de consultar temas do book, treinar e enfrentar um vilão para expressar objetivos do jogador? Desenhe um diagrama e justifique as associações e eventuais relações «include» ou «extend», sem usá-las apenas para indicar ordem de navegação.
 <img width="624" height="291" alt="Image" src="https://github.com/user-attachments/assets/d8898c1a-fe9f-4393-a74a-5398bed5dcae" />

25. Como um diagrama de atividades pode representar uma batalha do U.C. Battle? Modele seleção de resposta, atualização dos pontos de vida, solicitação de dica e encerramento, com decisões e guardas coerentes com as regras descritas
<img width="497" height="389" alt="Image" src="https://github.com/user-attachments/assets/854d3c11-653f-475b-8636-452632cdca56" />

26. Como você representaria o ciclo de uma batalha em um diagrama de estados? Defina estados, eventos e guardas para início, espera por resposta, vitória, derrota e rendição, distinguindo eventos de condições.
Estados: Preparando, Em batalha (com Aguardando resposta, Exibindo dica e Avaliando resposta dentro),
Vitória, Derrota e Rendição. Os três últimos são finais.
Eventos (o que acontece e dispara a transição): iniciarBatalha, batalhaPronta, pedirDica, fecharDica,
responder(opção), respostaProcessada e renderSe.
Guardas (condições avaliadas quando o evento ocorre): [dicas &gt; 0], [vida do vilão ≤ 0], [vida do jogador ≤
0], [os dois com vida &gt; 0] e [jogador confirmou].
Ideia central: vitória e derrota não são eventos, e sim resultado de guardas sobre a vida, avaliadas depois
de processar a resposta. A rendição sai de “Em batalha” inteiro, valendo em qualquer subestado.


27. Como você elaboraria um diagrama de sequência para o cenário em que o jogador acerta uma charada? Proponha participantes e mensagens para registrar a resposta, verificar o acerto, atualizar a vida do vilão e apresentar o resultado; identifique os elementos de projeto que não estão definidos no artigo.
<img width="632" height="385" alt="Image" src="https://github.com/user-attachments/assets/489d2d05-0529-4f91-b984-4f81f426686f" />

28. Como você construiria uma matriz de rastreabilidade para quatro requisitos do jogo, incluindo dois de acessibilidade? Relacione cada requisito à origem no artigo, ao caso de uso ou elemento do modelo pertinente e a um teste de aceitação.
<img width="659" height="253" alt="Image" src="https://github.com/user-attachments/assets/120bf039-11aa-4c9e-a5d7-e19d8d10476b" />

29. Até que ponto os questionários aplicados aos 26 estudantes demonstram atendimento aos requisitos de acessibilidade? Diferencie percepção dos participantes, verificação técnica e participação de pessoas com deficiência visual; proponha verificações adicionais sem presumir que esse perfil foi confirmado na amostra.
Três coisas distintas:
Percepção dos participantes: opinião subjetiva, sujeita a viés de cortesia e de familiaridade. Com 26
estudantes, é indicativa, sem poder estatístico para generalizar.
Verificação técnica: conferir objetivamente se o sistema cumpre critérios verificáveis (contraste,
compatibilidade com leitor de tela, navegação por teclado, texto alternativo). Questionário nenhum
substitui isso.
Participação de pessoas com deficiência visual: só quem usa tecnologia assistiva no dia a dia revela
barreiras reais. Opinião de estudantes videntes sobre acessibilidade não equivale a isso.
Verificações adicionais:
Auditoria técnica com checklist (contraste, rótulos, ordem de foco, alternativas textuais).
Testes com leitores de cumprindo tarefas reais, como responder uma charada e usar a dica.
Teste de navegação só por teclado, sem mouse.
Teste de usabilidade com pessoas com deficiência visual recrutadas de propósito, medindo taxa de
conclusão de tarefas, tempo e erros, além da satisfação.
Revisão por especialista em acessibilidade.

30. Como você organizaria uma revisão final de consistência entre requisitos, regras de negócio, casos de uso e demais modelos? Apresente um exemplo de inconsistência que procuraria e analise o impacto de uma mudança hipotética que permitisse usar a habilidade duas vezes por batalha.
Inventário: listar os artefatos (requisitos, regras de negócio, casos de uso, atividades, estados, sequência,matriz) com identificadores estáveis.Checagem cruzada por pares: requisito regra, regra caso de uso, caso de uso diagramascomportamentais, requisito teste. A matriz de rastreabilidade (28) é o instrumento principal.Verificar vocabulário: o mesmo conceito com o mesmo nome em todo lugar (ex.: “habilidade” vs.“poder”). Verificar completude: regra sem caso de uso, requisito sem teste, estado sem saída. Registrar achados com severidade e responsável, corrigir na fonte e propagar para os demais artefatos.




 

