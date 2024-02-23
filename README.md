<h1>Elastic SIEM Lab</h1>

### [A Simple Elastic SIEM Lab](https://medium.com/@aali23/a-simple-elastic-siem-lab-6765159ee2b2)

<h2>Descrição</h2>
Esse projeto tem como objetivo configurar um SIEM robusto usando o Elastic Stack. Meu principal objetivo otimizar a coleta de logs e a transmissão para a plataforma SIEM usando Elastic Agents, em conjunto apromorei minhas habilidades em análise de eventos de segurança e detecção de ameaças.

<br />


<h2>Utilitários usados</h2>

- <b>VMWare</b>
- <b>Bash</b>
- <b>Nmap</b>
- <b>Elastic</b>

<h2>Ambientes usados</h2>

- <b>Kali</b>

<h2>Passo a passo do projeto:</h2>

<p align="center">
<b>Criando os recursos iniciais</b> <br/>
  Primeiro, foi criado uma máquina virtual Kali com VMWare. Feito isso, foi criado uma conta gratuita na Elastic Cloud (https://cloud.elastic.co/registration). 
<br />
<br />

<p align="center">
<b>Criação do agente para coleta de logs</b> <br/>
  Um agente é um programa de software que é instalado em um dispositivo, como um servidor ou endpoint, para coletar e enviar dados a um sistema centralizado para análise e monitoramento. No contexto do Elastic SIEM, um agente é usado para coletar e encaminhar eventos de segurança dos seus endpoints para a sua instância do Elastic SIEM.
  Foi criada uma integração com o Elastic Defend
  <img src="https://i.imgur.com/PDhBbsL.png" height="80%" width="80%" alt="Integration"/>

<p align="center">
  Instalado no Kali e verificado seu status
  <img src="https://i.imgur.com/r8j2Tzs.png" height="80%" width="80%" alt="Installing"/>
  <img src="https://i.imgur.com/FbdlWQW.png" height="80%" width="80%" alt="Status check"/>
  
<br />
<br />

<p align="center">
<b>Geração de eventos com nmap e análise de logs</b> <br/>
  Através do NMap, foram feitos scans na rede do próprio host
  <img src="https://i.imgur.com/8z6UHpi.png" height="80%" width="80%" alt="Nmap Scan"/>

<p align="center">
   Isso possibilitou a análise dos eventos no Elastic SIEM.
  <img src="https://i.imgur.com/IaAQszV.png" height="80%" width="80%" alt="Logs"/>
  <img src="https://i.imgur.com/GzZrIlE.png" height="80%" width="80%" alt="Detailed Logs"/>

<br />
<br />

<p align="center">
<b>Dashboard e visualização dos eventos</b> <br/>
  O Elastic SIEM fornece ferramentas para análise de eventos específicos como o comando "sudo".
  <img src="https://i.imgur.com/FAHVQRp.png" height="80%" width="80%" alt="Dashboard"/>

<br />
<br />

<p align="center">
<b>Geração do alerta</b> <br />
  Por fim, foi criado um alerta onde ele monitora todas as atividades que correspondam o scan do nmap.
  <img src="https://i.imgur.com/9QvL7uy.png" height="80%" width="80%" alt="Dashboard"/>

<br />
<br />

<p align="center">
<b>Conclusão</b> <br />
  Esse laboratório fornece um ambiente valioso para aprendizado e prática das habilidades necessárias para monitoração de segurança efetiva e respostas a incidentes usando o Elastic SIEM.
  
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
