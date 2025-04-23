# 💃🏻🕺🏽 DanceHub - Um hub de eventos de dança

## Membros

- Leonardo (Tech Lead/Scrum Master)
- Genilson (Dev)
- Guilherme (Dev)
- Gustavo (Dev)
- Saullo (QA)

## Definições do projeto

Sugestões de funcionalidades no website feitas pelos membros da equipe

### Saullo

- Registro de clientes da plataforma e funcionários do festival.
- Inscrição em eventos por parte do diretor da companhia de dança ou pelo dançarino autônomo.
- Registro de eventos pelos funcionários do festival.
- Múltiplos perfis (Dançarino/Diretor/Coreógrafo/Funcionário).
- Pagamento das inscrições do evento e check-in com QR Code para obter acesso as áreas.
- Cancelamento do cartão em caso de perda.

Observação: Se a pessoa quiser cancelar a inscrição do evento, dar um prazo pra ela de até um dia antes do evento para ocorrer a devolução do dinheiro. Caso já tenha pago, mas apareceu outro evento que queira ir e desista do primeiro, mantenha os dados e a pessoa deve pagar a diferença do valor dos eventos.

### Guilherme

- Mapa mental das [ideias](https://miro.com/app/board/uXjVN3F-IB0=/?share_link_id=916369283026)

### Gustavo

- Mapa mental das [ideias](https://miro.com/app/board/uXjVN4fKbj4=/?share_link_id=542289396261)

### Leonardo

**Registro de usuários** (beta version)

- Funcionário do festival
- Diretor de companhia de dança
- Coreógrafo da companhia
- Dançarino (pode ser autônomo)

**Companhias** (beta version)

- Apenas um diretor de companhia poderá registrar uma nova
- A companhia possui diversos coreógrafos e dançarinos
- Os coreógrafos e dançarinos devem ser convidados por e-mail pelo diretor
- Para evitar criação desenfreada de companhias, há uma taxa inicial a ser paga (opcional)

**Cartão Fidelidade** (v2?)

- Todos usuários, exceto funcionário, possuem o cartão fidelidade
- O cartão é físico e possui um Qr Code que possui um token para identificar a pessoa
- O check-in no evento (registrar a entrada) ocorre através da leitura do qr code do cartão
- Em caso de perda do cartão, é gerado um novo token
- Possui saldo para consumir serviços presenciais

**Criação de Eventos e Catalogação** (beta version)

- Prerrogativa dos funcionários
- Eventos ocorrem em determinado local e horário
- Possuem uma identificação
- Apresentam regulamento para inscrição
- Eventos de dança podem ser SOLO, DUO, TRIO, EQUIPE.
- Podem possuir vencedor (companhia/dançarino)
- Todos possuem acesso ao catálogo de eventos

**Inscrição virtual em eventos** (beta version)

- Realizada pelo diretor ou dançarino autônomo
- Dançarino autônomo só poderá se inscrever em eventos solos
- Diretor deverá inscrever o coreógrafo e dançarinos da sua companhia
- Pagamento das inscrições pelo diretor ou dançarino autônomo (opcional)

**Inscrição presencial on-time** (v2?)

- Eventos que não possuem limite de inscrições
- Leitura composta: inicia-se uma sessão no leitor em que lê todos os integrantes da companhia
- Leitura simples: dançarino autônomo (dança solo)


## Desenvolvimento

### API BACKEND

- Tecnologias: Spring Data JPA, Spring Security, PostgreSQL.

**[+]** Projeto criado com a autenticação de usuários feita (26/01) <br>
**[+]** Criação da entidade evento e endpoint POST (26/01) <br>
**[+]** Upload do regulamento para o evento (27/01) <br>
**[+]** Criação da entidade inscrição e endpoint POST (28/01) <br>
**[+]** Correção da autenticação do usuário (28/01) <br>
**[+]** Download do regulmento do evento (29/01) <br>
**[+]** Retorno paginado dos eventos (29/01) <br> 
**[+]** Inscrição da companhia em evento (30/01) <br>
**[+]** Correção das validações do usuário (30/01) <br>
**[+]** Criação de companhia e convite (30/01) <br>
**[+]** Retorno das inscrições de atração no evento (GET) (31/01) <br>
**[+]** Finalização da lógica de convites (01/02) <br>
**[+]** Correções dos endpoints (03/02) <br>
**[+]** Adicionado os endpoints getRoles e getCategories (03/02) <br>
**[+]** Correções gerais (04/02 - 14/02) <br>
**[+]** Retorno dos usuários da companhia (14/02) <br>
**[+]** Correções gerais (15/02 - 17/02) <br>

### FRONTEND

- Tecnologias: ReactJS

**[+]** Projeto criado com o esqueleto de algumas páginas (29/01) <br>
**[+]** Consumo de alguns endpoints da API (30/01 - 05/02) <br>
**[+]** Mudança no estilo da página principal (05/02) <br>
**[+]** Refatoração no código (09/02) <br>
**[+]** Refatoração no código (10/02) <br>
**[+]** Melhoras no design (13/02) <br>
**[+]** Correções e melhoras no design (14/02) <br>
**[+]** Inscrição em eventos (15/02) <br>
**[+]** Refatoração no código (16/02) <br>
**[+]** Correções na inscrição em eventos (17/02) <br>

## Resultado final

O MVP foi entregue com sucesso :D <br>
Tivemos um ótimo feedback dos mentores. <br>
Para executar o que foi feito, basta configurar as credenciais de um DB e de um e-mail na application.yaml (dancehub-api).
