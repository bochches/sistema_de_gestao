# Canvas do Projeto

**Projeto:** Sistema de gestão - Sorver Frios  · **Equipe:** Thayná Fortunato, Wendrieley Clara, Carolaine Silva· **Data:** 15/09/2026 · **Organização parceira:** Loja de açaí - Sorver Frios

---

## 1. Problema

A Sorver Frios recebe pedidos por diferentes canais, principalmente pelo balcão, WhatsApp e Instagram. Atualmente, os pedidos são registrados pelo celular, o que pode causar desorganização, principalmente nos horários de maior movimento.

O principal problema identificado é a dificuldade em seguir corretamente a ordem dos pedidos, o que pode ocasionar pedidos esquecidos ou preparados de forma incorreta.

Além disso, o controle de estoque é realizado de cabeça, com conferência constante dos produtos. Isso dificulta o acompanhamento da quantidade disponível e pode fazer com que alguns ingredientes acabem sem que sejam identificados antecipadamente.

**Evidências de que o problema existe** (dados, falas, observação):

- A loja recebe pedidos pelo balcão, WhatsApp e Instagram.
- Os pedidos são registrados pelo celular.
- Já ocorreram casos de pedidos perdidos, esquecidos ou preparados incorretamente.
- Em horários de maior movimento, existe dificuldade para seguir a ordem dos pedidos.
- O estoque é controlado atualmente de cabeça.
- Já aconteceu de ingredientes acabarem sem que isso fosse percebido antecipadamente.
- A loja recebe aproximadamente 10 a 15 pedidos por dia.
- A loja atende aproximadamente 20 a 30 clientes por dia.

## 2. Quem é afetado

| Quem | Quantas pessoas | Como é afetado hoje |
| ---- | --------------- | -------------------- |
| Clientes|20 a 30 |Podem ser afetados por erros, atrasos ou desorganização na ordem dos pedidos|
| Funcionários| 2 | Precisam registrar e acompanhar os pedidos, em horários de maior movimento|
| Entregadores | 2 | Precisam organizar os pedidos destinados às entregas|
| Proprietário/Gerente | 1 |Precisa acompanhar pedidos, estoque, vendas e a logística da loja |

## 3. Solução proposta

Um sistema de gestão para a Sorver Frios que permita cadastrar produtos, organizar os pedidos por ordem de atendimento, acompanhar o status de cada pedido, controlar o estoque e visualizar informações sobre as vendas.
O sistema deverá permitir que os funcionários registrem e acompanhem os pedidos, enquanto o proprietário terá acesso a funcionalidades administrativas, como controle de estoque, vendas e logística.
O sistema também deverá permitir o acompanhamento dos pedidos por diferentes etapas, como: 

**Pedido recebido → Em preparação → Pronto → Entregue**

Como a loja pode apresentar problemas de conexão com a internet, o sistema deverá considerar o funcionamento adequado mesmo em situações de instabilidade.

## 4. Funcionalidades do MVP (3 a 5)

| # | Funcionalidade | Para quem | Por que é essencial |
| --- | -------------- | --------- | -------------------- |
| 1 | Cadastrar e gerenciar produtos | Admin |Permite manter o cardápio atualizado |
| 2 | Registrar pedidos |Funcionário | Centraliza os pedidos e reduz erros |
| 3 | Alterar status do pedido |Funcionário |Permite acompanhar preparação e conclusão |
| 4 | Controlar estoque de ingredientes e complementos |Admin | Evita falta de produtos e facilita o controle |
| 5 | Visualizar pedidos e vendas | Admin | Permite acompanhar o funcionamento da loja e vendas |

**Informações registradas no pedido**

Cada pedido deverá registrar, conforme informado pelo proprietário:
- Nome do cliente;
- Quantidade;
- Tamanho do açaí;
- Complementos;
- Adicionais;
- Endereço, quando for entrega.

Os tamanhos atualmente comercializados são:
- P;
- M;
- G.
  
Entre os principais complementos estão:

- Leite;
- Granola;
- Farinha láctea;
- Banana;
- Leite condensado.

Alguns adicionais possuem preços diferentes, como **morango e cremes**.

## 5. Fora do escopo

O que **não** faremos nesta versão, e por quê:

| Não faremos | Por quê |
| ----------- | ------- |
| Cadastro de novos funcionários| O proprietário informou que essa função não é necessária neste primeiro momento |
| Integração com iFood/WhatsApp|O proprietário informou que não considera essa integração necessária |
| Emissão de nota fiscal pelo sistema | Não foi considerada necessária para o sistema neste momento|
| Aplicativo para o cliente realizar pedidos |O proprietário informou que não deseja que os próprios clientes façam pedidos pelo aplicativo| 
| Sistema avançado de contabilidade |Não foi identificado como uma necessidade principal da loja |

