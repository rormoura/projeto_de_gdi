# GERENCIAMENTO DE DADOS E INFORMAÇÃO

Professor: Robson Fidalgo

Alunos: 

Danilo Augusto Barbosa Nogueira (dabn@cin.ufpe.br)

Filipe Baptistella Vieira (fbv@cin.ufpe.br)

Rafael do Nascimento Moura (rnm4@cin.ufpe.br)

Rodrigo Rocha Moura (rrm2@cin.ufpe.br)

Recife, 02 de Março de 2022

## Minimundo

A ATP (Associação de Treinadores Pokémon) deseja construir um histórico sobre o mundo Pokémon, este servirá tanto para os Treinadores mais antigos que desejam guardar suas conquistas, assim como para aqueles que começaram a pouco tempo. Esse histórico terá como título “Passado, Presente e Futuro do mundo Pokémon” e guardará informações como o nome dos Treinadores, seus Pokémons capturados, os Itens utilizados durante as jornadas, dentre outras coisas.

* Treinadores têm nome_do_Treinador, sexo, ranking, é_líder e um TCN (trainer card number), este sendo o que os identifica.

* Pokémon tem o tipo_do_Pokémon, o qual pode ter mais de um valor, além disso também possui um P_status (sendo subdividido em P_ataque, P_defesa, P_velocidade e P_pontos_de_vida), uma habilidade e um identificador chamado id.

* Regiões possuem nome_da_Região e assinatura geológica, a qual é o atributo que identifica cada região.

*	Cada Cidade tem nome_da_Cidade, que discrimina uma cidade da outra e um bioma característico.

*	Itens têm um identificador chamado código de barras e nome_do_Item.

* Insígnia tem tipo_da_Insígnia e código_da_Insígnia, o qual identifica cada Insígnia presente no histórico.

*	Um Treinador pode capturar vários Pokémon enquanto um Pokémon só pode ser capturado por um Treinador. Para que seja cadastrado, um Treinador não precisa estar vinculado a um Pokémon assim como um Pokémon não precisa estar vinculado a um Treinador para ser cadastrado. São cadastradas essas informações porque o coração do mundo Pokémon é a captura destes por seus treinadores.

*	Um Treinador pode desafiar vários outros Treinadores e pode ser desafiado por muitos Treinadores. Um duelo entre dois Treinadores pode ocorrer mais de uma vez e é possível que envolva uma Insígnia caso um dos Treinadores seja líder de um ginásio. Além disso, a data do duelo deve ser anotada. Sabemos quem venceu determinado duelo a partir da entidade associativa venceu. Os duelos fazem parte do cotidiano dos treinadores Pokémon, tanto dos comuns como dos líderes de ginásio. 

*	Uma Região pode ter várias Cidades, mas uma Cidade só pode pertencer a uma Região. Regiões podem ser cadastradas sem estarem vinculadas a Cidades, mas uma Cidade precisa pertencer a uma Região para ser cadastrada.

*	Um Pokémon é originário de apenas uma Cidade e não pode ser cadastrado sem ser vinculado a essa Cidade, já uma Cidade pode ser a origem de vários Pokémon e pode ser cadastrada sem ser a origem de algum Pokémon.

*	Um Treinador pertence a apenas uma Cidade e não pode ser cadastrado sem ser vinculado a essa Cidade, entretanto, uma Cidade pode conter vários Treinadores e pode ser cadastrada sem conter nenhum Treinador.
    - As divisões geográficas e culturais (Cidades e Regiões) do mundo Pokémon são bastante valorizadas por seus moradores. 

*	Um Treinador pode comprar vários itens e um Item só pode ser comprado por um Treinador. Não é necessário que um Item seja comprado por um Treinador para que este seja cadastrado, assim como um Treinador não precisa possuir um Item para que este seja cadastrado. Existem itens de vários tipos e muitos deles têm características próprias:
    - Os itens de aprimoramento multiplicam um status específico do Pokémon (A_ataque, A_defesa, A_velocidade, A_pontos_de_vida) por X vezes; 
    - Os itens de movimento servem para ensinar um movimento a um Pokémon. Um Pokémon se relaciona com um item de movimento a partir do relacionamento aprende. Um Pokémon pode aprender mais de um movimento e um mesmo movimento pode ser ensinado a mais de um Pokémon. Não é necessário que um movimento seja aprendido por um Pokémon para que este seja cadastrado, assim como um Pokémon não precisa aprender um movimento para que este seja cadastrado.
* Existem itens que não se encaixam em nenhuma dessas classificações como a Pokébola.
    - Tornou-se costume dos Treinadores Pokémon a compra de Itens, pois são ferramentas úteis tanto para o treinador como para o Pokémon.

* Desse modo, podemos ver que o histórico passa pelos aspectos mais importantes do mundo Pokémon; abrangendo cultura, geografia, relações entre treinadores, relações treinadores-Pokémons e objetos essenciais como Itens e Insígnias.
