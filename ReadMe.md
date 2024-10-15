> **Tabela ECP:**

| UseCase                            | Critérios   | C.E.V | C.E.V |
|------------------------------------|-------------|-------|-------|
| Classificação Triangulo Equilatero | Nº Inputs   |   3   |  !=3  |
|                                    | Tipo Inputs |  int  | !=int |
|                                    | Restrições  |S1=S2=S3 and S1,S2,S3 >= 0|       |
| Classificação Triangulo Isósceles  | Nº Inputs   |   3   | !=3   |
|                                    | Tipo Inputs |  int  | !=int |
|                                    | Restrições  |S1=S2!=S3 or S2=S3!=S1 or S1=S3!=S2 and S1,S2,S3 >= 0|  |
| Classificação Triangulo Retângulo  | Nº Inputs   |   3    |   !=3    |
|                                    | Tipo Inputs | int      |   !=int    |
|                                    | Restrições  |S1^2 = S2^2 + S3^2 or S2^2 = S1^2 + S3^2 or S3^2 = S1^2 + S2^2 and S1,S2,S3 >= 0|       |
| Classificação Triangulo Escaleno   | Nº Inputs   |   3    |    !=3   |
|                                    | Tipo Inputs |   int    |  !=int     |
|                                    | Restrições  |  S1!=S2!=S3  and S1,S2,S3 >= 0|       |
| Classificação Triangulo Impossível | Nº Inputs   |   3    |    !=3   |
|                                    | Tipo Inputs |   int    |  !=int     |
|                                    | Restrições  |  S1!=S2!=S3  and S1,S2,S3 >= 0|       |

> **Tabela BVA:**

| Inputs                           | Min   | Max |
|----------------------------------|-------|-----|
| S1 | 0  |   maxINT  |
| S2 | 0   |   maxINT   |
| S3 | 0   |   maxINT   |

#TC1 (maxINT,maxINT,maxINT)
#TC2 (0,0,0)
#TC3 (maxINT,0,maxINT)
#TC4 (0,maxINT,maxINT)
#TC5 (maxINT,maxINT,0)
#TC6 (maxINT,0,0)
#TC7 (0,0,maxINT)
#TC8 (0,maxINT,0)
#TC9 (null,null,null)
#TC10 (,,)


> **Tabela TestCases:**

|#TC   | Inputs   | Condição | Resultado Esperado | Resultado Obtido|
|------|----------|----------|--------------------|-----------------|
|EQ_TC1|  (2,2,2) |S1,S2,S3 >= 0 |   Equilatero       |                 |
|IS_TC1 |  (2,2,3) |S1,S2,S3 >= 0 |   Isósceles       |                 |
|RE_TC1 |  (5,3,4) | S1,S2,S3 >= 0  |   Retângulo       |                 |
|ES_TC1 |  (2,3,4) |  S1,S2,S3 >= 0 |   Escaleno       |                 |
|IM_TC1 |  (0,0,0) | S1,S2,S3 <= 0    |   Impossível       |                 |



