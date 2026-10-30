# Segurança e privacidade

Portaria não pode sair do ar nem expor quem entra e sai. Por isso estes pontos fazem parte do desenho dos sistemas, e não são opcionais.

## Isolamento entre clientes

Um mesmo sistema atende muitos clientes sem que um enxergue o outro, em cada consulta, chamada e relatório. No PBX e no VMS a organização multi-tenant é a base do modelo de dados.

## Controle dos dados

Gravações, fotos e registros de chamadas ficam sob controle de quem opera, com retenção configurável por cliente. Chaves de provedores de IA ficam apenas no [Magnus Core](magnus-core.md) e nunca são repassadas aos demais sistemas.

## Disponibilidade

O Magnus PBX tem alta disponibilidade com dois nós: se um falha, o reserva assume em cerca de 15 segundos. Para a conexão do próprio local, recomenda-se link redundante, avaliado na implantação.

## Segurança ativa na telefonia

Bloqueio automático de tentativas, bloqueio geográfico, monitor de ataques, listas de bloqueio e log de auditoria (Magnus Shield).

## Evidência íntegra

O Magnus VMS grava sem recompressão, com hash de integridade, e exporta evidência idêntica ao original. Eventos podem ser protegidos contra a retenção automática.

## IA com transparência

O consumo de cada tarefa de IA é medido por cliente e por tarefa. A IA sugere; decisões e ocorrências ficam registradas e o operador humano pode assumir.

## LGPD

O uso de câmeras e de reconhecimento facial é uma decisão do condomínio ou da empresa contratante, que define finalidade e retenção. A implantação inclui apoio para configurar apenas o necessário e documentar aviso e base legal. Recomenda-se validar o texto final com o jurídico de cada cliente.

## O que não é publicado

Código-fonte, configurações de rede, credenciais, topologias de clientes e dados operacionais permanecem fora deste repositório.
