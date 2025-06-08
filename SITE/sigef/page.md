# Explicação Sigef

####

{% embed url="https://drive.google.com/file/d/1ZGgysmmHGELjO7Qqkx_zwUYLp0n6Ce42/view?usp=drive_link" %}
PODCAST
{% endembed %}

#### 1. O Sistema de Gestão Fundiária (SIGEF)

O SIGEF é uma **ferramenta eletrônica desenvolvida pelo Incra para subsidiar a governança fundiária do território nacional.** ("manual\_geo\_imoveis.pdf", Seção 1.2.12). Ele substituiu o Sistema Nacional de Certificação de Imóveis Rurais (SNCI), embora as certificações emitidas pelo SNCI ainda sejam válidas e seu banco de dados seja utilizado para análise de sobreposições ("manual\_geo\_imoveis.pdf", Seção 1.2.13).

**1.1. Planilha Eletrônica do SIGEF**

A espinha dorsal do processo no SIGEF é uma planilha eletrônica, preferencialmente utilizada com LibreOffice e a extensão SIGEF. Esta planilha é organizada em abas para diferentes tipos de dados.

**1.1.1. Abas e Preenchimento:**

* **Aba de Identificação:** Contém informações cruciais sobre o serviço de georreferenciamento, a natureza do serviço, identificação do(a) detentor(a) (tipo de pessoa, nome, CPF/CNPJ), e identificação da área (Denominação, Situação, Natureza da área, Código do imóvel, CNS, Matrícula, Município).
* A 'Situação' da área pode ser:

1. "Imóvel Registrado" (com matrícula ou transcrição).
2. "Área Titulada não Registrada" (titulada, mas ainda não inscrita).
3. "Área não Titulada" (sem título de domínio, usada para georreferenciamento de áreas passíveis de titulação, como usucapião ou regularização fundiária) ("SIGEF - Sistema de Gestão Fundiária", "Aba de Identificação – Área georreferenciada").

* **Aba de Perímetro:** Detalha as composições da área georreferenciada, suportando diversas situações geométricas:
* **Situação 1 – Uma parcela:** A área é um único polígono.
* **Situação 2 – Múltiplas parcelas:** A área é composta por mais de uma parcela, exigindo uma aba de perímetro para cada parcela, com um número único para cada uma. Após a certificação, cada parcela recebe um código independente ("SIGEF - Sistema de Gestão Fundiária", "Situação 2 – Múltiplas parcelas").
* **Situação 3 – Parcela com vazio interno ou área encravada:** Representada por um polígono externo e um ou mais polígonos internos. O campo 'Lado' indica 'Externo' ou 'Interno', e o 'Parcela número' deve ser o mesmo para os lados externo e interno da mesma parcela encravada ("SIGEF - Sistema de Gestão Fundiária", "Situação 3 – Parcela com vazio interno ou área encravada").
* **Situação 4 – Situações combinadas.**
* **Dados de Vértices:** Inserção de coordenadas (UTM ou geodésicas/geográficas), Sigmas (desvios padrão em metros, com duas casas decimais, ex: "0,18"), altitude elipsoidal e método de posicionamento.
* As coordenadas UTM devem respeitar os limites do fuso e usar vírgula como separador decimal. Coordenadas geodésicas usam espaço entre graus, minutos e segundos, com vírgula para as casas decimais dos segundos ("SIGEF - Sistema de Gestão Fundiária", "Coordenadas UTM", "Coordenadas geodésicas/geográficas", "Sigmas").
* **Dados de Limites:** Inclui o tipo de limite (seguindo o Manual Técnico de Limites e Confrontações), confrontante, CNS, matrícula e descritivo.
* **Verificação de Erros na Planilha:** O sistema verifica automaticamente diversos erros, como cruzamento de perímetros, sistemas de referência inconsistentes, códigos de vértice repetidos, códigos de vértice inválidos, tipos de limite ou métodos de posicionamento incorretos, e desvio padrão dos vértices fora dos limites ("SIGEF - Sistema de Gestão Fundiária", "Verificação de Erros na Planilha").

