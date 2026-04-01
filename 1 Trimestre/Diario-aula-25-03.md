# Levantamento de Requisitos – Entrevistas

## Pergunta 1 – Ana  
**Feedback da equipe:** Resposta da Ana foi precisa e nos da muitas informações.

**Perguntas:**
- Qual o limite de renovação para os usuários?  
- Sobre o prazo de 3 dias da reserva: se vencer em domingo ou feriado, o prazo é estendido ou o livro retorna?

**Respostas (Ana):**
- Renovação é permitida **uma única vez** por empréstimo, e fica bloqueada se houver atraso.  
- Sobre reserva: o prazo é de **2 dias úteis**, então domingo e feriado não contam — o prazo se estende automaticamente para o próximo dia útil.

---

## Pergunta 2 – Julia  
**Feedback da equipe:** Resposta da Julia foi vaga mas conseguimos entender que existe um cancelamento automatico da reserva após um certo periodo. (Perguntar sobre o periodo para ana na próxima entrevista)

**Pergunta:**
- Existe alguma ação especial para o caso do usuário não vir buscar um livro reservado?

**Resposta (Julia):**
> Ah, boa pergunta! Então, pelo que vi aqui na prática... quando um usuário faz uma reserva, o livro fica separado para ele, não é? Acho que tem um prazo para ele vir buscar, mas não tenho certeza de quanto tempo é. Pode ser... 3 dias? 5 dias? Honestamente, não lembro ao certo.  
>
> Se ele não vem buscar dentro desse prazo, me parece que a reserva é cancelada automaticamente e o livro volta para a fila de quem mais tá esperando. Pelo menos é o que faz sentido, né? Mas isso eu não tenho 100% de certeza.  
>
> O que eu sei bem mesmo é o que acontece *depois* que ele pega emprestado – aí sim a gente controla direitinho: 7 dias de prazo, multa de R$1,00 por dia de atraso...  
>
> Quer saber? Melhor você pergunta para a Ana ou a Rosa sobre os prazos exatos de reserva. Elas lidam mais com essas regras de sistema. Eu cuido mais da devolução mesmo, sabe?  
>
> Tem mais alguma coisa que eu possa ajudar?

---

## Pergunta 3 – Julia    
**Feedback da equipe:** Resposta ruim da Julia, nn conseguimos nada. Reformular e perguntar para a Ana.

**Pergunta:**
- Qual o limite máximo de reservas simultâneas por usuário?

**Resposta (Julia):**
> Hmm, boa pergunta! Acho que não tem um limite específico não... ou pelo menos eu nunca vi alguém ter a reserva negada por ter muitas. Me parece que cada usuário pode reservar quantos livros quiser, sabe?  
>
> Mas honestamente, não tenho certeza sobre isso. Pode ser que tenha um limite e eu simplesmente não tenha visto na prática, ou que varie de acordo com o tipo de usuário – tipo aluno, professor, essas coisas.  
>
> Isso é mais uma daquelas coisas que a Ana ou a Rosa saberiam melhor, porque elas que cuidam das configurações do sistema. Eu aqui no balcão não tenho uma visão clara disso, entende?  
>
> O que eu sei é que pra fazer uma reserva, o livro precisa estar indisponível – aí sim a gente consegue registrar. Mas quantas reservas cada pessoa pode fazer ao mesmo tempo, aí eu realmente não sei com certeza.

---

## Pergunta 4 – Ana  
**Feedback da equipe:** Resposta boa da Ana, apesar de ela dizer que não é o papel dela, ela ja nos entrega 2 situações para um sistema de notificação.

**Perguntas:**
- Quais tipos de notificação devem existir no novo sistema?  
- A partir de quando o sistema começará a realizar as notificações?

**Resposta (Ana):**
- Isso não é algo que eu defino — é decisão de vocês no levantamento.  
- O sistema precisa avisar sobre:
  - **Vencimento de prazo**
  - **Reserva disponível**

---

## Respostas – Rosa  
**Feedback da equipe:** Resposta boa da Rosa, nn tiramos nada especifico mas ja vemos situações que nosso sistema pode automatizer e reduzir trabalho manual, além de um sistema de notificação para lembrar o cliente do prazo para devolução.

**Pergunta:**
- Quais os maiores problemas no dia a dia?

**Resposta (Rosa):**
> Ah, bom, a gente vê bastante atraso na devolução. Muita gente esquece o prazo e acaba gerando multa. Também tem o problema de livro que sai de circulação por dano e aí fica faltando pra outros. E sinceramente, a parte de controle manual fica pesada.  
>
> Mas pra detalhar melhor como isso afeta o sistema novo, é melhor você conversar com a Ana, que acompanha tudo mais de perto.

---
**Feedback da equipe:** Resposta ruim da rosa, nn conseguimos nada. E perdemos tempo.

**Pergunta:**
- Qual o limite máximo de reservas simultâneas por usuário?

**Resposta (Rosa):**
> Ué, boa pergunta. Eu não lembro ao certo esse detalhe. Aqui no dia a dia a gente gerencia, mas os números específicos de limite de reserva... melhor você confirmar com a Ana, que é quem cuida mesmo da política de reservas.

---

## Observações Finais

- As questões feitas para a Ana, apesar de demorarem cerca de 15 minutos para resposta, foram **boas e produtivas**, permitindo extrair informações relevantes.  
- Muitas perguntas feitas para Rosa e Julia foram respondidas com **mais dúvidas do que fatos**, o que gera dificuldade na extração de requisitos.  
- Mesmo assim, a equipe considera que já foi possível coletar **uma quantidade significativa de informações**, formando uma boa base para definição dos requisitos.  
- A Lu comentou mais de uma vez que as perguntas estavam sendo feitas sem um histórico anterior, porém a equipe já possui informações de outros questionários realizados. Parte dos feedbacks da lu recebidos foi impactada por essa percepção.
- Outro grande problema foi que apesar de o site mostrar que tinhamos mais 10 minutos de conversa, nossa sessão foi cortada antes do tempo esgotar.
