# O ecossistema Magnus

Voz, vídeo, operação e decisão são partes do mesmo problema: atender quem chega e liberar a entrada com segurança. Cada sistema Magnus resolve uma parte e conversa com as outras.

## Quem faz o quê

| Sistema | Responsabilidade | Conversa com |
| --- | --- | --- |
| [Magnus PBX](magnus-pbx.md) | Recebe a chamada do interfone, conduz o porteiro virtual e contata o morador. | ONE (entrega a chamada), Core (usa IA), VMS (traz a foto do portão) |
| [Magnus VMS](magnus-vms.md) | Mostra o portão ao vivo, lê placa e rosto e guarda a evidência. | ONE (abre câmeras), PBX (imagem para o porteiro), Core (análises) |
| [Magnus Core](magnus-core.md) | Interpreta, decide e redige com IA, escolhendo o modelo por cliente e tarefa. | Todos os sistemas |
| [Magnus ONE](magnus-one.md) | Console do operador: atende, confirma e libera, e registra a ocorrência. | PBX, VMS e Core |

## Uma visita, passo a passo

1. **O visitante chama no interfone.** A ligação chega ao Magnus PBX. O porteiro virtual atende em português, pergunta com quem o visitante quer falar e identifica a unidade.
2. **As câmeras abrem sozinhas.** O Magnus VMS mostra o portão ao vivo. Placa e rosto são lidos e comparados com o cadastro.
3. **A IA entende e decide.** O Magnus Core interpreta o que foi dito, confere se o visitante é esperado e define o caminho: liberar, consultar o morador ou chamar o operador.
4. **O morador autoriza.** Por ligação, ou por mensagem de WhatsApp com a foto do visitante e dois botões: autorizar ou negar. Sem aplicativo.
5. **O portão abre e tudo fica registrado.** No Magnus ONE o operador confirma e libera. A ocorrência é gravada com a evidência em vídeo e um rascunho de relatório escrito pela IA.

## Princípios de projeto

- **Humano no controle.** A IA sugere e organiza; o operador pode assumir a qualquer momento.
- **Cada sistema evolui sem quebrar os outros.** Integrações por interfaces definidas; provedores de IA trocáveis por configuração.
- **Isolamento por cliente** em toda consulta, chamada e relatório.
- **Adoção gradual.** É possível começar por um sistema e integrar os demais com o tempo.
