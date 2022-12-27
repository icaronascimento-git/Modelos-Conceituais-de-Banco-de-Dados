OFICINA/NARRATIVA

- Sistema de controle e gerenciamento de execução de ordens de serviço em uma oficina mecânica
- Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões periódicas
- Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e
preenche uma OS com data de entrega.
- A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
- O valor de cada peça também irá compor a OS
- O cliente autoriza a execução dos serviços
- A mesma equipe avalia e executa os serviços
- Os mecânicos possuem código, nome, endereço e especialidade
- Cada OS possui: Nº, data de emissão, um valor, status e uma data para conclusão dos trabalhos.
- Uma OS pode ser composta por vários serviços e um mesmo serviço pode estar contido em mais de uma OS.
- Uma OS po ter vários tipos de peça e uma peça pode estar presente em mais de uma OS.


Entidade Cadastro:
- É necessário que os clientes e os mecânicos possuam cadastros, foi criado essa entidade e seus diversos atríbutos para atender essa necessidade.


Entidade Veículos:
- Nela contém os atributos básicos necessários para identificação do veículo.
- Ela possui relação de 1:1 com mecânicos, pois cada veículo será designado para uma equipe especifica.
- Já com clientes, a relação 1:n foi por entender que um mesmo cliente possa ter vários veículos na mesma oficina.


Entidade Ordem de Serviço:
- A entidade Ordem de serviço possuí uma dependência com a entidade serviços, poís para a OS ser emitida, é necessário antes a verficiação do que 
será necessário na manutenção do veículo.
- Ela tem uma relação de 1:1 com clientes, pois cada cliente terá apenas uma ordem de serviço, mesmo ele possuindo mais de um veículo na oficina.
- Ela possui relação de 1:1 com forma de pagamento, por entender que cada OS, será acordado uma única forma de pagamento.


Esse foi meu projeto conceitual para um Banco de Dados de uma oficina mecânica.