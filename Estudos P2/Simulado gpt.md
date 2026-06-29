# Simulado PV2 - Redes de Dados I

**Professor:** Edson J. C. Gimenez  
**Estilo reproduzido:** múltipla escolha, verdadeiro/falso, questões práticas, alternativas próximas e uso de `n.d.a.`/`N.R.A.`  
**Conteúdos:** IPv4/ICMPv4, IPv6/ICMPv6, Ethernet/VLANs, Wi-Fi e Segurança Cibernética

---

# Parte 1 - Protocolos IPv4 e ICMPv4

**Assinale a alternativa correta:**

1. O protocolo IPv4 é caracterizado por:
   a) ser orientado à conexão e confiável  
   b) realizar transmissão de datagramas do tipo melhor esforço, não orientada à conexão e não confiável  
   c) garantir a entrega dos pacotes por meio de confirmações  
   d) substituir a camada de transporte  
   e) n.d.a.

2. O campo Versão do cabeçalho IPv4 possui:
   a) 4 bits e valor igual a 4  
   b) 8 bits e valor igual a 4  
   c) 4 bits e valor igual a 6  
   d) 16 bits e valor igual a 4  
   e) n.d.a.

3. Um datagrama IPv4 apresenta HLEN igual a 6. O tamanho do cabeçalho, em bytes, é:
   a) 6  
   b) 20  
   c) 24  
   d) 32  
   e) N.R.A.

4. Um pacote IPv4 possui Comprimento Total igual a 1500 bytes e HLEN igual a 5. O tamanho do campo dados é:
   a) 1480 bytes  
   b) 1500 bytes  
   c) 1520 bytes  
   d) 1450 bytes  
   e) N.R.A.

5. Um datagrama IPv4 transporta 2048 bytes de dados e utiliza cabeçalho padrão. Os valores dos campos Comprimento Total e HLEN são, respectivamente:
   a) 2068 e 5  
   b) 2048 e 20  
   c) 2068 e 20  
   d) 2048 e 5  
   e) n.d.a.

6. O campo HLEN do IPv4 pode variar, em valores decimais, de:
   a) 1 a 5  
   b) 4 a 16  
   c) 5 a 15  
   d) 20 a 60  
   e) n.d.a.

7. O campo Tipo de Serviço do IPv4 é usado principalmente para:
   a) indicar o endereço IP de destino  
   b) controlar o número máximo de saltos  
   c) indicar tratamento, prioridade ou QoS do datagrama  
   d) verificar erro nos dados da camada de aplicação  
   e) n.d.a.

8. O campo TTL do IPv4:
   a) aumenta de 1 a cada roteador  
   b) indica o tamanho total do datagrama  
   c) é decrementado a cada roteador e, ao chegar a zero, o pacote é descartado  
   d) substitui o endereço IP de origem  
   e) n.d.a.

9. Considerando o campo Número do Protocolo do IPv4, a alternativa correta é:
   a) ICMP = 6, TCP = 1, UDP = 17  
   b) ICMP = 1, TCP = 6, UDP = 17  
   c) ICMP = 17, TCP = 6, UDP = 1  
   d) ICMP = 89, TCP = 17, UDP = 6  
   e) n.d.a.

10. A soma de verificação do cabeçalho IPv4 permite:
    a) detectar possíveis erros no cabeçalho do datagrama  
    b) detectar erros apenas no payload da aplicação  
    c) criptografar os dados do datagrama  
    d) aumentar o tamanho do campo dados  
    e) n.d.a.

11. O campo Opções do IPv4:
    a) é obrigatório em todo pacote IPv4  
    b) pode ser utilizado para funções de teste e depuração, como Record Route  
    c) possui sempre 20 bytes  
    d) identifica diretamente o protocolo da camada de transporte  
    e) n.d.a.

12. O campo Dados, ou payload, do IPv4 é utilizado para:
    a) armazenar apenas endereços MAC  
    b) transportar protocolos de camadas superiores  
    c) definir o tempo de vida do pacote  
    d) substituir o campo de checksum  
    e) n.d.a.

13. Deseja-se enviar um datagrama IP cuja carga útil é de 1780 bytes por um enlace cuja MTU é de 600 bytes. Sabendo-se que HLEN = 7, o número de fragmentos necessários será:
    a) 2  
    b) 3  
    c) 4  
    d) 5  
    e) N.R.A.

14. Na situação da questão anterior, o deslocamento de fragmento do segundo fragmento será:
    a) 0  
    b) 8  
    c) 71  
    d) 75  
    e) N.R.A.

15. Deseja-se enviar um datagrama com 2000 bytes de dados, cabeçalho padrão e MTU de 800 bytes. O número de fragmentos será:
    a) 2  
    b) 3  
    c) 4  
    d) 5  
    e) n.d.a.

16. Na situação da questão anterior, o tamanho do campo dados do último fragmento será:
    a) 224 bytes  
    b) 448 bytes  
    c) 776 bytes  
    d) 800 bytes  
    e) n.d.a.

17. Na situação das questões 15 e 16, o deslocamento de fragmento do último fragmento será:
    a) 97  
    b) 185  
    c) 194  
    d) 200  
    e) n.d.a.

