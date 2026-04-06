- Toda aplicação de rede é um conjunto de programas em sistemas finais diferentes que comunicam entre si
- O software de aplicação é confinado aos sistemas finais 
- A inteligência de aplicação é separada da inteligencia de rede (inteligencia de redes fica nas camadas inferiores)
### Arquiteturas de aplicação
- Existem 2 grandes arquiteturas de aplicação:
	- Arquitetura cliente-servidor: Servidor sempre ligado com IP fixo, clientes não comunicam entre si, escabilidade via data centers, web (HTTP), FTP, SMTP, o custo é a infraestrutura do servidor
	- Arquitetura P2P (Peer-to-peer):  Sem servidor dedicado central, autoescalável por natureza, BitTorrent, desafios: ISP, segurança, incentivos
- P2P é autoescalável porque cada novo par que chega também traz capacidade de upload. Na arquitetura cliente-servidor, mais usuários = mais carga no servidor. Em P2P, mais usuários = mais recursos disponíveis
### Comunicação entre processos
- Processos são programas em execução 
- Cliente: O processo que inicia a comunicação
- Servidor: O processo que espera ser contactado 
- O que faz a comunicação entre o cliente e o servidor é o socket 
	- Socket: Interface (API) entre o processo e a rede, a "porta" pela qual o processo envia e recebe dados. É a fronteira entre a camada de aplicação e a camada de transporte
	- ![[Captura de Tela 2026-04-06 às 15.24.59.png]]