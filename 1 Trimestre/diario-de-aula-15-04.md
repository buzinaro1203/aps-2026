# Reserva
**História de usuário**
1. Como usuário logado da biblioteca (aluno/professor/funcionário)
Quero reservar livros que se encontram emprestados no momento
Para que eu entre na fila daquele título e seja notificado quando ele estiver disponível.

2. Como usuário logado da biblioteca (aluno/professor/funcionário)
Quero poder cancelar uma reserva efetuada
Para que eu possa liberar o item para outros usuários.

## Cenários

1. Dado que o usuário logado possui multas ou pendências ativas
Quando ele tentar solicitar a reserva de um livro
Então o sistema deve bloquear a solicitação e exibir um alerta para regularização.

2. Dado que o exemplar buscado está com status de "danificado" ou "perdido"
Quando o sistema processar a solicitação de reserva
Então a operação deve ser negada e o sistema deve informar que o exemplar está fora de circulação.

3. Dado que um livro reservado se tornou disponível
Quando se passarem 3 dias úteis sem que o usuário faça a retirada
Então o sistema deve cancelar a reserva automaticamente e passar a vez para o próximo da fila.

4. Dado que o limite total de itens do usuário é 3 e o usuário já possui 1 livro emprestado e 2 reservas ativas
Quando ele tentar realizar uma nova reserva
Então o sistema deve impedir a reserva informando que o limite total de movimentações foi atingido.

5. Dado que um livro possui uma fila de reserva com 2 Alunos
Quando um Professor solicitar a reserva deste mesmo livro
Então o Professor deve ser posicionado no topo da fila.

6. Dado que um aluno tenha uma reserva de um livro emprestado por um professor
Quando o professor realizar a renovação do livro
Então a reserva do aluno deve ser mantida e o sistema deve informar o aluno sobre o novo prazo devido à prioridade do professor.

7. Dado que um livro esteja disponível para empréstimo (quantidade > 0)
Quando o usuário solicitar a reserva do livro
Então o sistema deve informar que o livro está disponível e que ele deve realizar o empréstimo em vez da reserva.

8. Dado que um título possua vários exemplares no acervo
Quando qualquer um dos exemplares desse título for devolvido
Então o sistema deve notificar o primeiro usuário da fila de que o título já está disponível para retirada.



# Empréstimo
**História de usuário**
Como usuário logado (aluno/professor/funcionário)
Quero realizar o empréstimo de um exemplar disponível
Para que eu possa utilizar o material para meus estudos ou trabalho por um período determinado.

## Cenários

1. Dado que o sistema possui um limite total de 3 itens por usuário (Empréstimos + Reservas)
E o usuário já possui 2 livros emprestados e 1 reserva ativa
Quando ele tentar realizar um novo empréstimo
Então o sistema deve bloquear a operação e informar que o limite total de movimentações foi atingido.

2. Dado que o usuário não possui pendências e está dentro do limite de 3 itens
Quando ele realizar um empréstimo com sucesso
Então o sistema deve calcular a data de devolução prevista com base no perfil do usuário (ex: Aluno = 7 dias) a partir da data atual.

3. Dado que o usuário possui uma multa em aberto ou um livro em atraso
Quando ele tentar realizar um novo empréstimo
Então o sistema deve impedir a transação e solicitar a regularização da pendência.

4. Dado que o usuário deseja renovar um empréstimo
Quando não houver reserva de outros usuários para aquele título
Então o sistema deve permitir a renovação (limitado a uma única renovação).

5. Dado que um Professor deseja renovar um empréstimo
Quando houver uma reserva ativa de outro usuário para o mesmo título
Então o sistema deve permitir a renovação, ignorando a reserva.

6. Dado que um exemplar possui o status de referência
Quando o usuário tentar solicitar o empréstimo deste livro
Então o sistema deve bloquear a operação e informar que o material não pode ser emprestado.

7. Dado que a data de devolução prevista de um empréstimo caia em um sábado, domingo ou feriado
Quando o prazo estiver acabando
Então o prazo deve ser estendido automaticamente para o primeiro dia útil seguinte.

8. Dado que o usuário realize a devolução de um exemplar em bom estado
Quando o operador confirmar o recebimento
Então o sistema deve liberar o limite do usuário e disponibilizar o exemplar para novos empréstimos ou reservas.