18. Considerando um pacote IPv4 com HLEN = 7 e Comprimento Total = 1240 bytes, o tamanho do payload é:
    a) 1212 bytes  
    b) 1220 bytes  
    c) 1240 bytes  
    d) 1268 bytes  
    e) N.R.A.

19. Em um pacote IPv4, o campo Deslocamento de Fragmento possui valor 92. A quantidade de bytes de dados enviados em fragmentos anteriores é:
    a) 92 bytes  
    b) 184 bytes  
    c) 368 bytes  
    d) 736 bytes  
    e) N.R.A.

20. A mensagem ICMP Destination Unreachable com código “Fragmentation Needed and DF set” indica que:
    a) o TTL chegou a zero  
    b) o host respondeu ao ping  
    c) a fragmentação era necessária, mas estava proibida pelo bit DF  
    d) a porta destino respondeu corretamente  
    e) n.d.a.

21. As mensagens Echo Request e Echo Reply são utilizadas principalmente pelo comando:
    a) arp  
    b) ping  
    c) ipconfig  
    d) netstat  
    e) n.d.a.

22. A mensagem ICMP Time Exceeded é enviada quando:
    a) o endereço MAC não é encontrado  
    b) o campo TTL de um pacote é zerado  
    c) a porta TCP está aberta  
    d) o pacote possui cabeçalho padrão  
    e) n.d.a.

23. As mensagens ICMPv4 são:
    a) encapsuladas em datagramas IPv4  
    b) transmitidas fora do protocolo IP  
    c) usadas apenas em redes IPv6  
    d) equivalentes ao protocolo TCP  
    e) n.d.a.

24. Em uma mensagem Destination Unreachable, o código Port Unreachable indica que:
    a) a rede destino não existe  
    b) o host destino não existe  
    c) não há aplicação associada à porta destino  
    d) o roteador esgotou o TTL  
    e) n.d.a.

25. Assinale V ou F:
    1. ( ) O IPv4 pode transportar diferentes tipos de tráfego, como voz, vídeo e dados.  
    2. ( ) O campo Comprimento Total indica apenas o tamanho do cabeçalho.  
    3. ( ) A fragmentação ocorre sobre o campo dados do pacote IP.  
    4. ( ) O campo Deslocamento de Fragmento é contado em blocos de 8 bytes.

---

# Parte 2 - Protocolos IPv6 e ICMPv6

**Assinale V (verdadeiro) ou F (falso):**

1. ( ) A versão atual do IPv6 é definida pela RFC 8200.
2. ( ) O IPv6 utiliza 128 bits para endereçamento.
3. ( ) O cabeçalho básico IPv6 possui 12 campos fixos, como no IPv4.
4. ( ) O cabeçalho básico IPv6 possui tamanho fixo de 40 octetos.
5. ( ) O cabeçalho IPv4 pode variar entre 20 e 60 octetos.
6. ( ) O campo Próximo Cabeçalho identifica o cabeçalho que se segue ao cabeçalho IPv6.
7. ( ) O campo Tamanho do Conteúdo inclui o tamanho do cabeçalho básico IPv6.
8. ( ) O campo Limite de Saltos do IPv6 é equivalente ao TTL do IPv4.
9. ( ) O campo Rótulo de Fluxo possui 20 bits.
10. ( ) O campo Classe de Tráfego mantém a ideia de diferenciação de pacotes por serviço ou prioridade.
11. ( ) No IPv6, roteadores intermediários realizam fragmentação normalmente, como no IPv4.
12. ( ) No IPv6, a fragmentação e a remontagem ocorrem apenas na origem e no destino.
13. ( ) O IPv6 requer obrigatoriamente o uso de NAT para permitir comunicação fim-a-fim.
14. ( ) Cabeçalhos de extensão são utilizados para implementar funcionalidades adicionais no IPv6.
15. ( ) O cabeçalho básico IPv6 mantém o campo Checksum do cabeçalho.
16. ( ) O IPv6 possui endereço de broadcast de rede, assim como o IPv4.
17. ( ) Endereços unicast identificam uma única interface.
18. ( ) Endereços anycast identificam um grupo de interfaces, mas o pacote é entregue à interface mais próxima da origem.
19. ( ) Endereços multicast identificam um grupo de interfaces, e o pacote é entregue a todas as interfaces do grupo.
20. ( ) Uma mesma interface pode possuir mais de um endereço IPv6.

**Assinale a alternativa correta:**

21. Qual dos endereços abaixo está escrito em formato IPv6 inválido?
    a) 2001:db8::1  
    b) ::1  
    c) FE80:abcd::abcd::12fe  
    d) ::FFFF:192.168.0.1  
    e) n.d.a.

22. O prefixo utilizado para endereços IPv6 Global Unicast é:
    a) FE80::/10  
    b) FF00::/8  
    c) 2000::/3  
    d) ::1/128  
    e) n.d.a.

23. O endereço IPv6 Link Local é configurado automaticamente com o prefixo:
    a) 2001:db8::/32  
    b) FE80::/10  
    c) 2000::/3  
    d) ::FFFF/96  
    e) n.d.a.

