
## **Analise classe economica clientes - ACLScript**

Esse projeto se propõe a criar uma variável muito importante na segmentação do cliente que é composta por muitas outras, mas iremos focar na criação da classe econômica dos clientes de uma financeira (fictícia).

A grande maioria dos clientes quando necessitam de um empréstimo entregam os documentos em formato de PDF, incluindo o contracheque e nesse caso iremos usar todos esses contracheques para criação de uma base consolidada para que a seguir possamos segmentar os clientes nas seguintes classes de renda:

|CLASSES|LIMITE INFERIOR|LIMITE SUPERIOR|
|--|--|--|
| Classe E | R$ 0 | R$ 1.254 |
| Classe D | R$ 1.255 | R$ 2.004 |
| Classe C | R$ 2.005 | R$ 8.640 |
| Classe B | R$ 8.641 | R$ 11.261 |
| Classe A | R$11.262 | - |

#### Fonte: http://cps.fgv.br/qual-faixa-de-renda-familiar-das-classes 

Essa é uma análise *hands on* para atendimento de uma necessidade pontual, considerando que financeiras e outras empresas que trabalham com dados tão sensíveis assim tem sistemas informatizados para tratar esse tipo de informação, mas a proposta aqui é demostrar a extração de dados a partir de uma fonte não muito convencional como o PDF e a transformação desses arquivos em uma única base para ser usada na definição da classe econômica do cliente.

----------

### Arquivos originais

![](https://github.com/Renatoelho/Analise-classe-economica-clientes-ACLScript/blob/master/04-prints/contracheque_001.JPG?raw=true)

> **Observação:** Nessa análise será usada o contracheque de 7 clientes, mas poderiam ser milhares ou até  milhões de contracheques em formato de PDF.

----------

### Resultado consolidado dos arquivos

![](https://github.com/Renatoelho/Analise-classe-economica-clientes-ACLScript/blob/master/04-prints/consolidado_contracheques.JPG?raw=true)

 >  **Observação:** Está sendo usado PDFs criados com o mesmo *layout*, mas isso deve variar bastante em relação a localização de determinados caracteres quando os arquivos forem criados por sistemas diferentes, nesse caso para evitar problemas é melhor extrair dados de um PDF usando expressões regulares que vai ser um projeto futuro publicado aqui no *GitHub*.

----------

### Resultado da análise da classe econômica

![](https://github.com/Renatoelho/Analise-classe-economica-clientes-ACLScript/blob/master/04-prints/classe_economica_clientes.JPG?raw=true)

----------