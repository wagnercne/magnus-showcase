# Magnus Core

O Magnus Core é a camada central de serviços compartilhados para os produtos Magnus. Ele organiza o uso de recursos de IA por organização e tarefa, mantendo a integração com provedores desacoplada das aplicações que consomem o serviço.

## Papel na plataforma

- Identifica o contexto da organização e do serviço solicitado.
- Encaminha chamadas para provedores por uma camada de drivers.
- Permite evolução dos provedores sem espalhar integrações pela plataforma.
- Dá base para recursos de voz, texto e automação assistida nos produtos que necessitam deles.

## Critérios de avaliação

Uma avaliação técnica pode abordar o isolamento por organização, a rastreabilidade das solicitações, a integração com os sistemas Magnus e as opções de provedores compatíveis com a política de cada operação.

## Limites do material público

Parâmetros de provedores, chaves de acesso, políticas específicas de cada cliente, dados processados e detalhes de implantação não são divulgados.