24. O endereço IPv6 de loopback é:
    a) ::/128  
    b) ::1/128  
    c) FE80::1/10  
    d) 2001:db8::1  
    e) n.d.a.

25. Sobre o ICMPv6, assinale a alternativa correta:
    a) É usado apenas para mensagens de erro, com tipos de 128 a 255  
    b) Não participa da descoberta de vizinhança  
    c) Assume funcionalidades antes associadas ao ARP e ao IGMP no IPv4  
    d) É encapsulado diretamente em quadros Ethernet, sem IPv6  
    e) n.d.a.

---

# Parte 3 - Ethernet, VLANs e configuração básica

**Assinale a alternativa correta:**

1. O padrão IEEE 802.3 é conhecido popularmente como:
   a) Wi-Fi  
   b) Ethernet  
   c) Bluetooth  
   d) IPv6  
   e) n.d.a.

2. O padrão IEEE 802.3 implementa funcionalidades de quais camadas do modelo OSI?
   a) Rede e Transporte  
   b) Aplicação e Apresentação  
   c) Física e Enlace  
   d) Sessão e Transporte  
   e) n.d.a.

3. A camada de enlace no Ethernet é dividida nas subcamadas:
   a) IP e TCP  
   b) LLC e MAC  
   c) ARP e ICMP  
   d) TCP e UDP  
   e) n.d.a.

4. A subcamada MAC no IEEE 802.3 está associada ao controle de acesso ao meio e ao padrão:
   a) CSMA/CA  
   b) CSMA/CD  
   c) DNS  
   d) DHCP  
   e) n.d.a.

5. No CSMA/CD, quando um nó detecta colisão, ele deve:
   a) continuar transmitindo até o final do quadro  
   b) interromper a transmissão, enviar sinal de reforço de colisão e reiniciar o algoritmo de backoff  
   c) alterar o endereço MAC de origem  
   d) converter o quadro para IPv6  
   e) n.d.a.

6. Em conexões ponto a ponto full-duplex de Gigabit Ethernet, o CSMA/CD:
   a) continua sendo obrigatório em todos os casos  
   b) deixou de ser requisito obrigatório  
   c) foi substituído por ICMP  
   d) passou a operar na camada de rede  
   e) n.d.a.

7. O preâmbulo do quadro Ethernet é utilizado para:
   a) transportar o endereço IP de destino  
   b) sincronização  
   c) indicar o número da VLAN  
   d) transportar o checksum do IPv4  
   e) n.d.a.

8. O delimitador de início de quadro Ethernet possui a sequência de bits:
   a) 10101010  
   b) 11111111  
   c) 10101011  
   d) 00000000  
   e) n.d.a.

9. O campo FCS do quadro Ethernet:
   a) contém 4 bytes e utiliza CRC-32 para controle de erros  
   b) contém 20 bytes e substitui o cabeçalho IP  
   c) contém o endereço IPv4 de origem  
   d) identifica a VLAN nativa  
   e) n.d.a.

10. No quadro Ethernet, o campo Dados e enchimento possui, normalmente:
    a) mínimo de 20 bytes e máximo de 60 bytes  
    b) mínimo de 46 bytes e máximo de 1500 bytes  
    c) mínimo de 8 bytes e máximo de 512 bytes  
    d) sempre 40 octetos  
    e) n.d.a.

11. Um endereço MAC possui:
    a) 32 bits  
    b) 48 bits  
    c) 64 bits  
    d) 128 bits  
    e) n.d.a.

12. O campo Comprimento/Tipo do quadro Ethernet pode indicar:
    a) o protocolo de camada superior ou o número de bytes de dados  
    b) apenas o TTL do pacote  
    c) apenas o endereço MAC de origem  
    d) a senha da VLAN  
    e) n.d.a.

13. Uma VLAN pode ser entendida como:
    a) uma rede lógica usada para separar grupos de dispositivos  
    b) um endereço IPv6 especial  
    c) um protocolo da camada de transporte  
    d) um tipo de checksum  
    e) n.d.a.

14. A VLAN criada automaticamente e conhecida como VLAN padrão é:
    a) VLAN 0  
    b) VLAN 1  
    c) VLAN 10  
    d) VLAN 4095  
    e) n.d.a.

15. As VLANs de intervalo normal são identificadas por IDs:
    a) 0 a 255  
    b) 1 a 1005  
    c) 1006 a 4094  
    d) 1024 a 65535  
    e) n.d.a.

16. Um tronco de VLAN é:
    a) uma porta que pertence obrigatoriamente a uma única VLAN de acesso  
    b) um enlace ponto a ponto que pode transportar quadros de diferentes VLANs  
    c) um endereço MAC multicast  
    d) um protocolo de camada de aplicação  
    e) n.d.a.

17. O padrão usado para identificar VLANs em troncos Ethernet é:
    a) IEEE 802.1Q  
    b) IEEE 802.11  
    c) ICMPv6  
    d) ARP  
    e) n.d.a.

18. No cabeçalho de marcação de VLAN, o campo VID possui:
    a) 3 bits  
    b) 8 bits  
    c) 12 bits  
    d) 32 bits  
    e) n.d.a.

