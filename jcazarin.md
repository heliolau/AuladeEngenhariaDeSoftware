flowchart TD
    A((Início)) --> B[Receber Pedido]

    B --> F1{{Fork}}

    F1 --> C1[Preencher Pedido]
    C1 --> D1[Realizar Entrega]

    F1 --> C2[Enviar Fatura]
    C2 --> D2[Receber Pagamento]

    D1 --> J1{{Join}}
    D2 --> J1

    J1 --> E[Fechar Pedido]
    E --> F((Fim))