**1.2. Situação Jurídica do Imóvel Rural para Georreferenciamento**

O imóvel rural para georreferenciamento pode ser "aquele objeto do título de domínio, bem como aquele passível de titulação" ("manual\_geo\_imoveis.pdf", Seção 1.2.6).

* **Imóvel rural objeto de título de domínio:**&#xC1;rea matriculada ou transcrita em cartório.
* Área descrita em documento não registrado, mas suscetível de registro.
* **Imóvel rural passível de titulação:**&#xC1;rea pública ocupada por particular, incluída em ação de regularização fundiária (será certificada após a emissão do título) ("in\_77.pdf", § 1º; "manual\_geo\_imoveis.pdf", Seção 2.2.2).
* Área sobre a qual é exercida a posse _ad usucapionem_ (usucapião judicial ou extrajudicial). Nesses casos, as peças técnicas prévias são geradas sem a confirmação da submissão no sistema, e a certificação só ocorre após a titulação por órgão público competente, sentença judicial transitada em julgado, ou reconhecimento extrajudicial de usucapião ("orientacoes\_usocapiao\_nt\_3448\_2021", Seção 4.2.3.3, 4.2.3.4, 4.2.4.1; "manual\_geo\_imoveis.pdf", Seção 2.2.2).
* Em caso de auditoria, se não for apresentado o Mandado de Registro ou Certidão de Qualificação Registral Positiva, a certificação poderá ser cancelada ("orientacoes\_usocapiao\_nt\_3448\_2021", Seção 4.2.4.1).

#### 2. Georreferenciamento de Imóveis Rurais: Conceitos e Métodos

O georreferenciamento busca a "certificação de poligonais referentes a limites de imóveis rurais" ("manual\_gestao\_certif\_v2.pdf", Seção 1).

**2.1. Identificação do Imóvel Rural**

A identificação se dá pela "correta descrição dos seus limites" ("manual\_geo\_imoveis.pdf", Seção 1.3).

* **Vértice de Limite:** "É o ponto onde a linha limítrofe do imóvel rural muda de direção ou onde existe interseção desta linha com qualquer outra linha limítrofe de imóvel contíguo" ("manual\_geo\_imoveis.pdf", Seção 1.2.11, 2.4.2).
* **Codificação do Vértice:** O código do vértice é composto pelo "Código do credenciado", "Tipo do vértice" e "Número do vértice" (ex: AAAA-M-9999) ("manual\_geo\_imoveis.pdf", Seção 1.3.3). Os tipos de vértices são "M" (marco), "P" (ponto), e "V" (virtual) ("manual\_geo\_imoveis.pdf", Tabela 2).

**2.2. Tipos de Limites**

O Manual Técnico de Limites e Confrontações define diversos tipos de limites, com seus respectivos códigos ("manual\_geo\_imoveis.pdf", Seção 2.4.1, Tabela 1):

* **Limites Artificiais:**&#x4C;A1: Cerca
* LA2: Muro
* LA3: Estrada
* LA4: Vala
* LA5: Canal
* LA6: Linha ideal (linha reta imaginária, descrita pelos vértices extremos) ("manual\_geo\_imoveis.pdf", Seção 2.1.1).
* LA7: Limite artificial não tipificado.
* **Limites Naturais:**&#x4C;N1: Corpo d’água ou curso d’água
* LN2: Linha de cumeada
* LN3: Grota
* LN4: Crista de encosta
* LN5: Pé de encosta
* LN6: Limite natural não tipificado.

**2.3. Coordenadas e Precisão Posicional**

