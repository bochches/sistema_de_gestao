# Canvas do Projeto

**Projeto:** Aplicativo de Gestão para Transporte Alternativo · **Equipe:** Thayná Fortunato, Wendrieley Clara, Carolaine Silva· **Data:** 15/09/2026 · **Organização parceira:** Loja de açaí

---

## 1. Problema

A loja de açaí recebe pedidos de clientes principalmente de forma manual, por atendimento presencial e aplicativos de mensagens, o que pode causar desorganização no registro dos pedidos, demora no atendimento, erros na montagem dos produtos e dificuldade para acompanhar o estoque de ingredientes e complementos.

**Evidências de que o problema existe** (dados, falas, observação):

-Pedidos são registrados manualmente ou por mensagens.
- Há possibilidade de perda ou confusão entre pedidos.
- O cliente pode ter dificuldade para saber o andamento do pedido.
- O controle de estoque de açaí, frutas e complementos pode ser feito manualmente.
- A organização dos pedidos durante horários de maior movimento pode se tornar mais difícil.
## 2. Quem é afetado

| Quem | Quantas pessoas | Como é afetado hoje |
| ---- | --------------- | -------------------- |
| Clientes|A definir pela loja|Podem enfrentar demora, erros ou falta de informações sobre o pedido|
| Funcionários |A definir| Precisam organizar pedidos manualmente e acompanhar sua produção |
| Entregadores | A definir| Podem ter dificuldade para identificar e organizar pedidos para entrega|
| Proprietário/Gerente |1 ou mais |Tem dificuldade para acompanhar pedidos, estoque e funcionamento da loja |

## 3. Solução proposta

Um aplicativo de gestão para a loja de açaí que permita cadastrar produtos e complementos, registrar pedidos, acompanhar o status dos pedidos e controlar o estoque.
O sistema permitirá que os funcionários tenham uma visão organizada dos pedidos em andamento, enquanto o administrador poderá acompanhar as vendas e o estoque da loja.
Em uma etapa futura, o sistema poderá permitir que o próprio cliente realize o pedido pelo aplicativo

## 4. Funcionalidades do MVP (3 a 5)

| # | Funcionalidade | Para quem | Por que é essencial |
| --- | -------------- | --------- | -------------------- |
| 1 | Cadastrar e gerenciar produtos | Admin |Permite manter o cardápio atualizado |
| 2 | Registrar pedidos |Funcionário | Centraliza os pedidos e reduz erros |
| 3 | Alterar status do pedido |Funcionário |Permite acompanhar preparação e conclusão |
| 4 | Controlar estoque de ingredientes e complementos |Admin | Evita falta de produtos e facilita o controle |
| 5 | Visualizar pedidos e vendas | Admin | Permite acompanhar o funcionamento da lojasistema |

## 5. Fora do escopo

O que **não** faremos nesta versão, e por quê:

| Não faremos | Por quê |
| ----------- | ------- |
| Programa de fidelidade | Não é essencial para o primeiro MVP |
| Integração com iFood/WhatsApp| A integração pode ser adicionada posteriormente |
| Pagamento online dentro do aplicativo | O MVP terá foco na gestão dos pedidos|
| Sistema avançado de contabilidade | Não faz parte do objetivo inicial| 
| Aplicativo completo para clientes no primeiro sprint |O primeiro sprint priorizará a gestão interna da loja |

## 6. Usuários e papéis

| Papel | O que pode fazer |
| ----- | ------------------ |
| Administrador/Gerente | Cadastra produtos, gerencia estoque, acompanha pedidos e visualiza vendas|
| Funcionário | Registra pedidos, consulta pedidos e altera o status de preparação |
| Entregador | Visualiza pedidos destinados à entrega e atualiza o status da entrega |
| Cliente    | Consulta produtos e, futuramente, poderá realizar pedidos pelo aplicativo|

## 7. Restrições

| Tipo            | Restrição                                                  |
| --------------- | ----------------------------------------------------------- |
| Prazo           | 18 a 22 semanas, divididas entre planejamento, back-end, front-end, testes/QA e implantação |
| Equipe          | 5 pessoas, 20 a 25 h/semana no total |
| Técnica         |Flutter/Dart para aplicativo, Node.js ou Firebase Cloud Functions, Cloud Firestore/NoSQL   |
| Contexto de uso | O sistema será utilizado principalmente durante o atendimento e preparação dos pedidos|
| Conectividade   | Deve funcionar adequadamente mesmo em situações de instabilidade de internet
| Orçamento       |R$ 59.000,00, considerando desenvolvimento, implantação e treinamento em 5 unidades |

## 8. Riscos principais

| Risco | O que faremos |
| ----- | -------------- |
| Instabilidade da internet | Utilizar armazenamento local e sincronização quando a conexão retornar |
| Funcionários terem dificuldade para utilizar o sistema | Criar uma interface simples, com botões grandes e fluxo de pedido fácil de entender |
| Erros no controle de estoque | Registrar automaticamente a saída dos ingredientes conforme os pedidos |
| Grande quantidade de pedidos em horários de pico | Utilizar uma tela organizada por status: recebido, preparando, pronto e entregue |
| Aumento dos custos de hospedagem |Monitorar o consumo do banco de dados e dos serviços utilizados|
## 9. Critérios de sucesso

| Objetivo | Como mediremos | Meta |
| -------- | ---------------- | ----- |
| Reduzir erros nos pedidos | Número de pedidos com erros antes e depois do sistema | Reduzir em pelo menos 50% os erros registrados |
| Melhorar o tempo de atendimento | Tempo médio entre registro e conclusão do pedido /Reduzir em pelo menos 30% o tempo médio|
| Melhorar o controle de estoque | Diferenças entre estoque registrado e estoque físico |Reduzir em pelo menos 50% as divergências |
| Reduzir processos manuais |Pedidos registrados digitalmente vs. manualmente |Pelo menos 80% dos pedidos registrados pelo sistema |
## 10. O que fica depois

- **Quem opera o sistema: Loja de açaí, utilizando os perfis de Administrador e Funcionário.
- Quem mantém tecnicamente: Equipe/empresa responsável pelo desenvolvimento, mediante contrato ou acordo de manutenção com a loja.
- Custo mensal estimado: R$ 2.000 a R$ 4.000+, considerando hospedagem/cloud, banco de dados, manutenção e suporte.
- Licença do código: a definir entre a equipe, a instituição de ensino e a loja parceira antes da entrega final.
