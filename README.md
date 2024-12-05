### Software usado: MySQL Workbench

### Componentes principais:
Peças/Cliente/veículo/Pagamento/Estoque/Equipe de mecânicos/Ordem de serviço/Fornecedor

### Relacionamentos:
- Cliente/Veiculo: Clientes pode possui mais de um veiculo.
- Veiculo/OS: Um veiculo pode ter mais de uma ordem de serviço associada.
- OS/Peça: Uma OS pode conter várias peças.
- OS/Serviço: Uma OS pode conter vários serviços.
- Peça/Estoque: O estoque pode conter várias peças e um produto pode conter em mais de um estoque e o mesmo gerencia a sua quantidade.
- Peça/Fornecedor: Uma peça pode conter vários fornecedores e um fornecedor pode fornecer mais de uma peça.
- Pagamento/Serviço: O pagamento está associado a execução do serviço.
- Cliente/Pagamento: Cada cliente pode efetuar mais de uma forma de pagamento.

### Fluxo do sistema:
- Clientes levam veículos à oficina mecânica para serem consertados ou para passarem por revisões  periódicas.
- Cada veículo é designado a uma equipe de mecânicos que identifica os serviços a serem executados e preenche uma OS com data de entrega.
- A partir da OS, calcula-se o valor de cada serviço, consultando-se uma tabela de referência de mão-de-obra
- O valor de cada peça também irá compor a OSO cliente autoriza a execução dos serviços
- A mesma equipe avalia e executa os serviços
- Os mecânicos possuem código, nome, endereço e especialidade
- Cada OS possui: n°, data de emissão, um valor, status e uma data para conclusão dos trabalhos.
  
### O esquema está disponível no formato de imagem abaixo:
![OS Oficina](https://github.com/user-attachments/assets/a45753f4-bc74-4837-8711-9ef80cb356df)