19. O campo TPID da tag 802.1Q possui valor:
    a) 0x0800  
    b) 0x8100  
    c) 0x86DD  
    d) 0x0001  
    e) n.d.a.

20. O comando usado para criar a VLAN 10 no switch Cisco é:
    a) vlan 10  
    b) ip vlan 10  
    c) switchport vlan 10  
    d) create network 10  
    e) n.d.a.

21. Para colocar uma porta de switch em modo de acesso, utiliza-se:
    a) switchport mode access  
    b) switchport mode trunk  
    c) encapsulation dot1Q 10  
    d) show vlan brief  
    e) n.d.a.

22. Para associar a porta Fa0/1 à VLAN 10, no modo de interface, utiliza-se:
    a) vlan 10 name Fa0/1  
    b) switchport access vlan 10  
    c) interface vlan 10  
    d) ip address vlan 10  
    e) n.d.a.

23. Para verificar as VLANs criadas e as portas associadas a cada VLAN, utiliza-se:
    a) show interface trunk  
    b) show ip route  
    c) show vlan brief  
    d) ping vlan 10  
    e) n.d.a.

24. Em uma topologia com duas VLANs, sem roteamento entre VLANs, é correto afirmar que:
    a) hosts de VLANs diferentes se comunicam normalmente  
    b) hosts da mesma VLAN podem se comunicar, mas hosts de VLANs diferentes não se comunicam  
    c) todas as VLANs pertencem à mesma rede lógica  
    d) a VLAN 1 é removida automaticamente  
    e) n.d.a.

25. No roteamento entre VLANs com subinterfaces, o comando `encapsulation dot1Q 10` tem a função de:
    a) desligar a interface física  
    b) associar a subinterface à VLAN 10 usando 802.1Q  
    c) criar um endereço MAC de broadcast  
    d) definir o endereço IP do host final  
    e) n.d.a.

---

# Parte 4 - WLAN, Wi-Fi e configuração básica

**Assinale a alternativa correta:**

1. O padrão IEEE 802.11 é conhecido popularmente como:
   a) Ethernet cabeada  
   b) Wi-Fi  
   c) IPv4  
   d) VLAN  
   e) n.d.a.

2. O padrão IEEE 802.11 define funcionalidades das camadas:
   a) Física e Enlace  
   b) Rede e Transporte  
   c) Aplicação e Sessão  
   d) Transporte e Aplicação  
   e) n.d.a.

3. No Wi-Fi, a subcamada MAC utiliza como mecanismo de acesso ao meio:
   a) CSMA/CD  
   b) CSMA/CA  
   c) TCP  
   d) ICMP  
   e) n.d.a.

4. As duas topologias apresentadas para redes Wi-Fi são:
   a) Cliente-servidor e ponto a ponto  
   b) Ad-hoc e Infraestrutura  
   c) VLAN e Trunk  
   d) TCP e UDP  
   e) n.d.a.

5. O ponto de acesso sem fio, AP, tem como uma de suas funções:
   a) converter quadros 802.11 em quadros 802.3, e vice-versa  
   b) substituir o endereço IP do roteador  
   c) eliminar a necessidade de autenticação  
   d) atuar apenas na camada de aplicação  
   e) n.d.a.

6. No processo de associação entre cliente e AP, os quadros Beacon são usados para:
   a) anunciar a presença da WLAN  
   b) calcular o checksum do IPv4  
   c) criar VLANs no switch  
   d) fragmentar pacotes IPv6  
   e) n.d.a.

7. Os quadros de investigação, ou Probe, são usados pelos clientes WLAN para:
   a) localizar redes sem fio disponíveis  
   b) configurar subinterfaces dot1Q  
   c) calcular endereço MAC  
   d) desabilitar o DHCP  
   e) n.d.a.

8. O SSID corresponde:
   a) ao endereço MAC do roteador  
   b) ao nome da rede sem fio  
   c) ao número do protocolo IPv4  
   d) ao campo FCS do quadro Ethernet  
   e) n.d.a.

9. No laboratório de configuração básica de Wi-Fi, a rede é implantada utilizando:
   a) roteador WRT300N e dispositivos sem fio  
   b) apenas switches Catalyst 2960  
   c) roteadores com subinterfaces 802.1Q  
   d) somente cabos coaxiais  
   e) n.d.a.

10. Ao montar inicialmente a rede Wi-Fi do laboratório, antes das configurações de segurança, a rede está:
    a) fechada e inacessível  
    b) aberta, permitindo conexão automática dos dispositivos sem fio  
    c) protegida por WPA2 automaticamente  
    d) configurada sem DHCP  
    e) n.d.a.

11. Em um dispositivo físico, o acesso inicial ao roteador sem fio normalmente envolve:
    a) navegador no endereço 192.168.0.1 e login admin/admin  
    b) comando show vlan brief  
    c) encapsulation dot1Q 10  
    d) endereço IPv6 FE80::/10  
    e) n.d.a.

12. No laboratório, o SSID configurado para a rede sem fio é:
    a) inatelsemfio  
    b) labsemfio  
    c) redesdados  
    d) admin  
    e) n.d.a.

13. No laboratório, o modo de segurança selecionado no roteador é:
    a) Open  
    b) WEP  
    c) WPA2 Personal  
    d) WPA Enterprise  
    e) n.d.a.

