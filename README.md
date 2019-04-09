# tech-test-naval-battle

Você **não poderá usar bibliotecas externas** ou ferramentas para propósito de criação ou teste. Especificamente, você poderá usar bibliotecas de testes unitários ou ferramentas de build disponíveis para a linguagem que você escolher (por exemplo, Nunit, MSTest, etc).

**Precisaremos rodar e compilar o seu código**. Por favor encaminhe uma breve descrição do design e suposições junto com o seu código, bem como as instruções detalhadas de como rodar sua aplicação.

Não é necessário que você trabalhe nos mínimos detalhes da solução, porém estaremos procurando algo mais que somente o esqueleto do código.

O programa deve ser escrito usando o desenvolvimento orientado a testes, seguindo as etapas de refatoração vermelhas e verdes.
Não sacrifique TDD para completar a solução, isso resultará em uma falha.
Avaliaremos uma variedade de aspectos, como design da solução, SOLID e orientação a objeto. Mesmo que estes problemas não sejam extensos, nós esperamos que você encaminhe um código que acredite ser de qualidade, um código possível de ser rodado e evoluído.

## Introdução:
 - A aplicação deve executar
 - Realize um fork do projeto
 - Adicione @pottencial (Pottencial Seguradora) como membro do seu fork. Você pode fazer isto em  https://gitlab.com/`your-user`/tech-test-naval-battle/settings/members
 - Quando você começar, faça um commit vazio com a mensagem "Iniciando o teste de tecnologia" e quando terminar, faça o commit com uma mensagem "Finalizado o teste de tecnologia".
 - Commit após cada ciclo de refatoração pelo menos.
 - Não use branches.
 - Tente não gastar mais de 3 horas para concluir o teste técnico.

## Problema
Cada jogador deve dispor de uma área de 10x10 onde ele vai posicionar 5 navios de tamanhos diferentes: um porta-aviões (comprimento 5), um encouraçado (comprimento 4), um submarino e um destroyer (ambom de comprimento 3), e barco de patrulha (comprimento 2). Um jogador nunca deve saber a posição dos navios do oponente. Os navios de um mesmo jogador não podem se cruzar e devem estar dentro das fronteiras da sua área disponível.

Depois que todas as peças estão posicionadas, os jogadores se alternam em turnos para lançar bombas sobre o outro oponente especificando qual posição ele deseja atacar. Se algum dos navios do jogador que está sendo atacado estiver na posição atacada, considera-se que o navio foi atingido. O ataque falha se o atacante lançar uma bomba em um local onde não existe nenhum navio do oponente.

Caso todos as posições de um navio for atingida, o jogador atacado deve informar o oponente qual dos seus navios afundou. O jogo continua até que um jogador afunde todos os navios de seu oponente; este jogador é então considerado vencedor.

Você deve desenvolver um programa que jogue uma partida de batalha naval entre dois oponentes. Você precisa:

- Definir uma maneira de indicar o estado inicial dos navios dos jogadores;
- Exibir todos os movimentos dos jogadores, informando se os ataques foram bem sucedidos ou não;
- Informar quando um navio é atingido e quando ele é afundado;
- Exibir ao final do jogo um mapa final do posicionamento final dos navios dos jogadores.