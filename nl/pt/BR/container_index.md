---

copyright:
  years: 2014, 2018
lastupdated: "2018-08-06"

---

{:new_window: target="_blank"}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:pre: .pre}
{:table: .aria-labeledby="caption"}
{:codeblock: .codeblock}
{:tip: .tip}
{:download: .download}



# Introdução ao {{site.data.keyword.containerlong_notm}}
{: #container_index}

Tenha sucesso desde o início com o {{site.data.keyword.containerlong}} implementando apps altamente disponíveis em contêineres do Docker que são executados em clusters do Kubernetes.
{:shortdesc}

Os contêineres são uma maneira padrão de empacotar apps e todas as suas dependências para que seja possível mover perfeitamente os apps entre ambientes. Ao contrário de máquinas virtuais, os contêineres não empacotam o sistema operacional. Somente o código de app, o tempo de execução, as ferramentas de sistema, as bibliotecas e as configurações são empacotados dentro de contêineres. Os contêineres são mais leves, móveis e eficientes do que máquinas virtuais.


Clique em uma opção para começar:

<img usemap="#home_map" border="0" class="image" id="image_ztx_crb_f1b" src="images/cs_public_dedicated_options.png" width="440" alt="Clique em um ícone para iniciar rapidamente com o{{site.data.keyword.containershort_notm}}. Com o {{site.data.keyword.Bluemix_dedicated_notm}}, clique neste ícone para ver suas opções." style="width:440px;" />
<map name="home_map" id="home_map">
<area href="#clusters" alt="Introdução aos clusters do Kubernetes em{{site.data.keyword.Bluemix_notm}}" title="Introdução aos clusters do Kubernetes em{{site.data.keyword.Bluemix_notm}}" shape="rect" coords="-7, -8, 108, 211" />
<area href="cs_cli_install.html" alt="Instalar as CLIs." title="Instalar as CLIs." shape="rect" coords="155, -1, 289, 210" />
<area href="cs_dedicated.html#dedicated_environment" alt="{{site.data.keyword.Bluemix_dedicated_notm}} ambiente de nuvem" title="{{site.data.keyword.Bluemix_notm}} ambiente de nuvem" shape="rect" coords="326, -10, 448, 218" />
</map>


## Introdução aos clusters
{: #clusters}

Então você deseja implementar um app em um contêiner? Espere! Inicie criando um cluster do Kubernetes primeiro. Kubernetes é uma ferramenta de orquestração para contêineres. Com o Kubernetes, os desenvolvedores podem implementar apps altamente disponíveis em um flash usando o poder e a flexibilidade de clusters.
{:shortdesc}

E o que é um cluster? Um cluster é um conjunto de recursos, nós de trabalhador, redes e dispositivos de armazenamento que mantêm os apps altamente disponíveis. Após ter o seu cluster, é possível implementar seus apps em contêineres.

**Antes de começar**

Obtenha o tipo de [conta do {{site.data.keyword.Bluemix_notm}}](https://console.bluemix.net/registration/) certo para você:
* **Pré-paga ou Assinatura**: é possível criar um cluster de avaliação grátis. Também é possível provisionar os recursos de infraestrutura do IBM Cloud (SoftLayer) para criar e usar em clusters padrão.
* **Lite**: não é possível criar um cluster grátis ou padrão. [Faça upgrade de sua conta](/docs/account/account_faq.html#changeacct) para Pré-paga ou Assinatura.
* **Avaliação (para propósitos educacionais)**: é possível criar um cluster grátis que pode ser usado por 30 dias para se familiarizar com o serviço.

Para criar um cluster grátis:

1.  No [**Catálogo** do {{site.data.keyword.Bluemix_notm}} ![Ícone de link externo](../icons/launch-glyph.svg "Ícone de link externo")](https://console.bluemix.net/catalog/?category=containers), selecione **{{site.data.keyword.containershort_notm}}** e clique em **Criar**. Uma página de configuração do cluster é aberta. Por padrão, o **grátis cluster** é selecionado.

2. Forneça seu cluster um nome exclusivo.

3.  Clique em **Criar Cluster**. É criado um conjunto de trabalhadores que contém 1 nó do trabalhador. O nó do trabalhador pode demorar alguns minutos para provisionar, mas é possível ver o progresso na guia **Nós do trabalhador**. Quando o status atinge `Ready`, é possível começar a trabalhar com seu cluster!

Bom Trabalho! Você criou seu primeiro cluster do Kubernetes. Aqui estão alguns detalhes sobre seu cluster grátis:

*   **Tipo de máquina**: o cluster grátis tem um nó do trabalhador virtual que é agrupado em um conjunto de trabalhadores, com 2 CPUs, 4 GB de memória e um único disco SAN de 100 GB disponível para seus apps usarem. Ao criar um cluster padrão, é possível escolher entre máquinas físicas (bare metal) ou virtuais, juntamente com vários tamanhos de máquina.
*   **Mestre gerenciado**: o nó do trabalhador é monitorado e gerenciado centralmente por um mestre do Kubernetes pertencente ao {{site.data.keyword.IBM_notm}} dedicado e altamente disponível que controla e monitora todos os recursos do Kubernetes no cluster. É possível concentrar-se em seu nó do trabalhador e nos apps implementados nele sem se preocupar também com o gerenciamento desse mestre.
*   **Recursos de infraestrutura**: os recursos que são necessários para executar o cluster, como VLANS e endereços IP, são gerenciados em uma conta de infraestrutura do IBM Cloud (SoftLayer) pertencente à {{site.data.keyword.IBM_notm}}. Ao criar um cluster padrão, você gerencia esses recursos em sua própria conta de infraestrutura do IBM Cloud (SoftLayer). É possível aprender mais sobre esses recursos e as [permissões necessárias](cs_users.html#infra_access) ao criar um cluster padrão.
*   **Outras opções**: clusters grátis são implementados na região que você seleciona, mas não é possível escolher qual zona. Para controlar a zona, a rede e o armazenamento persistente, crie um cluster padrão. [Saiba mais sobre os benefícios de clusters grátis e padrão](cs_why.html#cluster_types).


**O que vem a seguir?**</br>
Experimente algumas coisas com seu cluster grátis antes de expirar.

* Acesse o [primeiro tutorial do {{site.data.keyword.containershort_notm}}](cs_tutorials.html#cs_cluster_tutorial) para criar um cluster do Kubernetes, instalar a CLI, criar um registro privado, configurar seu ambiente de cluster e incluir um serviço em seu cluster.
* Mantenha seu ritmo com o [segundo tutorial do {{site.data.keyword.containershort_notm}}](cs_tutorials_apps.html#cs_apps_tutorial) sobre a implementação de apps no cluster.
* [Crie um cluster padrão](cs_clusters.html#clusters_ui) com múltiplos nós para disponibilidade mais alta.