14. No laboratório, o tipo de criptografia configurado é:
    a) AES  
    b) TKIP  
    c) DES  
    d) CRC-32  
    e) n.d.a.

15. A senha de acesso à rede Wi-Fi configurada no laboratório é:
    a) admin  
    b) labsemfio  
    c) inatel2020  
    d) 192.168.0.1  
    e) n.d.a.

16. A senha administrativa do roteador, no laboratório, deve ser alterada para:
    a) admin  
    b) inatelsemfio  
    c) inatel2020  
    d) senha123  
    e) n.d.a.

17. No laboratório, recomenda-se que o gerenciamento remoto do roteador fique:
    a) habilitado  
    b) desabilitado  
    c) configurado como VLAN 10  
    d) configurado como ICMP  
    e) n.d.a.

18. O serviço DHCP do roteador sem fio fornece:
    a) endereços IP automaticamente aos dispositivos  
    b) endereços MAC aos switches  
    c) números de VLAN aos quadros 802.1Q  
    d) pacotes ICMPv6  
    e) n.d.a.

19. No laboratório, após alterar as configurações da rede sem fio, os dispositivos precisam ser reconfigurados porque:
    a) a rede passou a exigir SSID correto, autenticação e chave de acesso  
    b) o protocolo IPv4 foi removido  
    c) o roteador deixou de operar como equipamento sem fio  
    d) o padrão Ethernet foi desativado  
    e) n.d.a.

20. Nos dispositivos sem fio, a autenticação configurada para acessar novamente a rede é:
    a) WPA2-PSK  
    b) SSH  
    c) Telnet  
    d) ICMP  
    e) n.d.a.

21. Após configurar SSID, autenticação, chave e criptografia no cliente sem fio, deve-se:
    a) desabilitar e habilitar a placa sem fio para solicitar configuração IP via DHCP  
    b) criar uma VLAN 20  
    c) configurar encapsulation dot1Q  
    d) alterar o TTL para zero  
    e) n.d.a.

22. O teste final de conectividade no laboratório Wi-Fi é realizado usando:
    a) ping  
    b) show vlan brief  
    c) traceroute apenas  
    d) netstat apenas  
    e) n.d.a.

23. Uma recomendação de segurança para redes Wi-Fi domésticas é:
    a) manter SSID e senha administrativa padrão  
    b) desativar qualquer criptografia  
    c) alterar o SSID predefinido, trocar a senha administrativa e usar WPA2  
    d) usar apenas rede aberta  
    e) n.d.a.

24. Em hotspots Wi-Fi públicos, recomenda-se:
    a) enviar informações confidenciais livremente  
    b) evitar dados sensíveis e, se possível, usar túnel VPN criptografado  
    c) desabilitar toda autenticação  
    d) compartilhar senhas administrativas  
    e) n.d.a.

25. Em relação à evolução do Wi-Fi, a partir do Wi-Fi 6E e padrões superiores, o espectro passa a considerar:
    a) apenas 2,4 GHz  
    b) apenas 5 GHz  
    c) 2,4 GHz, 5 GHz e 6 GHz  
    d) apenas infravermelho  
    e) n.d.a.

---

# Parte 5 - Conceitos de Segurança Cibernética

**Assinale a alternativa correta:**

1. Segurança cibernética pode ser definida como:
   a) o esforço contínuo para proteger sistemas em rede e dados contra usos não autorizados ou prejudiciais  
   b) o processo de aumentar a velocidade da rede local  
   c) a criação de endereços IPv6  
   d) a configuração de VLANs em switches  
   e) n.d.a.

2. No nível corporativo, a segurança cibernética protege principalmente:
   a) apenas computadores pessoais  
   b) reputação, dados e clientes da empresa  
   c) somente endereços MAC  
   d) apenas redes sem fio abertas  
   e) n.d.a.

3. A identidade off-line inclui:
   a) apenas o nome de usuário usado em redes sociais  
   b) informações pessoais como nome, idade, CPF e endereço  
   c) apenas o endereço IP público  
   d) somente a senha do roteador  
   e) n.d.a.

4. Sobre a identidade on-line, é correto afirmar que:
   a) deve revelar o máximo possível de informações pessoais  
   b) corresponde à forma como o usuário se apresenta no ciberespaço  
   c) não possui relação com segurança  
   d) é sempre anônima  
   e) n.d.a.

5. Dados corporativos incluem:
   a) apenas endereços IP privados  
   b) informações de funcionários, propriedade intelectual e informações financeiras  
   c) apenas quadros Ethernet  
   d) somente senhas de Wi-Fi  
   e) n.d.a.

6. A tríade CID corresponde a:
   a) Criptografia, Internet e Dados  
   b) Confidencialidade, Integridade e Disponibilidade  
   c) Controle, Identificação e Domínio  
   d) Camada, Interface e Dispositivo  
   e) n.d.a.

7. A confidencialidade garante:
   a) privacidade dos dados, restringindo acesso inadequado  
   b) aumento da largura de banda  
   c) roteamento entre VLANs  
   d) fragmentação de pacotes  
   e) n.d.a.

