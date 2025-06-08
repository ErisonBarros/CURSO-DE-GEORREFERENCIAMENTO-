---
icon: message-bot
---

# PPP-IBGE



***

### 🛰️ **Tutorial: Como Fazer o PPP no Site do IBGE**

#### ✅ **Pré-requisitos:**

* Ter um arquivo RINEX (.obs ou .yyO) gerado por receptor GNSS em dupla frequência
* Ter o arquivo de navegação correspondente (.nav ou .yyN)
* Ter pelo menos 1h de dados de rastreio (idealmente mais de 2h para maior precisão)
* Ter conexão com a internet

***

### 🔗 **Passo 1 – Acesse o site do PPP**

Acesse o link recomendado pelo IBGE para uso do serviço PPP:

👉[https://www.ibge.gov.br/geociencias/informacoes-sobre-posicionamento-geodesico/servicos-para-posicionamento-geodesico/16334-servico-online-para-pos-processamento-de-dados-gnss-ibge-ppp.html?=\&t=processar-os-dados](https://www.ibge.gov.br/geociencias/informacoes-sobre-posicionamento-geodesico/servicos-para-posicionamento-geodesico/16334-servico-online-para-pos-processamento-de-dados-gnss-ibge-ppp.html?=\&t=processar-os-dados)

Esse serviço é mantido pelo **NRCan (Natural Resources Canada)**, e aceito pelo IBGE como método confiável para processar dados GNSS.

***

### 📂 **Passo 2 – Carregar os Arquivos**

1. Na página do CSRS-PPP, localize a seção **"Upload your data files"**
2. Clique em **“Choose File”** e selecione o **arquivo RINEX (.obs, .yyO)**
3. Se desejar maior precisão ou quiser resultados mais rápidos, pode também fazer upload do **arquivo de navegação** e **arquivo meteorológico**, mas não são obrigatórios.

***

### ⚙️ **Passo 3 – Configurar as Opções**

Configure os parâmetros conforme sua necessidade:

* **Processing Mode**: escolha _Static_ (para levantamento parado) ou _Kinematic_ (se o receptor estava em movimento)
* **Coordinate System**: normalmente manter como _ITRF (current epoch)_ ou _NAD83(CSRS)_ se desejar coordenadas compatíveis com o SIRGAS
* **Antenna Type**: selecione o modelo exato da antena usada (essencial para corrigir o centro de fase)
* **Antenna Height**: informe a altura da antena ao ponto de referência (em metros)
* **Email Address**: insira seu e-mail para receber o relatório

***

### 📤 **Passo 4 – Enviar para Processamento**

* Após preencher os dados, clique em **"Submit to PPP"**
* Aguarde o processamento. Um e-mail será enviado com o link para o **relatório completo (PDF e TXT)**

***

### 📊 **Passo 5 – Interpretar os Resultados**

O relatório incluirá:

* Coordenadas em diferentes sistemas (ITRF, NAD83, etc.)
* Erros RMS e desvios
* Gráficos de convergência e qualidade
* Dados processados hora a hora
* Arquivo .pos com as coordenadas em cada época (se modo cinemático)

***

### 🧭 **Dica do IBGE:**

Embora o CSRS-PPP seja canadense, ele usa a constelação GPS/GNSS e efemérides de alta precisão aceitas internacionalmente. O IBGE recomenda seu uso especialmente para **pós-processamento de bases GNSS estáticas** em trabalhos de georreferenciamento rural.

{% embed url="https://youtu.be/8poPUjRHTSM?si=dAFLw86PugMpzNEw" %}

