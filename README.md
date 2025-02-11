### atividade_aula_sincrona_06-02 - Controle de Servomotor por PWM

## Descrição do Projeto
Este projeto tem como objetivo controlar um servomotor utilizando PWM com o Raspberry Pi Pico W, dentro da plataforma BitDogLab. A GPIO 22 foi configurada para gerar um sinal PWM de 50Hz para posicionar o servo em diferentes ângulos. Além disso, o LED RGB conectado à GPIO 12 foi utilizado para observar seu comportamento conforme a movimentação do servo.

## Requisitos do Projeto

1. Utilizar o ambiente de desenvolvimento VS Code.
2. Escrever os códigos na linguagem C, utilizando o Kit de Desenvolvimento de Software Pico SDK.
4. Criar um repositório no GitHub para versionamento e submissão da atividade.
5. Implementar testes básicos para garantir o funcionamento correto do código.
6. Adicionar um arquivo README.md com instruções de uso do programa.
7. Produzir um vídeo ensaio de até 3 minutos apresentando a solução e os resultados, incluindo o link no README.md.

## Implementação

1. Configurar a GPIO 22 com uma frequência de 50Hz (Período de 20ms).
2. Ajustar o ciclo de trabalho (Duty Cycle) para:
   - 180° (2.400µs) e aguardar 5 segundos.
   - 90° (1.470µs) e aguardar 5 segundos.
   - 0° (500µs) e aguardar 5 segundos.
3. Criar uma rotina de movimentação suave entre 0° e 180°, com incrementos de ±5µs a cada 10ms.
4. Observar o comportamento do LED RGB (GPIO 12) durante a movimentação do servo.

## Configuração e Execução


### Executar na BitDogLab
1. Conecte a BitDogLab ao PC e entre no modo BOOTSEL.
2. A placa aparecerá como uma unidade USB.
3. Arraste o arquivo `servo_pwm.uf2` para essa unidade.

## Observações sobre o LED RGB (GPIO 12)
- Quando o servo está em 0° (500µs): O LED acende (vermelho).
- Quando o servo está em 90° (1470µs): O LED apaga.
- Quando o servo está em 180° (2400µs): O LED acende novamente (azul).
- Durante o movimento suave: O LED pode piscar ligeiramente.

## Conclusão
Este projeto demonstrou como controlar um servomotor via PWM no Raspberry Pi Pico W e analisar o comportamento do LED RGB na plataforma BitDogLab. O servo foi posicionado corretamente nos ângulos de 0°, 90° e 180°, e a movimentação suave foi realizada com sucesso.

## Vídeo Ensaio
O vídeo ensaio com a apresentação da solução e os resultados obtidos pode ser acessado no seguinte link:
[Inserir Link do Vídeo Aqui]

## Autor
Jotta

