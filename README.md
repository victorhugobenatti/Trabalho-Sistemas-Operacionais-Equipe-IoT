# Os desafios/problemas para interoperabilidade aplicada à Cidades Inteligentes

Nome da Equipe: Grupo - 9 IoT 

Integrantes:

MAURICIO GOMES ROCHA - 202107030

NORTON ALMEIDA PONTES - 202203526

RAFAEL RIBEIRO M. PARREIRA - 202107035

ROGÉRIO RODRIGUES ROCHA - 202203530

VICTOR HUGO BENATTI FRANCO - 202203532

# *Introdução*
## *Descrição do Problema:*
A Internet das Coisas (IoT) está se tornando uma parte integrante de nossas vidas, conectando um extenso número de dispositivos ao redor do mundo. No entanto, à medida que a adoção da IoT aumenta, também surgem desafios significativos relacionados à comunicação entre esses dispositivos [1]. 

A interoperabilidade entre os dispositivos IoT é um problema persistente. Muitos desses dispositivos operam em silos, utilizando protocolos de comunicação diferentes, o que dificulta a criação de soluções abrangentes e eficazes. A falta de padronização compromete a capacidade de diferentes dispositivos se comunicarem de maneira eficiente, prejudicando a criação de ecossistemas verdadeiramente integrados [2]. 

Dessa forma, o artigo abordará os obstáculos significativos que as Cidades Inteligentes enfrentam em relação à interoperabilidade entre os dispositivos IoT.

## *Proposta de Solução*
Com base nos desafios apresentados no artigo [2], uma sugestão para abordar a atual problemática é a concepção de um padrão de intercomunicação destinado a integrar os variados sistemas dos dispositivos IoT em uma Cidade Inteligente. A presença de diversos padrões, conforme destacado no artigo [3], dificulta a interoperabilidade de dados. Portanto, para assegurar uma comunicação eficiente entre esses dispositivos, a adoção de um padrão universal emerge como uma medida eficaz contra o problema em questão. Para alcançar esse objetivo, propõe-se a exploração de frameworks que promovam a padronização e facilitem a interação com os diversos tipos de sistemas, possibilitando a troca de dados e informações. Essa abordagem viabilizará a criação de aplicações multiplataformas, acessíveis através das diversas arquiteturas de fabricantes.

# *Fundamentos teóricos*
Com o conhecimento dos protocolos de comunicação mais usados, há ainda o desafio de solucionar o problema da interoperabilidade, que é um problema incessante [2], como todos os protocolos são bastante utilizados todos em seus propósitos específicos, há casos que irá conflitar os protocolos de comunicação, e para isso há uma possibilidade de solução, usando um bem maior, como por exemplo o avanço tecnológico como propósito a ser alcançado usando de soluções compartilhadas e experiências passadas como aprendizado para criar-se um termo de normas comuns.

A busca por uma interoperabilidade eficaz entre sistemas representa um dos desafios mais prementes no campo da tecnologia. A diversidade de plataformas, protocolos e padrões adotados por diferentes fabricantes dificulta a comunicação fluida entre dispositivos e sistemas heterogêneos. A ausência de uma padronização universal frequentemente resulta em silos de informação, onde a troca de dados torna-se complexa e limitada. Além disso, questões relacionadas à segurança, privacidade e a rápida evolução tecnológica também contribuem para a complexidade desse cenário.

Abordar os desafios na interoperabilidade requer esforços colaborativos, envolvendo padronização de protocolos, desenvolvimento de interfaces comuns e a implementação de práticas de segurança robustas. A superação desses obstáculos é crucial para promover ecossistemas tecnológicos mais integrados, capacitando a inovação e proporcionando benefícios significativos em diversas áreas, desde a Internet das Coisas até ambientes corporativos e sistemas de saúde.

Com base na problemática abordada, é necessário entender os principais protocolos de comunicação na IoT e frameworks para padronização já conhecidos para se ter uma base para determinar um padrão universal. Além disso, é preciso entender os desafios na interoperabilidade de sistemas dentro deste contexto.

## *Protocolos de Comunicação na IoT*
Com base no contexto apresentado, para alcançar a interoperabilidade entre dispositivos IoT, é vital compreender os diferentes protocolos de comunicação utilizados. Temos como exemplos de protocolos de comunicação na IoT o *MQTT*, o *CoAP*, o *HTTP*, o *AMQP* e o *Wi-fi*.

O protocolo MQTT é caracterizado por ser leve e eficiente, tornando-se ideal para ambientes com largura de banda limitada. Adota o modelo de publicação/assinatura, permitindo comunicação assíncrona, e é projetado para redes instáveis, assegurando confiabilidade na entrega de mensagens. Dentre suas vantagens tem se um baixo consumo de largura de banda, suporte a notificações push. Além disso, é adequado para dispositivos com recursos limitados, embora haja uma falta de mecanismos integrados de segurança, podendo depender de camadas adicionais.