**Funcionalidades que podem ser consideradas futuramente**

O pagamento diretamente pelo aplicativo **não é necessário neste momento**, mas o proprietário informou que seria uma funcionalidade positiva caso pudesse ser adicionada futuramente.

O programa de fidelidade para clientes foi considerado **uma funcionalidade desejada**.

## 6. Usuários e papéis

| Papel | O que pode fazer |
| ----- | ------------------ |
| Administrador/Gerente | Cadastra produtos, gerencia estoque, acompanha pedidos e visualiza vendas|
| Funcionário | Registra e acompanha pedidos |
| Entregador | Realiza as entregas dos pedidos |
| Cliente    |Recebe o pedido realizado por meio dos canais utilizados pela loja|

O sistema será utilizado pelos **2 funcionários**, porém o principal usuário administrativo será o proprietário, **Charles**.

O proprietário deverá possuir permissões diferentes das dos funcionários, principalmente para funções relacionadas ao **controle de estoque, vendas e logística**.

## 7. Restrições

| Tipo            | Restrição                                                  |
| --------------- | ----------------------------------------------------------- |
| Prazo           | 18 a 22 semanas, divididas entre planejamento, back-end, front-end, testes/QA e implantação |
| Equipe          | 3 pessoas, 20 a 25 h/semana no total |
| Técnica         |Flutter/Dart para aplicativo, Node.js ou Firebase Cloud Functions, Cloud Firestore/NoSQL   |
| Contexto de uso | O sistema será utilizado principalmente durante o atendimento e preparação dos pedidos|
| Conectividade   | Deve funcionar adequadamente mesmo em situações de instabilidade de internet
| Uso             | O sistema deverá possuir uma interface simples, considerando que será utilizado durante o atendimento e preparação dos pedidos|

## 8. Riscos principais

| Risco | O que faremos |
| ----- | -------------- |
| Instabilidade da internet | Utilizar armazenamento local e sincronização quando a conexão retornar |
| Dificuldade em manter a ordem dos pedidos | Organizar os pedidos em uma fila digital, mostrando claramente a ordem de atendimento |
| Erros ou pedidos esquecidos | Utilizar uma tela de acompanhamento com os diferentes status dos pedidos|
| Falhas no controle de estoque| Registrar e atualizar digitalmente os produtos disponíveis e emitir alertas quando determinado item estiver acabando |
| Grande quantidade de pedidos em horários de pico |Organizar os pedidos por ordem de chegada e status de preparação |

O proprietário informou que, atualmente, **não identifica nenhum outro risco específico relacionado à utilização do sistema**, além das dificuldades já mencionadas.

## 9. Critérios de sucesso

| Objetivo | Como mediremos | Meta |
| -------- | ---------------- | ----- |
| Melhorar a organização dos pedidos | Comparação da quantidade de pedidos perdidos, esquecidos ou preparados incorretamente antes e depois do sistema |Reduzir os erros relacionados aos pedidos|
| Melhorar a ordem de atendimento | Acompanhamento dos pedidos por ordem de chegada e status |Permitir que os pedidos sejam acompanhados corretamente|
| Melhorar o controle de estoque | Comparação entre a quantidade registrada no sistema e a quantidade disponível na loja |Identificar produtos que estão acabando antes que faltem |
| Melhorar o acompanhamento das vendas |Visualização das vendas diárias, semanais e mensais |Permitir que o proprietário acompanhe os resultados da loja |
| Melhorar a tomada de decisão | Visualização dos tamanhos e complementos mais vendidos | Identificar os produtos com maior demanda |
## 10. O que fica depois

- **Quem opera o sistema:** Loja de açaí Sorver Frios, utilizando principalmente o perfil de Administrador/Proprietário e os perfis dos funcionários.
- **Principal responsável pelo controle administrativo:** Charles, proprietário da loja.
- **Manutenção técnica:** Equipe/empresa responsável pelo desenvolvimento, mediante contrato ou acordo de manutenção com a loja.
- **Uso futuro:** O proprietário demonstrou interesse em utilizar o sistema em outras unidades caso a solução funcione adequadamente.
- **Acompanhamento remoto:** O proprietário deseja poder acompanhar as vendas da loja pelo celular mesmo quando estiver fora do estabelecimento.
- **Controle futuro desejado:** O proprietário deseja visualizar quanto existe em estoque, quais produtos precisam ser comprados e acompanhar os pedidos.
- **Custo mensal estimado:** A definir.
- **Licença do código:** A definir entre a equipe, a instituição de ensino e a organização parceira antes da entrega final.
