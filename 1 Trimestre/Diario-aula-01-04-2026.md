# Perguntas planejadas

Aqui está todas as perguntas que planejamos, algumas não deu tempo de fazer.
Para elaborar essas perguntas, cruzamos as informações de todos os questionarios até o momento.


Pergunta 1: Ana pelo que foi falado pela Julia na última entrevista, existe um prazo para virem buscar o livro após uma reserva e após isso um cancelamento automático da reserva. Qual a duração desse prazo? prioridade alta

Pergunta 2: Ana, quando é feita uma reserva, quais são os dados solicitados do usuário?

Pergunta 3: Ana, para evitar conflitos de um usuário reservar minutos livros, saberia me dizer quantas reservas um aluno pode realizar simultaneamente? Existe um limite diferente para professores?

Pergunta 4: Rosa,sobre o sistema de reservas, o que acontece quando 2 alunos tentam reservar um mesmo livro? (prioridade baixa)

Pergunta 5: Ana, acredito que seja importante o sistema ofertar ajuda às pessoas com deficiências, o que você acha de incluir recursos de acessibilidade? Como filtro de cores para daltonismo, letras maiores para pessoas com baixa visão, e outras.

Pergunta 6: Ana, sobre as multas, foi dito para nós que o valor é 1 real por dia, fins de semana contam também ou apenas dias úteis??

Pergunta 7: Ana, quando um livro for danificado, qual a ação que o sistema deve tomar para lidar com essa situação? e quando for perdido?

Pergunta 8: Ana, o cliente pode pagar a multa pelo pix ou cartão apenas no balcão ou pode fazer de forma remota pelo website por exemplo?

Pergunta 9: Ana, qual é o valor exato ou a regra de cálculo (cobrança adicional) gerada no sistema quando um livro é devolvido com danos?

Pergunta 10: Julia, a Ana falou que a multa pode ser paga em dinheiro pix ou cartão, como é o procedimento para os pagamentos de multa via pix ou cartão?








# Perguntas e Respostas Executadas — Sistema de Biblioteca

---

## Pergunta 1
Pergunta 1: Ana pelo que foi falado pela Julia na última entrevista, existe um prazo para virem buscar o livro após uma reserva e após isso um cancelamento automático da reserva. Qual a duração desse prazo? prioridade alta

Resposta 1:

Ana: Sim, existe esse prazo. Após a notificação de que o livro está disponível para retirada, o usuário tem 3 dias úteis para buscá-lo. Se não retirar dentro desse prazo, a reserva é cancelada automaticamente pelo sistema.

Rosa: Só complementando: esse cancelamento automático é importante para não deixar o exemplar parado na prateleira de reservas sem necessidade. É um ponto que aparece bastante no operacional do dia a dia.

Julia: Isso mesmo! E quando a reserva cai, o livro volta a ficar disponível normalmente para outros usuários. Ah, e a notificação ao usuário sobre a disponibilidade do livro — ela dispara na hora que o exemplar é devolvido ou processado, certo Ana?

Ana: Sim, a notificação dispara no momento em que o livro fica disponível para retirada. O prazo de 3 dias úteis começa a contar a partir daí.

---

## Pergunta 2
Pergunta 2: Ana, quando é feita uma reserva, quais são os dados solicitados do usuário?

Resposta 2:

Ana: Para registrar uma reserva, o sistema precisa identificar o usuário e o item. Então os dados básicos são: identificação do usuário — geralmente matrícula ou CPF — e o exemplar ou título que está sendo reservado. A data da solicitação é gerada automaticamente pelo sistema.

Rosa: Vale lembrar que o usuário já precisa estar cadastrado para fazer a reserva. Não é um cadastro feito na hora — é uma vinculação ao registro que já existe no sistema.

Julia: Exato! E normalmente o operador só confirma quem é o usuário e qual o título. O resto o sistema puxa sozinho, como o nome completo e o contato para a notificação.

---

## Pergunta 6
Pergunta 6: Ana, sobre as multas, foi dito para nós que o valor é 1 real por dia, fins de semana contam também ou apenas dias úteis??

Resposta 6:

