
# Materiais

Os materiais utilizados no projeto foram:
- 2 Pontes H
- 5 Motores 3-6V
- 4 Rodas
- 1 Chassi 4WD
- 1 Bateria 9V
- 4 Pilhas 1.5V
- 1 ESP 8266
- 2 Protoboards
- 1 Suporte para bateria
- 1 Borrifador
# Desenvolvimento

O desenvolvimento foi constituído por etapas das quais se destacam: 

## Desenvolvimento do Aplicativo



### Interface

Ao desenvolver a interface do APP, o Scrum Master Samuel chegou a conclusão que a tela do aplicativo deveria ser o mais minimalista possível e contendo tudo em uma interface somente, incluindo as setas de comando, o "slider" de velocidade, e o IP necessário para conectar a rede WIFI.

### Código

O código do APP coleta o IP digitado e o copia em um link HTTP, para se conectar com o ESP, e dependendo de qual botão é apertado a URL muda o "State" e assim ativando a condição respectiva no codigo da placa.

## Desenvolvimento do Hardware

### Montagem

A montagem do carrinho foi desenvolvida pensando em sua melhor performance e mobilidade. Um desses feitos foi o fato de termos alimentações separadas, tanto para o ESP, quanto a ponte H. O ESP 8266 por sua vez, é mais compacto e seu modo de comunicação por wi-fi retorna uma resposta mais rápida que o de bluetooth do ESP 32. A distribuição e cabeamento dos motores na ponte H foi feito de forma que as 2 rodas da direita fossem sincronizadas e o mesmo para as da esquerda.

### Desenvolvimento do Código

O desenvolvimento do código foi relativamente simples, em primeira instancia a equipe estava ocupada em fazer o carrinho andar via USB, criando seus comandos básicos, visando testar o funcionamento de cada motor e descobrindo se ele teria força para seguir todos os comandos. Segundamente era preciso conectar os comandos a condições de sinais via bluetooth, nesse momento foi percebido que a peça vendida não se tratava de um ESP32 e sim um ESP8266, assim excluindo a possibilidade da conexão via bluetooth e restando a opção de usar WIFI. Tendo isso em mente foi necessário procurar nos fóruns do app inventor como comunicar o app com o ESP via WIFI. Ao fim o ESP cria uma rede de WIFI chamada "firefighter car" para conectar o dispostivo com o APP a placa e assim receber informações que serão usadas nas condições "if" e executar os comandos atenriormente citados.

## Comunicação entre App e Hardware

Durante o desenvolvimento do Carrinho Bombeiro, uma das complicações enfrentadas foi relacionada à conexão e à configuração do microcontrolador. O projeto foi inicialmente planejado para usar um ESP32, devido às suas funcionalidades avançadas, como conectividade simultânea Wi-Fi e Bluetooth, maior capacidade de processamento e suporte a múltiplos sensores e dispositivos. No entanto, o vendedor forneceu erroneamente um ESP8266, que possui limitações em comparação ao ESP32.

Essa substituição trouxe desafios técnicos, pois o ESP8266, embora funcional e popular, não possui conectividade Bluetooth e tem menor desempenho em termos de capacidade de processamento e quantidade de GPIOs disponíveis. Esses fatores impactaram diretamente a integração de componentes e a comunicação do carrinho com o sistema de monitoramento remoto, além de demandar alterações no código e na arquitetura inicial do projeto.

A equipe precisou reavaliar as funcionalidades planejadas, ajustando os objetivos para adequar o protótipo às limitações do ESP8266 enquanto buscava minimizar os impactos na execução do projeto. Essa experiência destacou a importância de verificar com precisão os componentes adquiridos e adaptá-los de forma criativa quando imprevistos surgem, contribuindo para o aprendizado técnico e o desenvolvimento de soluções alternativas.