8. A integridade está relacionada a:
   a) precisão, consistência e confiabilidade dos dados  
   b) quantidade de endereços IPv6  
   c) velocidade de uma rede Ethernet  
   d) escolha do canal Wi-Fi  
   e) n.d.a.

9. A disponibilidade garante que:
   a) os dados estejam sempre públicos  
   b) informações, dispositivos e rede possam ser acessados quando necessário por usuários autorizados  
   c) todo acesso seja anônimo  
   d) o firewall fique desligado  
   e) n.d.a.

10. Uma violação de segurança ocorre quando:
    a) há qualquer incidente com acesso não autorizado a dados, aplicações, redes ou dispositivos  
    b) um usuário troca o nome do SSID  
    c) um pacote IP é fragmentado  
    d) um switch cria uma VLAN  
    e) n.d.a.

11. Ameaças internas podem ocorrer quando usuários internos:
    a) tratam dados confidenciais de forma incorreta ou instalam malwares acidentalmente  
    b) apenas usam endereços IPv6  
    c) apenas consultam o DNS  
    d) apenas usam cabos Ethernet  
    e) n.d.a.

12. Ameaças internas podem causar grande dano porque usuários internos:
    a) não conhecem a rede  
    b) possuem acesso direto e conhecimento sobre recursos e dados confidenciais  
    c) só acessam páginas públicas  
    d) nunca possuem permissões  
    e) n.d.a.

13. Ameaças externas podem explorar:
    a) vulnerabilidades em redes e dispositivos ou engenharia social  
    b) apenas o campo HLEN do IPv4  
    c) somente o endereço de broadcast Ethernet  
    d) apenas o campo FCS  
    e) n.d.a.

14. Engenharia social é um ataque que busca:
    a) manipular indivíduos para realizar ações ou divulgar informações confidenciais  
    b) calcular deslocamento de fragmento  
    c) configurar trunk 802.1Q  
    d) aumentar o tamanho do pacote  
    e) n.d.a.

15. Phishing ocorre normalmente por:
    a) e-mail fraudulento disfarçado de fonte legítima e confiável  
    b) cálculo incorreto de máscara de rede  
    c) criação de VLAN padrão  
    d) uso do protocolo ARP de forma correta  
    e) n.d.a.

16. A quebra de senha de acesso à rede Wi-Fi consiste em:
    a) descobrir a senha usada para acesso à rede sem fio  
    b) desligar o DHCP  
    c) converter IPv4 para IPv6  
    d) apagar o campo FCS  
    e) n.d.a.

17. Uma boa prática de proteção é:
    a) manter firewall habilitado e atualizado  
    b) desativar todos os antivírus  
    c) instalar softwares de qualquer site  
    d) manter navegador sempre desatualizado  
    e) n.d.a.

18. Antivírus e antispyware têm como objetivo:
    a) impedir ou reduzir acesso não autorizado por softwares mal-intencionados  
    b) criar endereços MAC  
    c) configurar VLAN 10  
    d) remover o campo TTL  
    e) n.d.a.

19. Sobre atualizações de segurança, é correto afirmar que:
    a) sistemas e navegadores devem ser mantidos atualizados com patches recentes  
    b) atualizações devem ser evitadas  
    c) patches servem apenas para redes IPv6  
    d) navegadores não possuem configurações de segurança  
    e) n.d.a.

20. Para proteger dispositivos, recomenda-se:
    a) usar senha e criptografar dados confidenciais quando necessário  
    b) manter todos os dispositivos sem senha  
    c) usar apenas rede aberta  
    d) compartilhar credenciais administrativas  
    e) n.d.a.

21. Em uma rede Wi-Fi doméstica, recomenda-se:
    a) manter SSID e senha administrativa padrão  
    b) alterar SSID predefinido, trocar senha administrativa e usar WPA2  
    c) usar apenas WEP sem senha  
    d) deixar o roteador aberto  
    e) n.d.a.

22. Em hotspots Wi-Fi públicos, recomenda-se:
    a) evitar informações pessoais e confidenciais e, se possível, usar VPN  
    b) acessar bancos sem proteção  
    c) compartilhar credenciais  
    d) desativar toda criptografia  
    e) n.d.a.

23. O IDS tem como função principal:
    a) bloquear todo tráfego automaticamente  
    b) detectar, registrar e relatar tentativas de ataque  
    c) criar túneis criptografados  
    d) atribuir endereços IP por DHCP  
    e) n.d.a.

24. O IPS tem como função principal:
    a) impedir ataques, bloqueando determinado tráfego com base em regras  
    b) apenas registrar eventos sem bloquear  
    c) substituir o roteador Wi-Fi  
    d) converter quadros 802.11 em 802.3  
    e) n.d.a.

25. Uma VPN é projetada para:
    a) criar tunelamento criptografado seguro sobre a internet pública  
    b) criar VLANs de intervalo normal  
    c) calcular CRC-32 do quadro Ethernet  
    d) definir o campo HLEN  
    e) n.d.a.

---

# Gabarito comentado

## Parte 1 - IPv4 e ICMPv4

