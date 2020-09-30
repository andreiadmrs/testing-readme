# Vulnerabilidades

Uma vulnerabilidade é uma fraqueza em um sistema que pode ser explorada para impactar negativamente a confidencialidade, integridade e / ou disponibilidade. Existem muitas maneiras de categorizar as vulnerabilidades. Este artigo usa três categorias de vulnerabilidade de alto nível: falhas de software, problemas de configuração de segurança e uso indevido de recursos de software. Essas categorias são descritas a seguir.

## Categorias de vulnerabilidade

Uma ***vulnerabilidade de falha de software*** é causada por um erro não intencional no design ou codificação do software. Um exemplo é um erro de validação de entrada, como a entrada fornecida pelo usuário não sendo avaliada adequadamente para cadeias de caracteres maliciosas e valores excessivamente longos associados a ataques conhecidos. Outro exemplo é um erro de condição de corrida que permite que o invasor execute uma ação específica com privilégios elevados.

Uma definição de configuração de segurança é um elemento de segurança de um software que pode ser alterado pelo próprio software. Exemplos de configurações são um sistema operacional que oferece acesso a listas de controle que definem os privilégios que os usuários têm para arquivos e um aplicativo que oferece uma configuração para habilitar ou desabilitar a criptografia de dados confidenciais armazenados pelo aplicativo.

Uma ***vulnerabilidade de problema de configuração de segurança*** envolve o uso de configurações de segurança que afetam negativamente a segurança do software.

Um recurso de software é uma capacidade funcional fornecida pelo software. Uma ***vulnerabilidade de uso indevido de recurso de software*** é uma vulnerabilidade em que o recurso também fornece uma via para comprometer a segurança de um sistema. Essas vulnerabilidades são causadas pelo designer do software que faz suposições de confiança que permitem que o software forneça recursos benéficos, ao mesmo tempo que introduz a possibilidade de alguém violar as suposições de confiança para comprometer a segurança.

Por exemplo, o software cliente de email pode conter um recurso que processa conteúdo HTML em mensagens de email. Um invasor pode criar uma mensagem de email fraudulenta que contenha hiperlinks que, quando processados ​​em HTML, parecem ao destinatário ser benignos, mas na verdade levam o destinatário a um site mal-intencionado quando são clicados. Uma das suposições de confiança no design do recurso de renderização de conteúdo HTML era que os usuários não receberiam hiperlinks mal-intencionados e clicariam neles.

Vulnerabilidades de uso indevido de recursos de software são introduzidas durante o design do software ou um componente do software (por exemplo, um protocolo que o software implementa). As suposições de confiança podem ter sido explícitas - por exemplo, um designer estando ciente de uma falha de segurança e determinando que um controle de segurança separado compensaria por isso.

No entanto, as suposições de confiança costumam estar implícitas, como criar um recurso sem primeiro avaliar os riscos que ele apresentaria. As ameaças também podem mudar ao longo da vida útil do software ou protocolo usado no software.

Por exemplo, o protocolo ARP (Address Resolution Protocol) confia que uma resposta ARP contenha o mapeamento correto entre os endereços Media Access Control (MAC) e Internet Protocol (IP). O cache ARP usa essas informações para fornecer um serviço útil - para permitir o envio de dados entre dispositivos em uma rede local. No entanto, um invasor pode gerar mensagens ARP falsas para envenenar a tabela ARP de um sistema e, assim, lançar um ataque de negação de serviço ou man-in-the-middle.

O protocolo ARP foi padronizado há mais de 25 anos e as ameaças mudaram muito desde então, portanto, as suposições de confiança inerentes ao seu projeto provavelmente ainda não serão razoáveis ​​hoje.

Pode ser difícil diferenciar as vulnerabilidades de uso indevido de recursos de software das outras duas categorias. Por exemplo, as falhas de software e as vulnerabilidades de uso indevido podem ser causadas por deficiências nos processos de design de software. No entanto, as falhas de software são puramente negativas - elas não fornecem nenhum benefício positivo para a segurança ou funcionalidade - enquanto vulnerabilidades de uso indevido de recursos de software ocorrem como resultado do fornecimento de recursos adicionais.

