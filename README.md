# Monitoramento de Nível de Água com ESP8266 e Telegram

## Descrição
Este projeto utiliza um ESP8266 NodeMCU e um sensor ultrassônico HC-SR04 para monitorar o nível de água em um copo de 250ml. Quando o nível da água estiver abaixo de um limite definido, um alerta é enviado automaticamente via Telegram.

## Funcionalidades
- Monitoramento contínuo do nível de água.
- Envio de alertas para um grupo ou usuário no Telegram.
- Integração com ESP8266 para processamento dos dados.
- Possibilidade de adaptação para diferentes recipientes.

## Componentes Utilizados
### Hardware:
- ESP8266 NodeMCU
- Sensor Ultrassônico HC-SR04
- Copo de 250ml
- Jumpers para conexão

### Software:
- Arduino IDE
- Biblioteca ESP8266WiFi
- Biblioteca HTTPClient

## Como Funciona
1. O sensor ultrassônico HC-SR04 mede a distância entre a superfície da água e o sensor.
2. O ESP8266 processa a leitura e compara com um limite estabelecido.
3. Se o nível da água estiver abaixo do limite, o ESP8266 envia um alerta via Telegram.

## Configuração e Uso
### 1. Configurar o Arduino IDE
- Instale a biblioteca ESP8266WiFi.
- Instale a biblioteca HTTPClient.
- Configure a placa como "NodeMCU 1.0 (ESP-12E Module)".

### 2. Configurar o Telegram
- Crie um bot no Telegram usando o BotFather.
- Obtenha o token do bot e o chat ID do destinatário.
- Adicione essas informações ao código.

### 3. Fazer o Upload do Código para o ESP8266
- Conecte o ESP8266 ao computador via cabo USB.
- Carregue o código na placa.
- Abra o Monitor Serial para verificar o funcionamento.

## Exemplo de Uso
- Encha o copo com água.
- Aos poucos, reduza o nível de água.
- Quando a água atingir o limite mínimo, uma notificação será enviada para o Telegram.

## Possíveis Melhorias
- Adição de um display OLED para exibição local do nível da água.
- Integração com um banco de dados para histórico de medições.
- Implementação de um relé para acionamento automático de uma bomba d'água.

## Licença
Este projeto está sob a licença MIT. Sinta-se à vontade para usá-lo e modificá-lo conforme necessário.