* **Coordenadas Geodésicas:** Expressas em ($\phi$, $\lambda$, h) com suas precisões ($\sigma\phi$, $\sigma\lambda$, $\sigma$h) ("manual\_geo\_imoveis.pdf", Seção 1.2.7).
* **Precisão Posicional Absoluta:** Relacionada à vinculação com o Sistema Geodésico Brasileiro (SGB) ("manual\_geo\_imoveis.pdf", Seção 1.2.8).
* **Padrões de Precisão:**&#x56;értices em limites artificiais: melhor ou igual a 0,50 m.
* Vértices em limites naturais: melhor ou igual a 3,00 m.
* Vértices em limites inacessíveis: melhor ou igual a 7,50 m.
* A tolerância admitida é de no máximo três vezes o valor da precisão para o tipo de limite ("manual\_geo\_imoveis.pdf", Seção 1.4.4).
* Os valores de desvio padrão (sigma) dos vértices georreferenciados não podem extrapolar os limites definidos na NTGIR 3ª edição ("SIGEF - Sistema de Gestão Fundiária", Erro 18).

**2.4. Métodos de Posicionamento**

O manual detalha "o conjunto de normas para execução dos serviços de georreferenciamento de imóveis rurais, que, em comparação com a versão anterior do Manual, trouxe uma maior possibilidade de técnicas que podem ser empregadas em casos específicos" ("manual\_geo\_imoveis.pdf", Considerações).

* **Posicionamento Direto:** Ocupa-se diretamente o vértice de interesse com um instrumento de medição.
* **Posicionamento Indireto:** Não há ocupação direta do vértice por um instrumento de medição ("manual\_geo\_imoveis.pdf", Seção 3.7).

Os métodos incluem:

* **GNSS (Global Navigation Satellite System):** Abrange sistemas como GPS, GLONASS, Galileu. O posicionamento relativo é crucial, utilizando a fase da onda portadora para maior precisão, sendo a única observável aceita para vértices de apoio e limites artificiais. A pseudodistância é permitida para limites naturais ("manual\_geo\_imoveis.pdf", Seção 3.1).
* Tipos: Estático, Estático-rápido, Semicinemático, Cinemático, e a partir de códigos.
* RTK (Real-Time Kinematic) e DGPS (Differential GPS) também são métodos GNSS. O IBGE oferece um serviço gratuito de RTK em rede via NTRIP ("manual\_geo\_imoveis.pdf", Seção 3.1.2.2).
* **Topografia Clássica:** Inclui métodos como Poligonação, Triangulação, Trilateração, Triangulateração, Irradiação, Interseção Linear, Interseção Angular, Alinhamento, e Estação Livre ("manual\_geo\_imoveis.pdf", Seção 3.2).
* **Geometria Analítica:** Posicionamento indireto onde as coordenadas são determinadas por cálculos analíticos a partir de vértices posicionados diretamente ("manual\_geo\_imoveis.pdf", Seção 3.3).
* **Aerolevantamento (Dados Aeroespaciais):** Inclui aerofotogrametria, radar aerotransportado, laser scanner aerotransportado, e sensores orbitais. Exige avaliação de acurácia posicional absoluta e, para laser scanner aerotransportados, habilitação pelo Ministério da Defesa e homologação da ANAC ("manual\_geo\_imoveis.pdf", Seção 3.4, 3.4.1). Produtos como ortomosaicos, ortofotocartas, MDT e MDS são utilizados ("manual\_geo\_imoveis.pdf", Seção 3.4.1).
* **Base Cartográfica:** Com ou sem precisão conhecida. Utilizado para feições de difícil definição ou limites inacessíveis ("manual\_geo\_imoveis.pdf", Seção 3.5.1, 3.5.2).

**2.5. Cálculo de Área e Distância**

* O cálculo de área deve ser realizado com base nas **coordenadas cartesianas locais referenciadas ao Sistema Geodésico Local (SGL)**, usando a fórmula de Gauss, e expresso em hectares. Isso proporciona resultados que "expressam melhor a realidade física" em comparação com o Sistema UTM, que era adotado anteriormente ("manual\_geo\_imoveis.pdf", Seção 3.8.3).
* A distância horizontal deve ser expressa em metros ("manual\_geo\_imoveis.pdf", Seção 3.8.4).

#### 3. Gestão da Certificação: Desmembramento, Remembramento e Atualização

O SIGEF e os manuais detalham os procedimentos para alterações em parcelas certificadas.

**3.1. Desmembramento**