1. **B** - O IPv4 opera por melhor esforço, sem conexão e sem garantia de entrega.  
2. **A** - O campo Versão tem 4 bits e, no IPv4, vale 4.  
3. **C** - HLEN é contado em palavras de 32 bits: 6 × 4 = 24 bytes.  
4. **A** - HLEN 5 indica cabeçalho de 20 bytes; 1500 - 20 = 1480 bytes de dados.  
5. **A** - Cabeçalho padrão = 20 bytes e HLEN = 5; total = 2048 + 20 = 2068.  
6. **C** - O HLEN varia de 5 a 15, representando 20 a 60 bytes.  
7. **C** - O campo Tipo de Serviço está relacionado a prioridade e QoS.  
8. **C** - O TTL é decrementado a cada roteador; ao chegar em zero, o pacote é descartado.  
9. **B** - ICMP = 1, TCP = 6 e UDP = 17.  
10. **A** - O checksum do IPv4 verifica erros no cabeçalho.  
11. **B** - O campo Opções é opcional e pode ser usado para testes e depuração.  
12. **B** - O payload transporta protocolos de camadas superiores.  
13. **C** - HLEN 7 = 28 bytes; MTU 600 permite 572 bytes, mas usa-se 568 bytes por fragmento até o penúltimo; 1780 exige 4 fragmentos.  
14. **C** - O segundo fragmento começa após 568 bytes; 568/8 = 71.  
15. **B** - MTU 800 e cabeçalho 20 dão 780 bytes, mas o maior múltiplo de 8 é 776; 2000 exige 3 fragmentos.  
16. **B** - 2000 - 776 - 776 = 448 bytes no último fragmento.  
17. **C** - Antes do último fragmento foram enviados 1552 bytes; 1552/8 = 194.  
18. **A** - HLEN 7 = 28 bytes; 1240 - 28 = 1212 bytes de payload.  
19. **D** - O deslocamento é em blocos de 8 bytes; 92 × 8 = 736 bytes.  
20. **C** - Indica que era necessário fragmentar, mas o bit DF impedia a fragmentação.  
21. **B** - Echo Request e Echo Reply são usadas pelo ping.  
22. **B** - Time Exceeded ocorre quando o TTL expira.  
23. **A** - O ICMPv4 é encapsulado em datagramas IPv4.  
24. **C** - Port Unreachable indica ausência de aplicação associada à porta destino.  
25. **V, F, V, V** - O IPv4 transporta tráfegos variados; Comprimento Total inclui cabeçalho + dados; fragmentação ocorre no campo dados; deslocamento usa blocos de 8 bytes.

## Parte 2 - IPv6 e ICMPv6

1. **V** - A especificação atual é a RFC 8200.  
2. **V** - IPv6 possui endereços de 128 bits.  
3. **F** - O IPv6 possui 8 campos fixos, não 12.  
4. **V** - O cabeçalho básico tem tamanho fixo de 40 octetos.  
5. **V** - O cabeçalho IPv4 varia entre 20 e 60 octetos.  
6. **V** - Próximo Cabeçalho identifica o cabeçalho seguinte.  
7. **F** - Tamanho do Conteúdo indica apenas os dados após o cabeçalho IPv6.  
8. **V** - Limite de Saltos tem função equivalente ao TTL.  
9. **V** - O Rótulo de Fluxo possui 20 bits.  
10. **V** - Classe de Tráfego diferencia pacotes por prioridade/serviço.  
11. **F** - Roteadores intermediários não fragmentam no IPv6.  
12. **V** - Fragmentação e remontagem ficam na origem e no destino.  
13. **F** - O IPv6 não requer NAT para comunicação fim-a-fim.  
14. **V** - Cabeçalhos de extensão adicionam funcionalidades.  
15. **F** - O IPv6 removeu o checksum do cabeçalho básico.  
16. **F** - IPv6 não utiliza broadcast como o IPv4.  
17. **V** - Unicast identifica uma única interface.  
18. **V** - Anycast entrega à interface mais próxima do grupo.  
19. **V** - Multicast entrega a todos os membros do grupo.  
20. **V** - Uma interface pode ter múltiplos endereços IPv6.  
21. **C** - O símbolo `::` só pode aparecer uma vez no endereço.  
22. **C** - Global Unicast usa 2000::/3.  
23. **B** - Link Local usa FE80::/10.  
24. **B** - Loopback é ::1/128.  
25. **C** - O ICMPv6 assume funções como descoberta de vizinhança e gerenciamento multicast.

## Parte 3 - Ethernet, VLANs e configuração básica

