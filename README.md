# **RAF:** Robô Autônomo de Farmácia

Trabalho de Interação Humano-Robô (IHR) apresentado ao Centro Universitário [FEI](https://portal.fei.edu.br/), como parte dos requisitos necessários para aprovação na disciplina de Interação Humano-Robô (IHR) (CCR230) do curso de Engenharia de Robôs, orientado pelo Prof. Dr. [Fagner de Assis Moura Pimentel](https://github.com/fagnerpimentel).

## Componentes do Grupo
 - Diego Gomes - 11.122.256-8
 - Miguel Savordelli - 11.122.007-5
 - Vinicius Grec - 11.122.375-6

## Resumo

O robô farmacêutico é um sistema robótico desenvolvido para automatizar o processo de separação e entrega de medicamentos em farmácias. Sua principal função é localizar e retirar os remédios armazenados em prateleiras, transportando-os até um balcão de atendimento, onde ficam disponíveis para serem entregues ao cliente ou ao funcionário responsável.

O robô pode utilizar sensores e sistemas de visão computacional para identificar os medicamentos, localizar suas posições nas prateleiras e realizar a movimentação com precisão. Além disso, pode contar com mecanismos de manipulação, como garras, para pegar e transportar os produtos com segurança.

A implementação desse sistema tem como objetivo reduzir o tempo de atendimento, diminuir erros na separação de medicamentos, otimizar a organização dos produtos e reduzir o esforço dos funcionários em tarefas repetitivas. Dessa forma, o robô atua como um auxiliar no ambiente farmacêutico, tornando o processo de atendimento mais ágil, eficiente e organizado.


## Introdução

Atualmente, as farmácias lidam diariamente com uma grande quantidade de medicamentos armazenados em prateleiras, o que exige que os funcionários realizem constantemente tarefas de localização, separação e transporte dos produtos até o balcão de atendimento. Esse processo pode gerar filas, aumentar o tempo de espera dos clientes e sobrecarregar os funcionários, principalmente em horários de maior movimento. Nesse contexto, a automação dessas atividades torna-se uma alternativa importante para melhorar a eficiência e a agilidade dos estabelecimentos.

O RAF é um robô desenvolvido para auxiliar no atendimento farmacêutico, tendo como principal função localizar e retirar medicamentos das prateleiras e transportá-los até o balcão de atendimento. Por meio de sensores e mecanismos de manipulação, o robô deverá identificar os produtos solicitados e realizar sua entrega de maneira autônoma e precisa.

Objetivo: automatizar a separação e o transporte de medicamentos das prateleiras até o balcão, reduzindo o tempo de atendimento e o esforço dos funcionários.

Experiência desejada: proporcionar uma experiência rápida, segura e intuitiva, transmitindo confiança aos funcionários e clientes, além de tornar o processo de atendimento mais eficiente e organizado.

## Público-Alvo e Stakeholders
### Público-Alvo
O público-alvo do RAF (Robô Autônomo de Farmácia) são farmácias, drogarias e estabelecimentos que trabalham com armazenamento e comercialização de medicamentos, especialmente aqueles que possuem grande variedade de produtos e alto fluxo de atendimento. O robô também será utilizado indiretamente por farmacêuticos e atendentes, auxiliando na separação e no transporte dos medicamentos até o balcão, além de beneficiar os clientes com um atendimento mais ágil.

### Stakeholders
Primários — farmacêuticos e atendentes da farmácia, que interagem diretamente com o RAF, solicitando a busca e a entrega dos medicamentos no balcão.

Secundários — clientes e demais funcionários da farmácia, que possuem contato indireto com o robô e são beneficiados pela redução do tempo de espera e pela agilidade no atendimento.

Terciários — proprietários e gerentes das farmácias, responsáveis pela implementação e manutenção do sistema, além de fornecedores de medicamentos e profissionais responsáveis pela organização do estoque, que podem ser impactados pelas mudanças nos processos internos.

### Personas
Persona primária — Mariana, 32 anos: farmacêutica responsável por uma drogaria de médio porte, com grande variedade de medicamentos e fluxo constante de clientes. Precisa localizar e separar diversos medicamentos ao longo do dia, conciliando o atendimento ao público com outras responsabilidades. Busca agilidade, precisão e redução de tarefas repetitivas. Antes de iniciar uma tarefa, o RAF deve saber qual medicamento foi solicitado, sua localização no estoque e a quantidade necessária.

Persona secundária — João, 24 anos: atendente de farmácia, responsável por auxiliar os clientes e separar os medicamentos solicitados pelos farmacêuticos. Trabalha em horários de grande movimento e frequentemente precisa percorrer diferentes prateleiras para encontrar os produtos. Possui familiaridade com tecnologias, mas não necessariamente conhecimentos técnicos sobre robótica. Espera que o RAF seja simples de operar, rápido e confiável. Antes de iniciar a tarefa, o robô deve receber o nome ou código do medicamento e o local de entrega.

### Mapa de empatia

![Mapa de empatia](empatia.png)

Persona: Mariana, 32 anos, farmacêutica responsável por uma drogaria.

- O que ela PENSA E SENTE?
-   Deseja garantir um atendimento rápido e eficiente.
-   Preocupa-se com a precisão na separação dos medicamentos.
-   Busca melhorar a produtividade da farmácia.
O que ela ESCUTA?
- Clientes reclamando da demora.
- Funcionários relatando dificuldades na rotina.
- Gerentes cobrando qualidade no atendimento.
O que ela VÊ?
- Grande variedade de medicamentos nas prateleiras.
- Funcionários ocupados procurando produtos.
- Filas em horários de maior movimento.
O que ela FALA E FAZ?
- Orienta os atendentes na separação dos medicamentos.
- Confere prescrições e produtos.
- Supervisiona o funcionamento da farmácia.
DORES
- Demora na localização dos medicamentos.
- Sobrecarga dos funcionários.
- Risco de erros na separação dos produtos.
GANHOS
- Maior agilidade no atendimento.
- Redução de erros operacionais.
- Melhor aproveitamento do tempo dos funcionários.
  
Persona: João, 24 anos, atendente de farmácia.
O que ele PENSA E SENTE?
- Deseja atender os clientes com rapidez.
- Preocupa-se em separar os medicamentos corretamente.
- Sente pressão em horários de grande movimento.
O que ele ESCUTA?
- Clientes reclamando da demora.
- Farmacêuticos solicitando medicamentos.
- Gerentes cobrando produtividade.
O que ele VÊ?
- Prateleiras com muitos medicamentos.
- Clientes aguardando atendimento.
- Funcionários procurando produtos constantemente.
O que ele FALA E FAZ?
- Procura medicamentos nas prateleiras.
- Confere os produtos antes da entrega.
- Busca agilizar o atendimento.
DORES
- Demora para localizar medicamentos.
- Sobrecarga de tarefas.
- Cansaço pela movimentação constante.
GANHOS
- Agilidade na separação dos medicamentos.
- Redução do esforço físico.
- Mais tempo para atender os clientes.

## Contexto de uso

> 💡
> - Descreva o ambiente em que o robô interage com os usuários
> - Qual/quais o(s) contexto(s) sociais, econômicos e culturais existentes neste ambiente?
> - Quais informações sobre o ambiente o robô deve saber antes de iniciar a tarefa?

<details>
<summary>📄</summary>

Saguão de entrada e corredores do prédio principal da FEI, durante o FEI Portas Abertas (evento de um único dia, com alta lotação). O ambiente é barulhento e há vários grupos de visitantes circulando ao mesmo tempo, muitos acompanhados de monitores humanos. O robô precisa saber, antes de começar, o mapa dos laboratórios abertos naquele dia e quais estão temporariamente fechados.

</details>

## Jornada do usuário

> 💡
> - Criar uma narrativa para o o seu robô e o usuário.
> - Determine o passo a passo que o usuário realiza desde o primeiro até o último encontro com robô na realização da tarefa.
> - O que está acontecendo com o ambiente quando o robô está interagindo com o usuário?
>   - Descreva o que acontece ou pode acontecer passo a passo
>   - Como a tarefa começa? Como a tarefa evolui? Como a tarefa termina?
> - Enfatize todos os momentos em que acontece uma interação verbal, não-verbal e espacial.

<details>
<summary>📄</summary>

1. Ana e o pai entram no saguão e ficam parados olhando ao redor, sem saber para onde ir.
2. O Rumo percebe o grupo parado (sinal de "perdido") e se aproxima devagar, pela frente, mantendo distância social *(espacial)*.
3. O robô pergunta "Posso ajudar vocês a encontrar algum curso ou laboratório?" e mostra um menu de ícones na tela *(verbal)*.
4. Ana toca em "Engenharia de Robôs"; o robô confirma e começa a andar, olhando de tempos em tempos para trás para checar se o grupo o segue *(espacial + não-verbal)*.
5. No corredor, o robô encontra duas pessoas conversando e contorna sem passar entre elas *(espacial)*.
6. Ao chegar no laboratório, o robô se vira de frente para o grupo, inclina levemente a "cabeça" e deseja uma boa visita *(não-verbal)*.

</details>

## Análise de concorrência

> 💡
> - Pesquise robôs existentes atualmente que possam fazer a tarefa deste projeto.
> - Selecione pelo menos 3 robôs diferentes que podem fazer essa tarefa.
> - Em relação aos concorrentes, respondam as seguintes perguntas:
>   - Existe plataforma similar que atende o mesmo mercado e funcionalidades? Se sim: Quais os pontos positivos? Quais os pontos negativos?
>   - Existe plataforma diferente quanto ao serviço, mas que atenda esse mercado? Se sim: Quais os pontos positivos? Quais os pontos negativos?
>   - Quais plataformas sua equipe acha mais interessantes? Qual a justificativa?

<details>
<summary>📄</summary>

- **Totens interativos de informação** (comuns em aeroportos e shoppings) — bons para consultar informação estática, mas não guiam fisicamente o visitante até o destino.
- **Aplicativo de mapa indoor do campus** — dispensa hardware físico, mas perde o acolhimento social que um robô oferece a um visitante inseguro.
- **Pepper (SoftBank Robotics)**, usado em recepções comerciais — proposta muito parecida (recepcionar e guiar), mas é caro e não é sob medida para o layout da FEI.

A equipe considera o Pepper a referência mais próxima, mas acredita que um robô mais simples e barato (sem braços articulados) atende igualmente bem ao caso de uso do FEI Portas Abertas.

</details>

## Design do Robô

### Forma, função e affordances

> 💡
> - Pense nas características de affordances do seu robô. Que tipo de acessibilidades devem ser consideradas dentro do seu projeto?
> - A aparência e o comportamento do robô **casam com a função**? Que affordances a forma sinaliza (olhos → enxergar, braços → pegar objetos, tela → interagir por toque)?
> - Discuta o papel das expectativas do usuário no projeto de um robô. Onde faz sentido "**prometer menos e entregar mais**" (underpromise, overdeliver)?

<details>
<summary>📄</summary>

O Rumo tem uma tela no "peito" (affordance de toque), uma "cabeça" com dois pontos luminosos (olhos) que sinalizam para onde está olhando, e **não** tem braços — o que sinaliza corretamente que ele não manipula objetos, apenas informa e guia. Para "prometer menos, entregar mais", o robô nunca é chamado de "assistente inteligente" nos materiais do evento, apenas de "guia do FEI Portas Abertas", evitando a expectativa de uma conversa livre e aberta.

</details>

### Grau de antropomorfismo

> 💡
> - O seu robô tem um padrão com mais ou menos características antropomórficas (androide, humanoide, zoomórfico, minimalista, robject)? Marquem um ponto no espectro máquina ↔ humano e justifiquem.
> - Qual padrão é mais aceito pela sociedade dentro do projeto que você está desenvolvendo?
> - Como o grupo pretende evitar o **vale da estranheza** (uncanny valley), caso o robô tenha um design muito próximo do humano?

<details>
<summary>📄</summary>

O Rumo fica próximo do polo **minimalista** do espectro, com leve antropomorfismo (olhos, "cabeça" que gira), sem rosto detalhado nem fala emocional complexa — parecido com o Keepon citado na aula de Design. Justificativa: um design fortemente humano geraria expectativa de conversa fluida, que o robô não tem; pouco antropomorfismo, por outro lado, dificultaria que visitantes se sintam à vontade para abordá-lo. Por ficar longe do polo humano, o risco de vale da estranheza é baixo.

</details>

### Padrões de design

> 💡
> Identifique **2 padrões de design** (design patterns) aplicáveis ao seu projeto e explique como eles se **combinam**.

<details>
<summary>📄</summary>

**"Apresentação inicial"** (o robô se apresenta brevemente antes de perguntar o destino) + **"em movimento junto"** (anda ao lado/à frente do grupo, ajustando o ritmo ao visitante mais lento) — combinados, formam o padrão composto de "robô guia turístico".

</details>

### Valores e ética

> 💡
> - Aplicando o **Value-Sensitive Design (VSD)** — a tecnologia deve se adaptar às necessidades humanas, não o contrário — identifique **1 a 2 valores** em jogo no seu projeto (privacidade, autonomia, segurança, inclusão, etc.).
> - Identifique **1 risco ético** do seu robô e como o grupo pretende mitigá-lo.

<details>
<summary>📄</summary>

**Valores:** acessibilidade (o robô deve ajustar a velocidade para visitantes com mobilidade reduzida) e privacidade (não deve gravar ou reconhecer rostos sem consentimento).

**Risco ético:** o robô poderia, sem querer, direcionar mais visitantes para cursos "badalados", reduzindo a visibilidade de cursos menos procurados. **Mitigação:** o menu de destinos sempre mostra todos os cursos na mesma ordem e tamanho, sem personalização por popularidade.

</details>

### Protótipo no papel

> 💡
> Modele o seu robô com desenhos de formas primitivas (caixas, cilindros, esferas): forma, tamanho, rosto/olhos, partes móveis, tela. É o protótipo mais barato e rápido — lembre-se do lema "**teste cedo, teste sempre**".
>

<details>
<summary>📄</summary>

 Corpo afunilado sobre uma base omnidirecional (três rodas onidirecionais, em arranjo triangular); "cabeça" arredondada com dois olhos, uma antena/sensor no topo; tela na parte de cima do torso, com o nome do robô; sem braços — apenas um anel de luz na base para sinalizar status. Altura total ≈1,55 m; diâmetro da base ≈0,90 m.

<img alt="Esboço do robô Rumo - V1'" src="rumo_esboco_v1.png" height="380"/>
<img alt="Esboço do robô Rumo - V2'" src="rumo_esboco_v2.png" height="380"/>
<img alt="Esboço do robô Rumo - V3'" src="rumo_esboco_v3.png" height="380"/>

</details>

## Ações do robô

> 💡
> Para cada ação:
> - Descreva a ação.
> - Determine os pré-requisitos para que a ação aconteça
> - Determine o que se espera que seja modificado no ambiente quando a ação é finalizada

<details>
<summary>📄</summary>

**Guiar até o destino** — pré-requisito: destino escolhido no menu e caminho livre conhecido no mapa do dia. Ao finalizar: o visitante está fisicamente no laboratório e o robô retorna à posição de espera no saguão.

**Dar informação rápida** — pré-requisito: pergunta reconhecida dentro do conjunto de perguntas frequentes cadastradas. Ao finalizar: a resposta foi falada e também exibida na tela.

</details>

## Interações do robô

### Espacial

> 💡
> - Descreva **onde** o robô se posiciona em relação ao usuário (distância e orientação do corpo), usando as **zonas de proxêmica** (Hall) e as **F-formations**.
> - Como o robô **inicia** a interação (direção de aproximação) e como **sinaliza** para onde vai?
> - Para cada interação espacial:
>   - Descreva a interação.
>   - Determine os pré-requisitos para que a interação aconteça.
>   - Determine a resposta emocional esperada do usuário quando a interação é finalizada.
> - O que o robô faz ao encontrar pessoas **paradas, em conversa ou em grupo**, e ao passar por elas num corredor (sem cruzar entre pessoas conversando)?
> - Proponha **um ajuste** desse comportamento espacial para um contexto de uso diferente do principal.

<details>
<summary>📄</summary>

- **Posicionamento:** aborda o grupo a uma distância social (2–3 m), sempre pela frente, nunca por trás.
- **Início da aproximação:** aproxima-se em diagonal (nunca em linha reta "contra" a pessoa), reduzindo a velocidade a 1,5 m de distância.
- **Sinalização de destino:** gira a "cabeça" na direção do laboratório antes de começar a andar.
- **Grupos e corredores:** ao encontrar duas pessoas conversando, contorna por trás delas, sem passar entre as duas; para grupos maiores, aguarda uma abertura natural na formação.
- **Ajuste de contexto:** em dias normais de aula (sem evento), o robô aumenta a distância de abordagem, já que há menos ruído social e mais espaço livre no saguão.

</details>

### Verbal

> 💡
> - A interação verbal do robô será **restrita** (comandos, FSM) ou **aberta** (LLM/chatbot)? Justifique a escolha.
> - Para cada interação verbal:
>   - Descreva a interação.
>   - Determine os pré-requisitos para que a interação aconteça.
>   - Determine a resposta emocional esperada do usuário quando a interação é finalizada.
> - Como o robô lida com o **timing** das respostas (silêncio, marcadores conversacionais como "uh-huh")?
> - Que tipo de voz (TTS) o robô usa, e por que ela **combina** com a aparência e o propósito dele?
> - Identifique **uma limitação** do reconhecimento de fala (ruído, sotaque, vocabulário) que afetaria o seu cenário de uso, e como mitigá-la.

<details>
<summary>📄</summary>

**Restrita** — usa uma árvore de diálogo (FSM) com um conjunto fechado de destinos e perguntas frequentes, pois o saguão é ruidoso e o vocabulário esperado é previsível; mais confiável do que abrir para um LLM.

**Timing:** ao processar um pedido, o robô emite um "hum" sonoro curto e pisca os olhos em sequência, evitando silêncio constrangedor.

**Voz:** TTS de tom jovem e neutro, volume ajustável ao ruído do saguão — combina com o porte pequeno do robô (uma voz grave soaria estranha).

**Limitação do ASR:** o ruído do evento atrapalha o reconhecimento de nomes de professores e disciplinas. **Mitigação:** escolhas críticas (curso, laboratório) são feitas por toque na tela; o reconhecimento de fala só é usado para perguntas simples de sim/não.

</details>

### Não-verbal

> 💡
> - Escolha **dois canais** não verbais (olhar, gesto, toque, postura, ritmo, imitação) e descreva como o robô os usaria.
> - Para cada interação não-verbal:
>   - Descreva a interação.
>   - Determine os pré-requisitos para que a interação aconteça.
>   - Determine a resposta emocional esperada do usuário quando a interação é finalizada.
> - Explique como o robô **perceberia** as pistas não verbais correspondentes da pessoa.
> - Descreva um caso em que a **falta de coordenação** entre fala e comportamento não verbal quebraria a interação.
> - Proponha **uma pista não verbal exclusiva** do robô (sem equivalente humano direto) que ajudaria na comunicação.

<details>
<summary>📄</summary>

**Canais escolhidos: olhar e postura.**
- **Olhar:** os "olhos" de LED giram na direção de quem está falando com o robô e na direção da rota a seguir.
- **Postura:** o corpo se inclina levemente para frente ao iniciar a aproximação (convite) e se afasta/gira de lado ao encerrar a interação (despedida).

**Percepção:** uma câmera de profundidade detecta se a pessoa está olhando para o robô (atenção) e se está parada olhando ao redor (sinal de estar perdida).

**Falta de coordenação:** se o robô disser "vamos ao laboratório de robótica" mas girar para o lado errado, o grupo hesita e para de segui-lo — a confiança se quebra.

**Pista exclusiva do robô:** um anel de luz na base pisca em verde quando o robô está confiante do caminho e em amarelo quando está recalculando a rota — sem equivalente humano direto, mas comunica incerteza de forma clara.

</details>

## Emoção

> 💡
> - Escolha um **modelo de emoção** (categorias básicas de Ekman, modelo OCC ou modelo dimensional — Russell ou PAD) e justifique a escolha para o seu caso de uso.
> - Descreva **como** o robô perceberia o estado emocional do usuário, e por quais canais (rosto, voz, postura, outro).
> - Defina **quando** o robô deve mimetizar a emoção da pessoa e **quando não deve** (lembre-se da exceção da raiva — retribuir raiva raramente ajuda a resolver o conflito).
> - Identifique um risco de **gerenciamento de expectativas**: se o robô parece emocionalmente responsivo, que outras capacidades sociais o usuário passa a esperar dele? O robô consegue cumprir essa expectativa?

<details>
<summary>📄</summary>

**Modelo:** categorias básicas de Ekman (feliz, surpreso, neutro) — simples o suficiente para expressar por luzes e tom de voz, sem exigir um rosto detalhado.

**Percepção:** o robô reconhece tom de voz alterado (frustração) pelo microfone e expressões faciais básicas pela câmera, para saber se o visitante está confuso ou satisfeito.

**Mimetismo:** mimetiza entusiasmo — se o visitante se anima ao ver o laboratório de robótica, o robô "sorri" com as luzes — mas **nunca** mimetiza a impaciência de um visitante apressado; nesse caso mantém tom calmo e oferece um caminho mais curto.

**Risco de expectativa:** se o robô demonstra "empolgação", visitantes podem esperar que ele converse sobre assuntos abertos (ex.: "e as notas de corte?"). O robô precisa deixar claro, de forma simpática, quando um assunto está fora do seu escopo.

</details>

---                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     
[^1]: Fonte: Adaptado de <https://hazeshift.com.br/mapa-de-empatia/>
