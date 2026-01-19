# Casos de Teste – Simulação de Crédito Imobiliário

Este diretório contém os casos de teste executados para validar a jornada de simulação de crédito imobiliário do Banco Santander.

## Estrutura dos Arquivos

- `README.md` — arquivo índice e documentação geral dos casos de teste  
- `casos_de_teste_simulacao_credito.md` — arquivo com a descrição detalhada dos casos de teste (funcionais e negativos)  

## Objetivo

Garantir a cobertura das funcionalidades principais da jornada, validando o fluxo completo desde o preenchimento dos dados pessoais até a visualização dos resultados da simulação.

## Tipos de Casos de Teste

- **Funcionais:** validação do comportamento esperado para entradas válidas  
- **Segurança:** validação da autenticação via token SMS  
- **Regressão:** validação da exibição dos resultados da simulação  
- **Negativos:** validação das mensagens e bloqueios para dados inválidos ou incompletos  

## Como Utilizar

1. Abra os arquivos de casos de teste para verificar os passos, pré-condições, dados, resultados esperados e evidências.  
2. Utilize as evidências presentes na pasta `/evidencias` para validar os testes.  
3. Consulte o README raiz para contexto geral do projeto e integração com documentação de processos.

---

## Resumo dos Casos de Teste Principais

| ID            | Título                                  | Tipo              | Status      |
|---------------|----------------------------------------|-------------------|-------------|
| CT-IMOBS-001  | Início da Simulação (Dados Pessoais)   | Funcional         | ✅ Aprovado |
| CT-IMOBS-002  | Confirmação de Token SMS                | Funcional/Security| ✅ Aprovado |
| CT-IMOBS-003  | Preenchimento Dados da Proposta (Usecasa) | Funcional     | ✅ Aprovado |
| CT-IMOBS-004  | Visualização do Resultado da Simulação | Funcional/Regressão| ✅ Aprovado |
| CT-IMOBS-005  | Dados da Proposta (Financiamento)      | Funcional         | ✅ Aprovado |
| CT-IMOBS-006  | Resultado da Simulação (Financiamento) | Funcional/Regressão| ✅ Aprovado |

---

## Testes Negativos Executados

| ID        | Cenário                  | Resultado Esperado                 |
|-----------|--------------------------|----------------------------------|
| CT-NEG-01 | Campo obrigatório vazio  | Sistema bloqueia o avanço         |
| CT-NEG-02 | CPF inválido             | Sistema impede continuidade      |
| CT-NEG-03 | Token incorreto          | Sistema não valida               |
| CT-NEG-04 | CAPTCHA não resolvido    | Simulação não executa            |

