# Controles de Segurança

Os dados confidenciais devem ser protegidos com base no impacto potencial de uma perda de confidencialidade, integridade ou disponibilidade. As medidas de proteção (também conhecidas como ***controles de segurança*** ) tendem a se enquadrar em duas categorias. Primeiro, as deficiências de segurança do sistema precisam ser resolvidas. Por exemplo, se um sistema tem uma vulnerabilidade conhecida que pode ser explorada por invasores, o sistema deve ser corrigido para que a vulnerabilidade seja removida ou mitigada. Em segundo lugar, o sistema deve oferecer apenas a funcionalidade necessária para cada usuário autorizado, de forma que ninguém possa usar funções desnecessárias. Este princípio é conhecido como ***privilégio mínimo*** . Limitar a funcionalidade e resolver os pontos fracos de segurança têm um objetivo comum: dar aos invasores o mínimo de oportunidades possível de violar um sistema.

Existem três tipos de controles de segurança, como segue:

- **Controles de gestão:** os controles de segurança que se concentram na gestão de riscos e na gestão da segurança do sistema de informação.
- **Controles operacionais:** os controles de segurança que são principalmente implementados e executados por pessoas (em oposição aos sistemas).
- **Controles técnicos:** os controles de segurança que são principalmente implementados e executados pelo sistema por meio do hardware, software ou firmware do sistema.

Todos os três tipos de controles são necessários para uma segurança robusta. Por exemplo, uma política de segurança é um controle de gerenciamento, mas seus requisitos de segurança são implementados por pessoas (controles operacionais) e sistemas (controles técnicos). Pense em ataques de phishing. Uma organização pode ter uma política de uso aceitável que especifica a conduta dos usuários, incluindo não visitar sites maliciosos. Os controles de segurança para ajudar a impedir o phishing, além do controle de gerenciamento da própria política de uso aceitável, incluem controles operacionais, como treinamento de usuários para não cair em golpes de phishing e controles técnicos que monitoram e-mails e o uso do site em busca de sinais de atividade de phishing.

Um problema comum com os controles de segurança é que eles geralmente tornam os sistemas menos convenientes ou mais difíceis de usar. Quando a usabilidade é um problema, muitos usuários tentarão burlar os controles de segurança; por exemplo, se as senhas devem ser longas e complexas, os usuários podem anotá-las. Equilibrar segurança, funcionalidade e usabilidade costuma ser um desafio. O objetivo deve ser encontrar um equilíbrio adequado: fornecer uma solução razoavelmente segura, ao mesmo tempo que oferece a funcionalidade e a usabilidade que os usuários exigem.

Outro princípio fundamental dos controles de segurança é o uso de várias camadas de segurança - defesa em profundidade . Por exemplo, dados confidenciais em um servidor podem ser protegidos de ataques externos por vários controles, incluindo um firewall baseado em rede, um firewall baseado em host e patch de sistema operacional. A motivação para ter várias camadas é que, se uma camada falhar ou não puder neutralizar uma determinada ameaça, outras camadas podem impedir que a ameaça violar o sistema. Uma combinação de controles baseados em rede e baseados em host geralmente é mais eficaz para fornecer proteção consistente.

## Referência

[Security Controls - MDN](https://developer.mozilla.org/en-US/docs/Archive/Security/Controls)