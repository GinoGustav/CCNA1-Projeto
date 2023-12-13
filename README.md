# CCNA-1 - PROJETO
![ccna](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/bd5dbfb8-2c12-4792-9564-e2af61d34b24)

#### License
[![NPM](https://img.shields.io/npm/l/react)](https://github.com/GinoGustav/CCNA1-Projeto/blob/main/LICENSE)

# Sobre o projeto
Utilizado como introdutorio as Redes o **CCNA** apresenta as arquiteturas, modelos, protocolos e elementos de rede que conectam usuários, dispositivos, aplicativos e dados através da Internet e através de redes de computadores modernas.

A criação desse projeto é para fins de estudos e demonstração do meu caminho e da minha aprendizagem dentro do curso CCNA-1 que a partir da 7ª Maratona do Programa CiberEducação Cisco do Brasil fui qualificado entre as **34 mil pessoas do Brasil**. E passando com mais de **98% de qualificação** no curso inteiro. 

Criarei um projeto simples e fictício de uma pequena rede com as configurações e utilizações realizadas e abordadas dentro do Curso. Gerando um relátorio de topologia de rede, cabeamento, segurança e teste de conexão.



## Sumário:
- Organização e criação da topologia da rede
- Estruturação do meio lógico e do meio físico
- Configuração do Switch/Roteador
- Enderaçamento MAC/Ipv4/Ipv6
- Teste/Visualização de Conectividade da Rede


## • Organização e criação da topologia da rede
Nesse primeiro caso peguei um projeto ficticio para demonstrar a conectvidade entre as redes! Na imagem mostra:
- *4 Dispositivos finais*
- *4 Switches*
- *2 Roteadores*

![image](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/c8672826-a1e4-4814-b67d-f19954050a01)

Nesse primeiro caso irei fazer a tabela de endereçamento no **excel** para ficar mais fácil a **visualização e organização**. 'A mesma poderia ser imprimida e utilizada para organização fisicamente.'

![image](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/a949c166-c0c6-42bd-b787-ce2262f4482d)


## • Estruturação do meio lógico e do meio físico
Como a imagema acima demonstra irei trazer só o meio lógico pois iremos conectar uma rede a outra rede mas segue o mesmo principio se fosse uma rede local.
Através de cabos, Par trançado blindado (STP), Par trançado não blindado (UTP) ou Cabo coaxial fiz as ligações entre as redes e conectando em suas respectivas interfaces assim, prontos para fazer as configurações no dispositivos. Em alguns casos poderia utilizar Cabeamento de Fibra Óptica. Lembrando que para se fazer as configurações utiliza-se um cabo de console conectado nos dispositivos ou conexões SSH ou Telnet.

![54043200469628939__pt-BR__Original (1)](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/6fa5b966-2244-41bc-a462-fd47790a9048)

## • Configuração do Switch/Roteador
Nesse tópico irei começar a fazer a configurações do Switch/Roteador para estabelecer conexões. Irei utilizar "-G" no hostname dos dispositivos para indetificar minha titularidade do projeto!

![image](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/f0511eed-b555-446c-a0c1-8af18ea6d46a)

• Nessa primeira imagem entrei no modo enable para acesso do modo **EXEC** e depois no modo de **Configuração Global** do Roteador e utilizando o código **"hostname R1-G"** declarei o nome do dispositivo identificado na tabela de endereçamento.

![image](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/cc21baf5-677e-4d00-9744-f26122a60348)

• Agora configurei as senhas para o modo exec com criptografia e para o modo line console 0 e utilizei o serviço de criptografia para não exibir a senha, e utilizando o conceito de segurança criei uma senha "difícil" (Nesse caso como é um projeto estou utilizando a praticidade a meu favor mas o correto seria uma senha mais longa). Utilizei tambem os comandos **"security passwords min-length 7"** para definir a senha de no máximo 7 dígitos, e **"login block-for 120 attempts 3 within 60"** , bloqueará as tentativas de login por 120 segundos se houver três tentativas de login com falha dentro de 60 segundos. 

![image](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/77f3040b-fd26-4425-a14f-c57b0f45edc0)

• Nesse caso eu configurei o SSH para acesso remoto seguro.

![image](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/41a10472-967e-42ca-b410-76b67f99b050)

• Finalizando nossa configuração básica e de segurança.

![image](https://github.com/GinoGustav/CCNA1-Projeto/assets/45954363/41a8e617-667e-4fb1-adf1-99f853eb005f)

• Configurando as interfaces de R1 consultando a tabela de enderaçamento!








# Autor

Gustavo Gino Pereira

Linkedin:
https://www.linkedin.com/in/gustavo-gino

Agradecimento a PUC MG por disponibilizar a realização da maratona, pelo professor que acompanhei as aulas no youtube Deividson Okopnik.
