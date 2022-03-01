# GERENCIAMENTO DE DADOS E INFORMAÇÃO

Professor: Robson Fidalgo
Alunos: 

Danilo Augusto Barbosa Nogueira (dabn@cin.ufpe.br)

Filipe Baptistella Vieira (fbv@cin.ufpe.br)

Rafael do Nascimento Moura (rnm4@cin.ufpe.br)

Rodrigo Rocha Moura (rrm2@cin.ufpe.br)

Recife, 02 de Março de 2022

## Minimundo

Uma federação de treinadores quer armazenar de maneira estruturada as informações referentes ao seu contexto.

* Treinadores têm nome, sexo, ranking, é_líder e um TCN (trainer card number), este sendo o que os identifica.

* Pokémon tem um tipo, o qual pode ter mais de um valor, além disso também possui um status (sendo subdividido em ataque, defesa e velocidade), uma habilidade e um identificador chamado id.

* Regiões possuem um nome e uma assinatura geológica, a qual é o atributo que identifica cada região.

*	Cada Cidade tem um nome, que discrimina uma cidade da outra e um bioma característico.

*	Itens têm um identificador chamado código de barras e um nome.

*	Um Treinador pode capturar vários Pokémon enquanto um Pokémon só pode ser capturado por um Treinador. Para que seja cadastrado, um Treinador não precisa estar vinculado a um Pokémon assim como um Pokémon não precisa estar vinculado a um Treinador para ser cadastrado.

*	Um Treinador pode liderar apenas um Ginásio, assim como um Ginásio só pode ser liderado por um Treinador. É possível cadastrar um Treinador sem ele estar vinculado a um Ginásio, mas não é possível cadastrar um Ginásio sem estar vinculado a um Treinador.

*	Um Treinador pode desafiar vários outros Treinadores e pode ser desafiado por muitos Treinadores. Um duelo entre dois Treinadores pode ocorrer mais de uma vez e é possível que envolva uma insígnia (item) caso um dos Treinadores seja líder de um ginásio. Além disso, a data do duelo deve ser anotada para formação de um histórico.

*	Uma Região pode possuir várias Cidades, mas uma Cidade só pode pertencer a uma Região. Regiões podem ser cadastradas sem estarem vinculadas a Cidades, mas uma Cidade precisa pertencer a uma Região para ser cadastrada.

*	Um Pokémon é originário de apenas uma Cidade e não pode ser cadastrado sem ser vinculado a essa Cidade, já uma Cidade pode ser a origem de vários Pokémon e pode ser cadastrada sem ser a origem de algum Pokémon.

*	Um Treinador pertence a apenas uma Cidade e não pode ser cadastrado sem ser vinculado a essa Cidade, entretanto, uma Cidade pode conter vários Treinadores e pode ser cadastrada sem conter nenhum Treinador.

*	Um Treinador pode comprar vários itens e um Item pode comprado por vários Treinadores. Não é necessário que um Item seja comprado por um Treinador para que este seja cadastrado, assim como um Treinador não precisa possuir um Item para que este seja cadastrado. Existem itens de vários tipos e muitos deles têm características próprias:
  - Os itens de recuperação trazem de volta os pontos de vida do Pokémon; 
  -	Os itens de aprimoramento multiplicam um status específico do Pokémon (ataque, defesa, velocidade etc.) por X vezes; 
  -	Os itens de estado curam um estado específico de um Pokémon (envenenamento, paralização, congelamento etc.); 
  -	Os itens de movimento servem para ensinar um movimento a um Pokémon. 
*	Existem itens que não se encaixam em nenhuma dessas classificações como a Pokébola, além de que alguns itens podem estar em mais de uma categoria.