O CoAP é projetado para dispositivos com restrições de recursos, apresentando eficiência e suporte a multicast. Utiliza o modelo de requisição/resposta, semelhante ao HTTP, e destaca-se por seu consumo eficiente de recursos, menor sobrecarga em comparação com o HTTP, sendo adequado para ambientes IoT com dispositivos limitados. Entretanto, o CoAP é menos difundido que o HTTP, o que pode limitar a interoperabilidade em alguns casos.

Amplamente utilizado na web, o HTTP é conhecido por seu modelo de requisição/resposta e pelo uso de URLs para identificação de recursos. Sua fácil integração com a infraestrutura web existente, suporte generalizado em dispositivos e plataformas, e compatibilidade com firewalls e proxies são vantagens notáveis. Como suas maiores limitações, o HTTP tem um maior overhead em comparação com protocolos mais leves como MQTT e CoAP e uma menor eficiência em ambientes com restrições severas de recursos.

O AMQP é um protocolo de mensagens orientado a filas, oferecendo suporte a filas de mensagens, trocas e roteamento flexível. Projetado para cenários de mensageria complexos, destaca-se pela flexibilidade na implementação de padrões avançados e suporte a cenários de mensageria assíncrona e distribuída. Entretanto, ele pode ser mais complexo do que protocolos como MQTT para casos de uso simples. Além disso, há um maior consumo de recursos em comparação com protocolos mais leves.

A tecnologia Wi-Fi, padrão IEEE 802.11, é amplamente utilizada para conectividade de rede local sem fio, oferecendo largura de banda relativamente alta em comparação com tecnologias mais antigas. Este modelo possui uma alta taxa de transferência de dados, além de uma ampla disponibilidade e compatibilidade. Em contrapartida, há também um consumo mais elevado de energia em comparação com tecnologias de baixo consumo, junto a um alcance limitado em comparação com tecnologias de longo alcance como LoRa.

## *Frameworks para Padronização na IoT*
Seguindo a proposta de solução apresentada, para se alcançar a interoperabilidade entre dispositivos IoT é fundamental compreender os diferentes frameworks de desenvolvimento para IoT. Alguns dos principais são:

 - Arduino: Plataforma de código aberto para prototipagem eletrônica. Suporte a uma ampla variedade de placas e módulos. Comunidade ativa e vasta documentação.
 - Raspberry Pi: Placa de computador de baixo custo. Pode ser utilizado como um controlador central em projetos IoT. Suporte a diversas linguagens de programação.
 - IoTivity: Framework open-source mantido pela OCF (Open Connectivity Foundation). Focado em padronizar a comunicação entre dispositivos IoT. Suporta diferentes protocolos de comunicação.
 - Node-RED: Plataforma de código aberto para programação visual. Facilita a criação de fluxos de dados IoT de maneira intuitiva. Suporte a uma variedade de dispositivos e protocolos.
 - AWS IoT Core: Serviço gerenciado pela Amazon Web Services. Oferece recursos para conectar dispositivos à nuvem. Suporte a segurança e gerenciamento de dispositivos.
 - Microsoft Azure IoT: Plataforma de IoT integrada ao ecossistema Azure. Oferece serviços para conectar, monitorar e gerenciar dispositivos IoT. Integração com ferramentas de análise de dados e machine learning.
 - Google Cloud IoT: Oferece serviços para conectar e gerenciar dispositivos IoT na nuvem. Integração com outros serviços do Google Cloud. Suporte a segurança e monitoramento.
 - Eclipse IoT: Conjunto de projetos de código aberto para desenvolvimento IoT. Inclui ferramentas, frameworks e protocolos. Foco na interoperabilidade e padronização.


# *Referências:*
[1] D. L. Dantas, L. V. L. Filgueiras, and A. A. F. Brandão, "Portability and interoperability in IoT Platforms application layer portabilidade e interoperabilidade na camada de aplicação de plataformas de internet das coisas," in Anais, 2019.

[2] S. Andrade and D. Luque. "Interoperabilidade de Sistemas aplicados às Cidades Inteligentes: Um Estudo de Mapeamento Sistemático", in Anais do X Workshop de Computação Aplicada em Governo Eletrônico, Niterói, 2022, pp. 97-108, doi: https://doi.org/10.5753/wcge.2022.222970.

[3] D. V. A. Silveira et al., "Proposta de padronização de comunicação para dispositivos IoT," in Congresso Brasileiro de Automática-CBA, vol. 1, no. 1, 2019, doi: https://doi.org/10.20906/CBA2022/511.

