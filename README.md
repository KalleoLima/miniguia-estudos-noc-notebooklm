# 🛡️ Miniguia de Estudos: NOC (Network Operations Center)

Este repositório contém um Caderno Temático construído com o apoio de Inteligência Artificial (NotebookLM), focado em explorar as rotinas, conceitos e ferramentas essenciais para um Centro de Operações de Rede (NOC). O projeto é fruto do desafio de Aprendizagem Ativa da DIO.

---

## 🎯 Contexto e Objetivos

* **Tema:** Fundamentos e Monitoramento de Redes em um NOC.
* **Objetivos de Estudo:** Compreender o papel de um analista de NOC, mapear as principais ferramentas de monitoramento de infraestrutura e criar um glossário de termos essenciais da área para consultas rápidas.

---

## 📚 Curadoria de Fontes

Para garantir que a IA não gerasse informações incorretas (alucinações), alimentei o NotebookLM estritamente com os seguintes materiais:

1. **Revista Fatec (Interface Tecnológica)** - [Acesse o artigo](https://revista.fatectq.edu.br/interfacetecnologica/pt_BR/article/view/2090)
2. **Allied IT (NOC: O coração das operações de TI)** - [Acesse o artigo](https://alliedit.com.br/noc-o-coracao-das-operacoes-de-ti/)
3. **Allied IT (Plano de Resposta a Incidentes)** - [Acesse o artigo](https://alliedit.com.br/plano-de-resposta-a-incidentes/)
4. **IBM (Network Operations Center)** - [Acesse o artigo](https://www.ibm.com/br-pt/think/topics/network-operations-center)
5. **Faculdade de Imperatriz (FACIMP)** - Artigo em PDF: *Ferramentas de Gerenciamento de Redes de Computadores*.

---

## 🧠 Engenharia de Prompts e "Cicatrizes"

Durante a construção deste guia, utilizei a técnica de delimitação de escopo. 

**Prompt Principal Utilizado:**
> *"Com base estritamente nestes documentos, crie um resumo estruturado usando tópicos (bullet points) sobre as principais responsabilidades de um analista de NOC e as ferramentas que ele costuma utilizar."*

**Análise Crítica (Troubleshooting):**
A experiência com o NotebookLM foi altamente direta. Ao utilizar uma curadoria prévia de fontes confiáveis em formato PDF, a IA conseguiu extrair conceitos técnicos sem alucinar ou misturar conceitos de áreas correlatas (como SOC/Segurança). A restrição do banco de dados da IA provou ser uma tática excelente para estudos objetivos.

---

## 📖 Miniguia de Estudo

### Resumo: O Papel do Analista de NOC

**Principais Responsabilidades:**
* **Monitoramento e Gerenciamento Contínuo:** Realizar a supervisão em tempo real (24/7) da infraestrutura de rede, incluindo servidores, bancos de dados, firewalls e dispositivos, para garantir conectividade e disponibilidade.
* **Tratamento de Incidentes e Falhas:** Detectar, isolar e resolver anormalidades e problemas de conectividade, minimizando o tempo de inatividade (downtime).
* **Escalonamento de Problemas:** Atuar em uma estrutura de camadas (Níveis 1 a 3), onde incidentes mais graves ou complexos, como ataques de ransomware, são encaminhados para técnicos mais experientes.
* **Manutenção e Atualização de Sistemas:** Instalar e atualizar softwares em sistemas conectados, além de realizar o gerenciamento de correções (patches) e suporte antivírus.
* **Gestão de Configuração e Inventário:** Manter bases de dados de configuração atualizadas e realizar o inventário de hardware e software da rede.
* **Proteção e Segurança de Dados:** Monitorar firewalls e softwares de segurança, identificar malwares e vulnerabilidades, além de gerenciar backups e planos de recuperação de desastres.
* **Análise de Desempenho e Capacidade:** Medir e controlar a performance dos componentes da rede, analisando o perfil do tráfego e planejando a expansão da capacidade conforme a necessidade.
* **Gestão de Contabilidade e Acesso:** Registrar e controlar o acesso de usuários e dispositivos aos recursos da rede, alocando privilégios e verificando utilizações que possam sobrecarregar o tráfego.

**Ferramentas Utilizadas:**
* **Protocolo SNMP:** Principal protocolo de gerência utilizado para facilitar o intercâmbio de informações entre dispositivos de rede e estações de gerenciamento.
* **Zabbix:** Utilizada para monitorar a performance e a disponibilidade de ativos como servidores, switches e roteadores.
* **Nagios:** Aplicação para monitorar clientes e serviços, enviando alertas quando surgem problemas e quando são resolvidos.
* **OpenNMS:** Ferramenta premiada capaz de monitorar a disponibilidade de serviços, coletar dados de performance e gerenciar eventos e notificações.
* **MRTG (Multi Router Traffic Grapher):** Gera gráficos de tráfego de rede a partir de dados coletados via SNMP.
* **Ntop:** Demonstra informações detalhadas e gráficos sobre o tráfego de rede e protocolos (TCP/UDP, ICMP, etc.).
* **IBM Netcool Operations Insight e Watson:** Tecnologias avançadas e cognitivas usadas para monitorar grandes volumes de elementos e transformar a operação em preditiva através de inteligência artificial.
* **SpiceWorks:** Software que combina monitoramento, inventário de rede, relatórios e suporte (Help Desk).
* **Ferramentas de Segurança:** Incluem o Wireshark (análise de protocolos), Snort (detecção de intrusão), Nessus e GFI LANguard (scanners de vulnerabilidades).
* **Outras Ferramentas:** Angel (monitoramento gráfico), IPPL e HIDS OSSEC (análise de tráfego).

### Glossário de Termos Técnicos

* **NOC (Network Operations Center):** Local centralizado para o monitoramento e gerenciamento contínuo (24/7) de redes, telecomunicações ou satélites.
* **SNMP (Simple Network Management Protocol):** Protocolo padrão da camada de aplicação utilizado para facilitar a troca de informações de gerência entre dispositivos de rede.
* **Downtime (Tempo de inatividade):** Período em que os sistemas de rede ficam indisponíveis, sendo o principal objetivo do NOC minimizá-lo.
* **MIB (Management Information Base):** Base de dados estruturada em árvore que contém objetos que representam o estado dos recursos gerenciáveis da rede.
* **FCAPS:** Modelo que define as cinco áreas funcionais do gerenciamento: Falhas, Configuração, Contabilidade (Accounting), Desempenho (Performance) e Segurança.
* **SOC (Security Operations Center):** Centro focado na segurança da informação, realizando análise de ameaças e mitigação de ataques cibernéticos.
* **Firewall:** Dispositivo ou software de segurança monitorado pelo NOC para proteger a rede contra acessos não autorizados.
* **Agente (Agent):** Processo associado a um elemento de rede que responde a requisições do gerente e o notifica sobre eventos.
* **Gerente (Manager):** Estação de gerenciamento que solicita informações de monitoramento aos agentes e as traduz para os operadores.
* **Observabilidade de rede:** Uso de IA e automação para analisar dados rapidamente e corrigir problemas proativamente em milhões de endpoints.

### Prompts de Revisão

1. *"Qual é o principal protocolo de gerência de redes citado como a ferramenta padrão utilizada largamente desde o final dos anos 80 até os dias atuais?"*
2. *"Em qual camada do modelo OSI (Open Systems Interconnection) o protocolo SNMP está localizado?"*
