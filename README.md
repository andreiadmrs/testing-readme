# Tag audio, inserindo música e sons na página

Um elemento de áudio representa um som ou fluxo de áudio. O conteúdo pode ser fornecido dentro do elemento de áudio. Os agentes do usuário não devem mostrar esse conteúdo para o usuário; destina-se a navegadores da Web mais antigos que não suportam áudio, para que os plug-ins de áudio herdados possam ser tentados ou para mostrar texto aos usuários desses navegadores mais antigos, informando-os sobre como acessar o conteúdo de áudio.O elemento de áudio é um elemento de mídia cujos dados de mídia são ostensivamente dados de áudio. Os atributos src,preload, autoplay, mediagroup, loop, muted, e controls são os atributos comuns a todos os elementos de mídia.

- [X] **`<audio>`**
  - Display: none
  - Categoria: Fluxo, fraseado e incorporado
  - Contido por: Qualquer conteúdo
  - Filhos: depende se tem src
  - DOM interface
  - HTMLAudioElement new

## Atributos

- autoplay: Indica se audio vai tocr automaticamente ou não (verdadeiro ou falso)
- preload: tamanho da memoria que ele vai usar para buferizar o audio 
- controls: Exibe a barra de controles
- loop: Da loop no audio 
- mediagroup: informar qual midia de grupos o audio pertence
- muted: Cilenciar 
- src: link para o audio