Ana: O valor de R$ 1,00 por dia está correto. E para fechar: a contagem é em dias úteis, não corridos. Fins de semana não entram na conta.

Rosa: Bom lembrar também que recesso não suspende a multa — pelo menos é assim que funciona no operacional. Se o prazo venceu antes do recesso, a multa continua acumulando normalmente.

Julia: Rosa, vou corrigir esse ponto: recesso não suspende a contagem. A multa segue acumulando em dias úteis independentemente de recesso. Isso vale registrar direto como regra no sistema.

---

## Pergunta 7
Pergunta 7: Ana, quando um livro for danificado, qual a ação que o sistema deve tomar para lidar com essa situação? e quando for perdido?

Resposta 7:

Ana: São dois cenários distintos, mas ambos exigem ação no sistema. Para o livro danificado: o operador precisa registrar a ocorrência, o exemplar sai de circulação e fica com status de indisponível até que seja avaliado. O que acontece depois disso depende do grau do dano — se é reparável ou não. Para o livro perdido: o sistema precisa registrar a perda vinculada ao usuário responsável, bloquear novas movimentações desse exemplar e gerar o registro de responsabilidade. Em ambos os casos, o ponto central é que o exemplar não pode simplesmente sumir do sistema — precisa ter rastreabilidade do que aconteceu com ele.

Rosa: No operacional, o que aparece bastante é a dúvida de quando o operador pode agir sozinho e quando precisa de aval. Para danificado, normalmente o operador registra a ocorrência e tira de circulação, mas a decisão final sobre o destino do exemplar costuma ser de outro nível. Para perdido, o vínculo com o usuário é essencial — sem isso o sistema não consegue controlar responsabilidade nem cobrar nada.

Julia: Só para complementar: no caso de perda, o usuário fica bloqueado para novas retiradas enquanto a situação não for resolvida, né? Tipo, o sistema trava o perfil dele até ele regularizar. E no danificado, se o livro for considerado irrecuperável, aí o caminho seria diferente de um que só precisa de reparo... Mas aí já entraria em outra etapa do fluxo, imagino.

Ana: Julia, o bloqueio por perda não registrada é correto — o usuário com pendência ativa não pode retirar novos itens. Sobre o exemplar danificado irrecuperável: isso envolve outro procedimento, mas não vou entrar nesse detalhe agora porque é uma etapa separada no fluxo. Se quiserem fechar esse ponto, vale perguntar de forma direta e específica.

---

## Pergunta 8
Pergunta 8: Ana, o cliente pode pagar a multa pelo pix ou cartão apenas no balcão ou pode fazer de forma remota pelo website por exemplo?

Resposta 8:

Ana: Boa pergunta, mas ela toca num ponto que precisa de definição de vocês, não minha. O que posso fechar é o seguinte: o sistema precisa registrar o pagamento da multa e vinculá-lo ao usuário e ao exemplar correspondente, independentemente do canal. Se o pagamento for aceito apenas no balcão, o operador registra manualmente. Se houver canal remoto — site, aplicativo, o que for — o sistema precisa capturar esse evento e atualizar o status automaticamente. O que não pode acontecer é o pagamento ocorrer fora do sistema e o registro não refletir isso. Canal é decisão de vocês. Rastreabilidade é requisito.

Rosa: No operacional do dia a dia, o que aparece com mais frequência é o pagamento presencial mesmo — o usuário chega no balcão, paga, o operador baixa a pendência. Canal remoto existe em alguns sistemas, mas aí o fluxo muda bastante: quem confirma o pagamento? O sistema aguarda confirmação automática do gateway ou depende de ação manual do operador? Isso precisa estar definido antes de qualquer decisão sobre o canal.

Julia: Faz sentido pensar no remoto, especialmente se o usuário estiver com pendência e não puder retirar nada até regularizar. Se ele puder resolver pelo site, resolve mais rápido e o sistema atualiza na hora. Mas aí o sistema teria que se comunicar com alguma solução de pagamento externo, né? Tipo um gateway de Pix ou cartão. Isso é algo que vocês já têm mapeado como integração necessária?



