
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

Descreva aqui como foi o desenvolvimento do trabalho, destacando cada uma das etapas necessárias para chegar até a solução final.

## Desenvolvimento do Aplicativo

### Interface

Descreva o desenvolvimento das telas do aplicativo.

### Código

Descreva o desenvolvimento do código do aplicativo.

## Desenvolvimento do Hardware

### Montagem

Descreva como foi o processo da montagem do projeto.

### Desenvolvimento do Código

Durante o desenvolvimento do caminhão de bombeiros, que representa um avanço significativo, foi feita uma tentativa de compilar e executar o código sem o microcontrolador fornecido. Projeto de uso de aeronaves para ESP32, suportando nosso suporte e bibliotecas, processos principais e recursos especiais para IoT. No entanto, o fornecedor forneceu um ESP8266 por engano.

Essa opção foi inicialmente ignorada, levando a falhas durante a fase de compilação. Bibliotecas específicas do ESP32, como aquelas que permitiam a conectividade Bluetooth e a manipulação de vários núcleos de processador, não eram compatíveis com o ESP8266. Além disso, configurações como mapeamento de memória e pinos de gerenciamento de memória tiveram que ser ajustadas porque os dois microcontroladores possuem arquiteturas e capacidades diferentes.

Falha na identificação e repetição de erros na compilação e pré-verificação de firmware, exigindo diagnósticos cuidadosos para entender novamente que hardware sofisticado não atende à especificação no projeto. Correspondência exata de código e soluções alternativas de barramento, bibliotecas alternativas e bibliotecas incompatíveis e limitação do uso de restrições de recursão no ESP8266.

## Comunicação entre App e Hardware

Durante o desenvolvimento do Carrinho Bombeiro, uma das complicações enfrentadas foi relacionada à conexão e à configuração do microcontrolador. O projeto foi inicialmente planejado para usar um ESP32, devido às suas funcionalidades avançadas, como conectividade simultânea Wi-Fi e Bluetooth, maior capacidade de processamento e suporte a múltiplos sensores e dispositivos. No entanto, o vendedor forneceu erroneamente um ESP8266, que possui limitações em comparação ao ESP32.

Essa substituição trouxe desafios técnicos, pois o ESP8266, embora funcional e popular, não possui conectividade Bluetooth e tem menor desempenho em termos de capacidade de processamento e quantidade de GPIOs disponíveis. Esses fatores impactaram diretamente a integração de componentes e a comunicação do carrinho com o sistema de monitoramento remoto, além de demandar alterações no código e na arquitetura inicial do projeto.

A equipe precisou reavaliar as funcionalidades planejadas, ajustando os objetivos para adequar o protótipo às limitações do ESP8266 enquanto buscava minimizar os impactos na execução do projeto. Essa experiência destacou a importância de verificar com precisão os componentes adquiridos e adaptá-los de forma criativa quando imprevistos surgem, contribuindo para o aprendizado técnico e o desenvolvimento de soluções alternativas.
