## 🧪 Caso de Teste 01 – Início da Simulação (Dados Pessoais)

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

### Evidência

🖼️ *Imagem 01:* [Tela de Dados Pessoais preenchida](../evidencias/Imagem-01-2026-01-16.png)

### Observações / Bugs

Nenhum bug identificado nesta etapa.

---

## 🧪 Caso de Teste 02 – Confirmação de Token SMS

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

## 🧪 Caso de Teste 03 – Preenchimento dos Dados da Proposta

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

## 🧪 Caso de Teste 04 – Visualização do Resultado da Simulação

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

### Observações / Bugs

Nenhum bug funcional identificado.

---

## 🐞 Testes Negativos Executados (Resumo)

| Cenário                 | Resultado                   | Evidências
| ----------------------- | --------------------------- | ---------------------------|
| Campo obrigatório vazio | Sistema bloqueia avanço     | Obriga-vazio1.png, Obriga-vazio1.png   |
| CPF inválido            | Sistema impede continuidade | CPF-invalido.png               |
| Token incorreto         | Sistema não valida          | Token-incorreto.png            |
| CAPTCHA não resolvido   | Simulação não executa       | CAPTCHA-nao-resolvido.png      |


✅ Comportamentos esperados atendidos.

---

## ✅ Conclusão Geral dos Testes

* A jornada de simulação de crédito imobiliário do Santander apresentou **estabilidade**
* Não foram identificados bugs críticos ou bloqueantes
* Fluxo bem estruturado e intuitivo
* Validações obrigatórias funcionando corretamente
* Processo atende aos requisitos funcionais esperados
