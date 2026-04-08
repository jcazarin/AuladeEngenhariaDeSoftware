```mermaid
%% Victor Parmeziani Limberger
stateDiagram-v2
    state "Nó inicial" as inicio <<start>>
    state "Nó final" as fim <<stop>>
    
    state fork_node <<fork>>
    state join_node <<join>>
    state decizao <<choice>>
    state uniao <<choice>>

    [*] --> Receber_Pedido
    Receber_Pedido --> fork_node : bifurcação (fork)

    %% Caminho de Cima: Pedido e Entrega
    fork_node --> Preencher_Pedido
    Preencher_Pedido --> decizao : ramificação

    decizao --> Entrega_Rapida : [Entrega Rápida]
    decizao --> Entrega_Normal : [Entrega Normal]

    Entrega_Rapida --> uniao
    Entrega_Normal --> uniao
    uniao --> join_node : ponto de união

    %% Caminho de Baixo: Faturamento
    fork_node --> Enviar_Fatura
    Enviar_Fatura --> Receber_Pagamento
    Receber_Pagamento --> join_node

    %% Finalização
    join_node --> Fechar_Pedido : junção (join)
    Fechar_Pedido --> [*]

    Receber_Pedido: Receber Pedido
    Preencher_Pedido: Preencher Pedido
    Entrega_Rapida: Entrega Rápida
    Entrega_Normal: Entrega Normal
    Enviar_Fatura: Enviar Fatura
    Receber_Pagamento: Receber Pagamento
    Fechar_Pedido: Fechar Pedido
