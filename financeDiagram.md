```mermaid
    erDiagram
        CONTRATO }o..|| PRODUTO :has
        CONTRATO ||..|| CONTA_DEBITO :has
        CONTA_DEBITO }|..|| STATUS_CONTA :has
        PRODUTO }|..|| PAGAMENTO_BENEFICIARIO :has
        BENEFICIARIO ||..|| PAGAMENTO_BENEFICIARIO :has
        SPLIT_PAGAMENTO ||..|| PAGAMENTO_BENEFICIARIO :has
        CONTA_DEBITO ||..|{ PARCELA :has
        PAGAMENTO ||..|| PARCELA :has
```