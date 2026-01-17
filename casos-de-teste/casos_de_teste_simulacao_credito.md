##  Caso de Teste 01 – Início da Simulação (Dados Pessoais)

**ID:** CT-IMOBS-001

**Título:** Preenchimento correto dos dados pessoais para iniciar simulação

**Tipo:** Funcional

**Prioridade:** Alta

### Pré-condições

* Usuário com CPF válido
* Acesso à internet
* Navegador compatível

### Passos

1. Acessar a URL: [Negócios Imobiliários](https://www.negociosimobiliarios.santander.com.br/negociosimobiliarios/#/home) de simulação de crédito imobiliário do Santander
2. Informar Nome Completo
3. Informar CPF válido
4. Informar Data de Nascimento
5. Informar E-mail válido
6. Informar Número de Celular válido
7. Informar Renda Mensal
8. Clicar no botão **“Próximo”**

### Resultado Esperado

* Sistema deve aceitar os dados preenchidos
* Usuário deve ser direcionado para a etapa de confirmação via SMS

### Resultado Obtido

✅ Conforme esperado

### Evidência

🖼️ *Imagem 01:* [Tela de Dados Pessoais preenchida](../evidencias/Imagem-01-2026-01-16.png)

### Observações / Bugs

Nenhum bug identificado nesta etapa.

---

##  Caso de Teste 02 – Confirmação de Token SMS

**ID:** CT-IMOBS-002

**Título:** Validação de código SMS para autenticação do usuário

**Tipo:** Funcional / Segurança

**Prioridade:** Alta

### Pré-condições

* Celular informado corretamente
* Recebimento do SMS

### Passos

1. Aguardar recebimento do código SMS
2. Informar o código recebido no campo indicado
3. Clicar em **“Confirmar Código Token”**

### Resultado Esperado

* Sistema deve validar o código
* Usuário deve avançar para a etapa de Dados da Proposta

### Resultado Obtido

✅ Código validado com sucesso
✅ Avanço de etapa realizado corretamente

### Evidência

*Imagem 02:* [Confirmação de SMS](../evidencias/Imagem-02-2026-01-16.png)

*Imagem 03:* [Código validado com sucesso](../evidencias/Imagem-03-2026-01-16.png)

### Observações / Bugs

Nenhum bug identificado.

---

##  Caso de Teste 03 – Preenchimento dos Dados da Proposta (Empréstimo – Usecasa)

**ID:** CT-IMOBS-003

**Título:** Preenchimento dos dados do imóvel para simulação

**Tipo:** Funcional

**Prioridade:** Alta

### Pré-condições

* Usuário autenticado via SMS

### Passos

1. Selecionar objetivo **“Empréstimo – Usecasa”**
2. Selecionar tipo de imóvel **Residencial – Casa**
3. Informar valor do imóvel (R$ 400.000,00)
4. Informar valor a financiar (R$ 40.000,00)
5. Informar prazo de financiamento (20 anos)
6. Selecionar opção de financiamento de IOF
7. Resolver o CAPTCHA
8. Clicar em **“Simular”**

### Resultado Esperado

* Sistema deve aceitar os dados informados
* Simulação deve ser processada com sucesso

### Resultado Obtido

✅ Simulação processada corretamente

### Evidência

*Imagem 04:* [Tela de Dados da Proposta](../evidencias/Imagem-04-2026-01-16.png)

### Observações / Bugs

Nenhum bug identificado.

---

##  Caso de Teste 04 – Visualização do Resultado da Simulação

**ID:** CT-IMOBS-004

**Título:** Exibição correta dos valores da simulação de crédito

**Tipo:** Funcional / Regressão

**Prioridade:** Alta

### Pré-condições

* Simulação concluída com sucesso

### Passos

1. Visualizar valor do empréstimo
2. Verificar prazo total em meses
3. Validar valor da parcela inicial
4. Conferir taxa de juros e CET
5. Verificar botão de continuidade da análise de crédito

### Resultado Esperado

* Todos os valores devem ser exibidos claramente
* Taxas e parcelas devem estar coerentes com os dados informados

### Resultado Obtido

✅ Valores exibidos corretamente
✅ Taxa efetiva: 21,70% a.a
✅ Parcela inicial exibida corretamente

### Evidência

*Imagem 05:* [Resultado da Simulação](../evidencias/Imagem-05-2026-01-16.png)

*Imagem 06:* [Resultado da Simulação](../evidencias/Imagem-06-2026-01-16.png)

### Observações / Bugs

Nenhum bug funcional identificado.

---
## Caso de Teste 05 – Preenchimento dos Dados da Proposta (Financiamento do Imovel)

**ID:** CT-IMOBS-005

**Título:** Preenchimento dos dados do imóvel para simulação

**Tipo:** Funcional

**Prioridade:** Alta

### Pré-condições

* Usuário autenticado via SMS

### Passos

1. Selecionar objetivo **“Financiamento do Imovel – ”**
2. Selecionar tipo de imóvel **Residencial – Apartamento**
3. Informar valor do imóvel (R$ 300.000,00)
4. Informar valor mínimo a financiar (R$ 60.000,00)
5. Informar prazo de financiamento máximo (35 anos)
6. Em "Deseja financiar as despesas de ITBI e Registro do imóvel? (5% do valor do Imóvel)" selecione a opção "não".
7. Resolver o CAPTCHA
8. Clicar em **“Simular”**

### Resultado Esperado

* Sistema deve aceitar os dados informados
* Simulação deve ser processada com sucesso

### Resultado Obtido

✅ Simulação processada corretamente

### Evidência

*Imagem 07:* [Tela de Dados da Proposta](../evidencias/Imagem-07-2026-01-16.png)

### Observações / Bugs

Nenhum bug identificado.

---

## Caso de Teste 6 – Visualização do Resultado da Simulação (Financiamento de Imóvel)

ID: CT-IMOBS-06
Título: Exibição correta dos valores do resultado da simulação de financiamento imobiliário
Tipo: Funcional / Regressão
Prioridade: Alta

## Pré-condições

* Usuário autenticado via SMS
* Simulação de financiamento imobiliário concluída com sucesso

### Passos

1. Visualizar o valor do financiamento
2. Verificar o prazo total do financiamento em meses
3. Conferir o valor da entrada
4. Validar o valor da 1ª parcela
5. Conferir a taxa de juros efetiva
6. Verificar o Custo Efetivo Total (CET)
7. Verificar a exibição do seguro habitacional (CESH)
8. Validar a presença do botão “Continue para analisar o crédito”

## Resultado Esperado

* Todos os valores devem ser exibidos de forma clara e legível
* Valor do financiamento deve ser R$ 60.000,00
* Prazo deve ser exibido como 35 anos (420 meses)
* Valor da entrada deve ser exibido corretamente
* Valor da parcela inicial deve estar coerente com os dados simulados
* Taxa de juros efetiva, CET e seguro habitacional devem estar visíveis
* Botão para continuidade da análise de crédito deve estar disponível

## Resultado Obtido

✅ Valor do financiamento exibido corretamente: R$ 60.000,00.
✅ Prazo exibido corretamente: 420 meses.
✅ Valor da 1ª parcela exibido corretamente: R$ 820,20.
✅ Taxa efetiva exibida corretamente: 13,29% a.a / 1,05% a.m + TR.
✅ CET exibido corretamente: 15,30% a.a.
✅ Seguro habitacional (CESH) exibido corretamente.
✅ Botão “Continue para analisar o crédito” exibido e funcional.

## Evidência

*Imagem 08:* [Tela de Dados da Proposta](../evidencias/Imagem-08-2026-01-16.png)
*Imagem 09:* [Tela de Dados da Proposta](../evidencias/Imagem-09-2026-01-16.png)

## Observações / Bugs

* Nenhum bug funcional identificado.


## 🐞 Testes Negativos Executados (Resumo)

| Cenário                   | Resultado                   | Evidências
| ------------------------- | --------------------------- | ---------------------------|
| Campo obrigatório vazio   | Sistema bloqueia avanço     | [Campo-obrigatório.png](../evidencias/Campo-obrigatorio.png)                   |
| CPF inválido              | Sistema impede continuidade | [CPF-invalido.png](../evidencias/CPF-invalido.png)                             |
| Token incorreto           | Sistema não valida          | [Token-incorreto.mp4](../evidencias/token-incorreto.mp4)                       |
| RECAPTCHA não resolvido   | Simulação não executa       | [RECAPTCHA-nao-resolvido.mp4](../evidencias/RECAPTCHA-nao-resolvido.mp4)       |


✅ Comportamentos esperados atendidos.

---

## ✅ Conclusão Geral dos Testes

* A jornada de simulação de crédito imobiliário do Santander apresentou **estabilidade**
* Não foram identificados bugs críticos ou bloqueantes
* Fluxo bem estruturado e intuitivo
* Validações obrigatórias funcionando corretamente
* Processo atende aos requisitos funcionais esperados
