# Glossário de [Fundamentos  SI]


Sistema: conjunto de elementos que interagem entre si em prol de solucionar e fazer funcionar um esquema

Arquitetutra de computadores: Ela define como os componentes de hardware (processador, memória, entrada/saída) interagem e são organizados para executar instruções e processar dados.

Modelos de Arquitetura: (Contratação de serviços)

    Daas: Computador virtual completo pela internet: seu desktop roda na nuvem. Empresas alugam para que seus funcionários trabalgem remotamente. Um exemplo: Microsoft (Azure Virtual Desktop)
    DBaaS: Aluga um banco de dados pronto na nuvem. Sem instalar MySQL e sem configurar o servidor. Serve para aplicações que precisam armazenar dados sem gerenciar estrutura. Exemplo: Google Cloud Plataform
    Iaas: Infraestrutura como serviço: Aluga base da máquina: servidor, armazenamento, rede. É como alugar uma casa só com água e energia, completamente sem nada. Exemplo: Amazon Web Service
    Paas: No Iaas você monta o computador. No Paas, ele já vem montado e com sistema operacional. Serve para desenvolvedores que querem focar no código e não na infraestrutura. Exemplo: Netflix
    Saas: Modelo do Software como negócio, como serviço. Software totalmente pronto. Nada de instalar, configurar servidor ou programar. Exemplo: Microsoft 365 -SECaas: Ferramentas de segurança hospedadas na nuvem: Antivirus, firewall, monitoramento de ameaças Exemplo: Cisco

Tipos de Sistemas de Informações:

Sistemas de Processamento de Transações (SPTs): Sistemas responsaveis por registrar e processar operações rotineiras do dia a dia, como vendas, pagamentos e estoque.

Sistemas de Informação Gerencial (SIGs): Sistemas que acompanham a monitoração, o controle, a tomada de decisão e as atividades admnistrativas.

Sistemas de Apoio à Decisão (SADs): Sistemas que auxiliam os gerentes de nivel medio a tomar decisões que não são comuns.

Sistemas de Apoio ao Executivo (SAEs): Sistemas voltados para alta administração, com informações estratégicas e indicadores de desempenho.

CRUD:

C create

R retrieve

U update

D delete

TCP/IP: Conjuno de protocolos que definem como dispositivos conectados conversam entre si.

    ERP: solução de software de gestão integrada que centraliza dados de departamentos como financeiro, RH, vendas, estoque e produção. Ele automatiza fluxos de trabalho e conecta processos, eliminando o uso de planilhas separadas e garantindo uma visão única e em tempo real da empresa, o que facilita a tomada de decisão.

THROUGPUT: Transações que um sistema consegue responder

Web -> Cloud computing: Computação em nuvem

    Apps: Software instalado em equipamento
    IoT: Internet of Things (Internet das Coisas), é a nuvem onde todas as coisas do cotidiano estão conectadas, bem como um carro elétrico, uma tomada inteligente, Alexa, etc.
    Vantagens: Flexibilidade, agilidade, autonomia e integração de tecnologias
    Desvantagens: Segurança, dependência
    Imperícia: Irresponsabilidade para com coisas importantes, como atualização de sistemas críticos
    Virtualização de Maquinas: Criar máquinas virtuais de servidores, storages ou redes em um único hardware físico, otimizando recursos e reduzindo custos
    Sistemas Pervasivos: Dispositivos presentes do cotidiano, onipresentes. Geralmente são conectados e podem compartilhar informações em prol da experiencia do usuario. ELa impulsiona a IoT.
    Sistemas Ubíquos: Presença inperceptivel de dispositivos inteligentes no cotidiano, podendo ser estar presentes em móveis, roupas e em outros objetos do dia-a-dia. São bem interativos e adaptaveis, favorecendo uma boa experiência personalizada.

TCP/IP: Conjuno de protocolos que definem como dispositivos conectados conversam entre si.

    Protocolo: Regras de comunicação


## Aula 7 IoT e Modelo TCP/IP
O Modelo TCP/IP é um conjunto de protocolosque define como os dispositivos secomunicam entre si.
  -tipos de comunicação
    -Envio de informação(escrita), recebimento de informação(leitura) e requisição de serviço(com e sem retorno)
    ## 1. Camada de aplicação
      FUNÇÃO: Ela atua como a interface direta entre o usuário final e os aplicativos de rede, permitindo que programas (como navegadores ou clientes de e-mail) acessem os serviços de rede.
    ## 2. Camada de Transporte
      FUNÇÃO:  Esta camada gerencia o fluxo de dados entre dispositivo e garante a entrega correta dos pacotes(TCP e UDP)
    ## 3. Camada de Internet
      FUNÇÃO:  Esta camada é responsavel pelo roteamento e endereçamento de pacotes de dados(IP)
    ## 4. Camada de Rede
      FUNÇÃO: A camada de acesso à rede lida com o envio de pacotes atraves de diferentes tipos de redes fisicas
# FRAGILIDADES
  SEGURANÇA: SYN Flooding (Inundação SYN) - IP Spoofing (Falsificação de IP) - Sequestro de Sessão (TCP Connection Hijacking) - Ataques RST e FIN - Ping da Morte - Falta de Criptografia Nativa
  ESTRUTURAIS E DE PROTOCOLO: Protocolo UDP - Ataques ICMP - Source Routing
  
# Como diminuir as fragilidades:
  Para mitigar as fragilidades do modelo TCP/IP, é necessário aplicar camadas de proteção que o protocolo original não possui. Como ele foi desenhado para ser eficiente e não necessariamente seguro, a estratégia padrão é "envelopar" o tráfego e validar rigorosamente as conexões.
## Criptografia para combater o Texto Claro
  - A falha de privacidade é corrigida substituindo protocolos inseguros por suas versões criptografadas
## Defesas contra SYN Flood (DoS)
  - Para evitar que um servidor fique travado esperando por conexões falsas, utilizam-se técnicas de gerenciamento de tráfego.
## Filtros contra IP Spoofing
  - Para impedir que atacantes mascarem sua identidade usando IPs falsos, as redes devem ser configuradas para não aceitar tráfego incoerente.
