# GS-Edge



Participantes : Vinicius Cont e Italo Caliari

Bom Dia professor ,Tudo bem ?

link do projeto: https://www.tinkercad.com/things/dvb8NmaAERE-gs-arduino?sharecode=Zl9-en66HfjDvJBYn21CxWB8MetvV4P3T27AeNoKp3o


Este é um projeto que ultiliza um sensor de distância ultrassônico que ultiliza o sensor HC-SR04 e um LED para Indeicar qaundo tem lixo (residuos,Plastico) em uma distacia de 10 cm de distancia quando liga o LED e indica que tem lixo por perto.

O codigo Fonte ultilizado é C++.

Para iniciarmos o codigo começamos com as definições de pinos com o 'trigPin', 'echoPin' , 'ledPin' ; então o 'trigPin' foi definido como Pino 9 , 'echoPin' foi definido como Pino 8 e o 'ledPin' foi definido como Pino 4.

Com isso configuramos o void setup onde ajustamos os pinos como de saída ou entrada. Tambem ultilizamos o 'Serial.begin' para iniciar sua comunicação.

Depois de definimos os Pinos criamos uma variável global chamada 'distance' para medir a distância em centrímetros e configurar o void setup.
Com isso foi configurado o void loop onde foi ultilizado uma função chamada 'measureDistance()' para medir a distância com o sensor, Logo apos disso ultilizei um 'if' e 'else' para dizer um limite. Então foi colocado no 'if' a 'distance' menor que 10cm ligando o LED e fazendo uma print no Serial "Lixo por perto" e no 'else' para desligar o Led.

Depois de fazer toda esta configuração temos que falar sobre a função 'measureDistance()' criada para enviar um pulso de 10 microsegundos para o sensor, tambem foi usado o 'pulseIn()' para medir o tempo do pulso ultrassônico e a formula para calcular a distancia em centimetros ultilizando 'distance = duracao * 0.0343 / 2'