Também pode haver confusão em relação às vulnerabilidades de uso indevido de recursos que podem ser ativados ou desativados - de certa forma, configurados - versus problemas de configuração de segurança. A principal diferença é que, para uma vulnerabilidade de uso indevido, a definição de configuração ativa ou desativa o recurso inteiro e não altera especificamente apenas sua segurança; para uma vulnerabilidade de problema de configuração de segurança, a definição de configuração altera apenas a segurança do software.

Por exemplo, uma configuração que desabilita todo o uso de HTML em emails tem um impacto significativo na segurança e na funcionalidade, portanto, uma vulnerabilidade relacionada a esta configuração seria uma vulnerabilidade de uso indevido. Uma configuração que desabilita o uso de um recurso antiphishing em um cliente de email tem um impacto significativo apenas na segurança, portanto, uma vulnerabilidade com essa configuração seria considerada uma vulnerabilidade de problema de configuração de segurança.

## A presença de vulnerabilidades

Nenhum sistema é 100% seguro: todo sistema possui vulnerabilidades. A qualquer momento, um sistema pode não ter nenhuma falha de software conhecida, mas problemas de configuração de segurança e vulnerabilidades de uso indevido de recursos de software estão sempre presentes.

As vulnerabilidades de uso indevido são inerentes aos recursos do software porque cada recurso deve ser baseado em suposições de confiança - e essas suposições podem ser quebradas, embora envolvam custos e esforços significativos em alguns casos. Os problemas de configuração de segurança também são inevitáveis ​​por dois motivos.

Em primeiro lugar, muitas definições de configuração aumentam a segurança às custas de reduzir a funcionalidade, portanto, usar as configurações mais seguras pode tornar o software inútil ou inutilizável. Em segundo lugar, muitas configurações de segurança têm consequências positivas e negativas para a segurança.

Um exemplo é o número de tentativas consecutivas de autenticação com falha permitidas antes de bloquear uma conta de usuário. Definir como 1 seria a configuração mais segura contra ataques de adivinhação de senha, mas também faria com que usuários legítimos fossem bloqueados após digitar uma senha incorretamente uma vez e também permitiria que invasores executassem ataques de negação de serviço contra usuários mais facilmente gerando uma única tentativa de login com falha para cada conta de usuário.

Por causa do número de vulnerabilidades inerentes às configurações de segurança e possibilidades de uso indevido de recursos de software, além do número de vulnerabilidades de falhas de software em um sistema a qualquer momento, pode haver dezenas ou centenas de vulnerabilidades em um único sistema.

Essas vulnerabilidades provavelmente têm uma ampla variedade de características. Alguns serão muito fáceis de explorar, enquanto outros só serão exploráveis ​​sob uma combinação de condições altamente improváveis.

Uma vulnerabilidade pode fornecer acesso de nível raiz a um sistema, enquanto outra vulnerabilidade pode permitir apenas acesso de leitura a um arquivo insignificante.

Em última análise, as organizações precisam saber o quão difícil é para alguém explorar cada vulnerabilidade e, se uma vulnerabilidade for explorada, qual seria o possível impacto.

## Vulnerabilidades de sites

OWASP ou Open Web Security Project é uma organização de caridade sem fins lucrativos focada em melhorar a segurança de software e aplicativos da web. De acordo com o Open Web Application Security Project, o XSS foi a sétima vulnerabilidade de aplicativo da Web mais comum em 2017.

A organização publica uma lista das principais vulnerabilidades de segurança da web com base nos dados de várias organizações de segurança.

As vulnerabilidades de segurança da web são priorizadas dependendo da capacidade de exploração, detectabilidade e impacto no software, que pode ser qualquer CMS, como WordPress, Joomla, Magento, Wocommerce e muito mais.

Aqui estão seis das vulnerabilidades mais comuns de sites contra as quais você deve se proteger.

- Injeções de SQL
- Cross Site Scripting (XSS)
- Broken Authentication & Session Management - IdentityManager
- Insegure Direct Object References - DOM (Document Object Model)
- Configuração incorreta de segurança
- Cross-Site Request Forgery (CSRF)

## Referências

[Vulnerabilities - MDN](https://developer.mozilla.org/en-US/docs/Archive/Security/Vulnerabilities)