1. **B** - IEEE 802.3 é Ethernet.  
2. **C** - Ethernet atua nas camadas física e de enlace.  
3. **B** - A camada de enlace é dividida em LLC e MAC.  
4. **B** - Ethernet cabeada utiliza CSMA/CD no controle de acesso ao meio.  
5. **B** - Em colisão, interrompe, envia sinal de reforço e faz backoff.  
6. **B** - Em Gigabit full-duplex ponto a ponto, CSMA/CD deixou de ser obrigatório.  
7. **B** - O preâmbulo serve para sincronização.  
8. **C** - O delimitador de início de quadro usa 10101011.  
9. **A** - FCS tem 4 bytes e usa CRC-32.  
10. **B** - Dados/padding variam de 46 a 1500 bytes.  
11. **B** - Endereço MAC possui 48 bits.  
12. **A** - O campo pode indicar comprimento ou tipo/protocolo superior.  
13. **A** - VLAN separa logicamente grupos de dispositivos.  
14. **B** - A VLAN padrão é a VLAN 1.  
15. **B** - Intervalo normal: 1 a 1005.  
16. **B** - Tronco transporta quadros de várias VLANs.  
17. **A** - O padrão de marcação em troncos é IEEE 802.1Q.  
18. **C** - VID possui 12 bits.  
19. **B** - TPID Ethernet para 802.1Q é 0x8100.  
20. **A** - `vlan 10` cria a VLAN 10.  
21. **A** - `switchport mode access` define porta de acesso.  
22. **B** - `switchport access vlan 10` associa a porta à VLAN 10.  
23. **C** - `show vlan brief` mostra VLANs e portas associadas.  
24. **B** - Sem roteamento, VLANs diferentes não se comunicam; mesma VLAN comunica.  
25. **B** - O comando associa a subinterface à VLAN 10 com encapsulamento 802.1Q.

## Parte 4 - WLAN, Wi-Fi e configuração básica

1. **B** - IEEE 802.11 é Wi-Fi.  
2. **A** - Atua nas camadas física e enlace.  
3. **B** - Wi-Fi usa CSMA/CA, pois busca evitar colisões.  
4. **B** - As topologias são Ad-hoc e Infraestrutura.  
5. **A** - O AP converte quadros 802.11 para 802.3 e vice-versa.  
6. **A** - Beacons anunciam a presença da WLAN.  
7. **A** - Probes ajudam o cliente a localizar redes disponíveis.  
8. **B** - SSID é o nome da rede sem fio.  
9. **A** - O laboratório usa WRT300N e dispositivos sem fio.  
10. **B** - Inicialmente a rede está aberta e os dispositivos conectam automaticamente.  
11. **A** - Acesso comum: navegador em 192.168.0.1 com admin/admin.  
12. **B** - O SSID configurado é labsemfio.  
13. **C** - O modo de segurança usado é WPA2 Personal.  
14. **B** - O laboratório usa TKIP.  
15. **C** - A passphrase é inatel2020.  
16. **B** - A senha administrativa passa a ser inatelsemfio.  
17. **B** - O gerenciamento remoto deve ficar desabilitado.  
18. **A** - DHCP fornece IP automaticamente.  
19. **A** - Os clientes precisam coincidir com SSID, autenticação, chave e criptografia.  
20. **A** - A autenticação configurada no cliente é WPA2-PSK.  
21. **A** - Desabilitar/habilitar a placa força nova solicitação DHCP.  
22. **A** - O teste de conectividade é feito com ping.  
23. **C** - Trocar SSID/senha padrão e usar WPA2 aumenta segurança.  
24. **B** - Em hotspots públicos, evitar dados sensíveis e usar VPN quando possível.  
25. **C** - Wi-Fi 6E e superiores consideram 2,4 GHz, 5 GHz e 6 GHz.

## Parte 5 - Segurança Cibernética

1. **A** - Segurança cibernética protege sistemas em rede e dados contra uso não autorizado ou prejudicial.  
2. **B** - Empresas devem proteger reputação, dados e clientes.  
3. **B** - Identidade off-line envolve dados pessoais de identificação.  
4. **B** - Identidade on-line é a forma de apresentação no ciberespaço.  
5. **B** - Dados corporativos incluem funcionários, propriedade intelectual e informações financeiras.  
6. **B** - CID significa Confidencialidade, Integridade e Disponibilidade.  
7. **A** - Confidencialidade restringe acesso inadequado.  
8. **A** - Integridade envolve precisão, consistência e confiabilidade.  
9. **B** - Disponibilidade garante acesso quando necessário a usuários autorizados.  
10. **A** - Violação envolve acesso não autorizado a dados, aplicações, redes ou dispositivos.  
11. **A** - Ameaças internas podem ser acidentais ou intencionais.  
12. **B** - Usuários internos têm acesso e conhecimento privilegiado.  
13. **A** - Ameaças externas exploram vulnerabilidades ou engenharia social.  
14. **A** - Engenharia social manipula pessoas para obter ações ou dados.  
15. **A** - Phishing usa mensagens fraudulentas disfarçadas de fonte confiável.  
16. **A** - Quebra de senha Wi-Fi busca descobrir a senha da rede sem fio.  
17. **A** - Firewall habilitado e atualizado é medida básica de proteção.  
18. **A** - Antivírus e antispyware reduzem riscos de softwares maliciosos.  
19. **A** - Sistemas, navegadores e patches devem ficar atualizados.  
20. **A** - Senhas e criptografia protegem dispositivos e dados.  
21. **B** - Alterar SSID/senha padrão e usar WPA2 protege a rede doméstica.  
22. **A** - Em Wi-Fi público, deve-se evitar dados sensíveis e usar VPN quando possível.  
23. **B** - IDS detecta, registra e relata tentativas de ataque.  
24. **A** - IPS busca impedir ataques, bloqueando tráfego por regras.  
25. **A** - VPN cria túnel criptografado seguro sobre a internet pública.
