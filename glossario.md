# Glossário de [Fundamentos  SI]

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
## FRAGILIDADES
  SEGURANÇA: SYN Flooding (Inundação SYN) - IP Spoofing (Falsificação de IP) - Sequestro de Sessão (TCP Connection Hijacking) - Ataques RST e FIN - Ping da Morte - Falta de Criptografia Nativa
  ESTRUTURAIS E DE PROTOCOLO: Protocolo UDP - Ataques ICMP - Source Routing
## Como diminuir as fragilidades:
  Para mitigar as fragilidades do modelo TCP/IP, é necessário aplicar camadas de proteção que o protocolo original não possui. Como ele foi desenhado para ser eficiente e não necessariamente seguro, a estratégia padrão é "envelopar" o tráfego e validar rigorosamente as conexões.
# Criptografia para combater o Texto Claro
  - A falha de privacidade é corrigida substituindo protocolos inseguros por suas versões criptografadas
# Defesas contra SYN Flood (DoS)
  - Para evitar que um servidor fique travado esperando por conexões falsas, utilizam-se técnicas de gerenciamento de tráfego.
# Filtros contra IP Spoofing
  - Para impedir que atacantes mascarem sua identidade usando IPs falsos, as redes devem ser configuradas para não aceitar tráfego incoerente.