Ação de fracionar uma parcela certificada. Para parcelas com registro confirmado, exige-se que o perímetro certificado do Projeto de Assentamento também esteja confirmado no Sigef ("manual\_gestao\_certif\_v2.pdf", Seção 4.2).

* **Rejeição automática** do requerimento em situações como supressão de vértices originais, espaço vazio entre parcelas do desmembramento, ou sobreposição com outras parcelas no SIGEF sem limite comum ("manual\_gestao\_certif\_v2.pdf", Rejeição Automática; "req\_desm\_oc\_1237\_2022.pdf", Rejeição Automática).
* Regras específicas aplicam-se quando há parcelas confrontantes de natureza "Assentamento" ou "Assentamento Parcela", ou com situação "Aguardando Aprovação por Fiscalização" ou "Área Não Titulada" ("req\_desm\_oc\_1237\_2022.pdf", v, vi).

**3.2. Remembramento**

Ação de fundir duas ou mais parcelas certificadas, com registro confirmado ("manual\_gestao\_certif\_v2.pdf", Seção 4.3). Permite fusionar áreas contíguas de diferentes títulos em uma única parcela ("manual\_geo\_imoveis.pdf", Seção 2.2.1).

**3.3. Atualização de Parcela**

Permite alterar informações dos vértices de limite de uma parcela certificada, incluindo código, altitude, e inclusão de novos vértices em limites existentes ("manual\_gestao\_certif\_v2.pdf", Seção 4.4).

* A inclusão de novos vértices do tipo "V" (virtual) exige avaliação do analista sobre a necessidade e os dados que subsidiaram as coordenadas ("req\_atua\_parc\_oc\_987\_2023.pdf", Seção 1.1.2).
* Tolerâncias específicas são aplicadas para a inclusão de vértices em limites comuns a parcelas confrontantes (0 a 0,5m: automática; 0,5 a 9,0m: mediante análise; acima de 9,0m: não permitida) ("manual\_geo\_imoveis.pdf", Tabela 3; "req\_atua\_parc\_oc\_987\_2023.pdf", Seção 1.1.3).

**3.4. Retificação**

Permite corrigir informações de parcelas certificadas, incluindo retificação de atributos comuns em parcelas vinculadas (multiabas) e retificação da situação e natureza da área ("manual\_gestao\_certif\_v2.pdf", Seção 6.3, 6.4).

#### 4. Fiscalização e Sanções

O INCRA realiza auditorias nas certificações e pode propor sanções a credenciados por erros nos serviços de georreferenciamento, procedimentos de certificação e requerimentos indevidos ("manual\_gestao\_certif\_v2.pdf", Seção 9, 11.5).

* **Erros posicionais:** Relacionados à obtenção e processamento de coordenadas (ex: dados não processados, ausência de ajuste).
* **Erros de definição de limites e domínio:** Relacionados à identificação, levantamento e descrição dos limites e sua correspondência com o documento de domínio. A certificação de parte ou todo com dados de título de domínio inexistente ou fraudado pode levar ao descredenciamento ("manual\_gestao\_certif\_v2.pdf", Seção 11.5.1, 11.5.2).

#### 5. Documentação e Normas

Vários documentos e normas são fundamentais para o processo:

* Lei nº 6.015/1973 (Lei de Registros Públicos)
* Decreto nº 4.449/2002 e Decreto nº 5.570/2005
* Instrução INCRA nº 77/2013 (regulamenta a certificação) ("in\_77.pdf", Seção 2.4).
* Portaria INCRA/P/486/2013 (homologa a 3ª Edição da Norma Técnica de Georreferenciamento de Imóveis Rurais - NTGIR) ("orientacoes\_usocapiao\_nt\_3448\_2021", Seção 2.5). A Portaria nº 205 também aprova o "Manual Técnico para Georreferenciamento de Imóveis Rurais - MTGIR - 2º" ("portaria\_205.pdf").
* Manual Técnico de Limites e Confrontações e Manual de Posicionamento (mencionados para detalhes específicos de campo e métodos de levantamento).



c
