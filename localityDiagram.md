```mermaid
    erDiagram
        CFC ||..|{ CATEGORIA : has
        CFC ||..|| LICENCA : has
        CFC ||..|| RESPONSAVEL_LEGAL : has
        CFC ||..|{ ENDERECO :has
        CFC }|..|| LOCALIDADE : has
        LOCALIDADE ||..|{ LOCALIDADE : has
        LOCALIDADE }|..|{ REGRA :has
        REGRA }|..|{ REGISTRO :has
```