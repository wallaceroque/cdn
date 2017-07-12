# CDN - Content Distribution or Delivery Network

Com o crescimento de aplicações web, cresceram de forma vertiginosa a adoção de frameworks para aprimorar a usabilidade do usuário e promover o reuso para os desenvolvedores cansados de resolver sempre os mesmos problemas. Com isso, cresceram o uso de frameworks como AngularJS, React, Bootstrap etc. Uma simples aplicação single page pode ter um tamanho considerável utilizando todos esses frameworks além de seus próprios dados. A distribuição desse conteúdo de forma eficiente é desejável.

O CDN é um recurso para entrega de artefatos estáticos de forma distribuída. Ele pode ser utilizado no contexto de streaming, servindo conteúdos web como css, html, js e imagens ou qualquer outro tipo de conteúdo estático, de forma distribuída, visando ganho principalmente de performance e segurança.

O objetivo do CDN é servir o conteúdo de um ponto de origem mais próximo possível do solicitante, ou seja, utilizando menos saltos de rede, e de forma eficiente. Apesar da idéia ser simples, ela implica em diversos serviços de infraestrutura que podem se tornar gargalos e/ou pontos de falha que devem ser considerados em toda a arquitetura.

Servir eficientemente artefatos estáticos é algo realizado comumente na internet. No caso de conteúdo web, os servidores HTTP cumprem esse papel. O mais famoso deles é o Apache que perdeu espaço para outros como Nginx e Gwan, mais eficientes nesse quesito e que, somados às estratégias de cache, podem se obter ganhos consideráveis de performance no carregamento de páginas html, por exemplo.

Para alcançar uma solução de CDN eficiente e minimamente robusta, os seguintes desafios devem ser respondidos:

- Como será a infraestrutura de entrega de conteúdo ? 
- Qual a estratégia de balanceamento de carga?
- Qual é a estratégia do mecanismo de redirecionamento de requisição, responsável por redirecionar o cliente para o servidor de réplica mais apropriado ? (DNS Global)
- Qual é a estratégia distribuição de conteúdo, responsável pela distribuição do servidor de origem para os servidores de réplica e manter os servidores de réplica atualizados ?
- Quantos servidores de réplica utilizar e onde os mesmos devem estar localizados ?
- Administração e gerenciamento dos conteúdos
- Qual a solução de backup ?
- Qual a solução de monitoramento ?




