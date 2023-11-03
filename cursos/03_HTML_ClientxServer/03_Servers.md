# Servidores

São computadores que se comportam de modo diferente em relação ao *Client*. Servidores podem operar pela internet ou em rede local, é uma espécie de *computador central* que guarda alguns arquivos que servem para atender a requisições de computadores *clients* ligados a ele.

Normalmente é um computador mais robusto, pois precisa de uma capacidade maior de processamento para responder às requisições. Podem servir para armazenar arquivos de mídia, segurança, streaming de dados, emails, web enfim, para atender às mais diversas necessidades de uma rede.

## Hardwares &  Softwares em Servidores

Todo computador, servidor ou não, é baseado em duas partes: a parte lógica e a parte física. Ou seja, software e hardware. A diferença entre os dois é que o software é toda a parte que não é tangível e faz o sistema funcionar e o hardware são as peças do equipamento. Como disse uma vez um amigo: software nós xingamos e hardware nós chutamos. Abaixo uma tabela esquematiza a relação:

|**Softwares**        |**Hardwares**          |
|:-------------------:|:---------------------:|
|Sistemas Operacionais|Discos de Armazenamento|
|Monitoramento        |Memórias               |
|Servidores Web       |Processadores          |

### Sistemas Operacionais

Em servidores, os SOs mais comuns são Windows Server, Ubuntu, Fedora, Debian, Oracle Linux e CentOS. Cada um com sua particularidade, todos eles são voltados para atender à questões específicas de servidores. Todos eles são baseados em sistemas UNIX.

No caso de servidores Web, precisamos de aplicativos específicos para esse trabalho. Hoje em dia, os mais conhecidos são: Apache e Nginx. Os servidores web serão responsáveis por atender e responder às requisições HTTP.

O uso de servidores web significam, na prática, lidar com custos de manutenção de um site no ar. Servidores baseados em Linux costumam ser mais baratos por não terem gastos com licenças, como servidores Windows, por exemplo.

## Tipos de Servidores

Como já vimos anteriormente, existem vários tipos de servidores:

- Arquivos;
- Segurança (Firewall);
- Streaming;
- Email;
- Proxy
- Web

Por exemplo, servidores **Proxy** são importantes por serem servidores intermediários que estabelecem critérios de segurança e autenticação para acessos à internet. Eles podem impedir acesso a sites maliciosos ou sites que contenham informações sensíveis.

Servidores do tipo **Firewall** protegem o sistema de ataques externos, tornando a navegação mais segura. Servidores também podem ser do tipo **Email**, que operam para o funcionamento deste serviço. Ou ainda, do tipo **Database** que provêem comunicação entre aplicações e bancos de dados.

Podemos utilizar um servidor para operar **Intranet**, que são serviços web que funcionam somente a um nível local. Um servidor muito comum é o **DNS** (*Domain Name Service*), que possuem uma lista de nomes associados a IPs. É o que permite que digitemos um nome de um site para acessarmos. Por exemplo, podemos digitar `uol.com.br`, ao invés de `200.221.2.45`. Tornando tudo muito mais simples.

## Hospedagem de Sites

Hospedar um site é armazenar o conteúdo de um site em um servidor web, permitindo o acesso do seu público ao conteúdo. Neste caso, podemos contratar um servidor ou manter um servidor próprio, dedicado ao serviço (o que é muito mais complicado).

Além disso, temos o registro de domínio em um servidor DNS para que seja possível acessar o site através de um endereço http. É um serviço de taxa anual de baixo custo.

Após contratados os serviços de hospedagem e domínio, precisamos efetuar uma conexão ftp direta ao servidor, para trocarmos arquivos com o servidor para efetuarmos mano, produção e atualização do conteúdo de nosso site. Utilizamos normalmente o aplicativo **Filezilla** para essa operação.