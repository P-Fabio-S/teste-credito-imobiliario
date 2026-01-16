# 📘 Casos de Teste – Simulação de Crédito Imobiliário | Santander

| ID    | Caso de Teste                                | Pré-condições                             | Passos                                                                                                                     | Resultado Esperado                              | Resultado Obtido                          | Evidências                              | Status                     |
| ----- | -------------------------------------------- | ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------- | ----------------------------------------- | --------------------------------------- | -------------------------- |
| CT-01 | Acesso ao simulador de crédito imobiliário   | Usuário com acesso à internet e navegador | 1. Acessar o site do Santander: [Negócios Imobiliários](https://www.negociosimobiliarios.santander.com.br/negociosimobiliarios/#/home)<br>2. Clicar em "Simule e Contrate"<br>                 | Página do simulador exibida corretamente        | Página exibida conforme esperado          | `evidencia_01_inicio_simulacao.png`     | ✅ Aprovado                 |
| CT-02 | Simulação com dados válidos                  | Acesso ao simulador                       | 1. Informar valor válido do imóvel<br>2. Informar valor de entrada válido<br>3. Selecionar prazo<br>4. Confirmar simulação | Exibição de parcelas, prazo e taxa de juros     | Valores exibidos corretamente             | `evidencia_02_preenchimento_dados.png`  | ✅ Aprovado                 |
| CT-03 | Validação de campos obrigatórios             | Acesso ao simulador                       | 1. Não preencher campos obrigatórios<br>2. Tentar avançar                                                                  | Exibição de mensagens solicitando preenchimento | Mensagens exibidas corretamente           | `evidencia_03_mensagem_erro_campos.png` | ✅ Aprovado                 |
| CT-04 | Valor de entrada maior que o valor do imóvel | Acesso ao simulador                       | 1. Informar valor do imóvel<br>2. Informar entrada maior que o valor do imóvel<br>3. Tentar simular                        | Bloquear simulação e exibir mensagem clara      | Simulação bloqueada com mensagem genérica | `evidencia_04_entrada_maior.png`        | ⚠️ Aprovado com observação |
| CT-05 | Simulação sem informar valor de entrada      | Acesso ao simulador                       | 1. Informar valor do imóvel<br>2. Deixar entrada em branco<br>3. Confirmar simulação                                       | Permitir simulação ou aplicar valor mínimo      | Simulação realizada com sucesso           | `evidencia_05_entrada_vazia.png`        | ✅ Aprovado                 |
| CT-06 | Seleção do prazo máximo de financiamento     | Acesso ao simulador                       | 1. Informar dados válidos<br>2. Selecionar maior prazo disponível<br>3. Simular                                            | Simulação realizada sem erros                   | Simulação realizada corretamente          | `evidencia_06_prazo_maximo.png`         | ✅ Aprovado                 |

---

### 🔹 Observações

* Coloque **o nome exato do arquivo de evidência** que está na pasta `/evidencias/` do repositório.
* Se quiser, você pode até usar links no GitHub:

```md
[Evidência](../evidencias/evidencia_01_inicio_simulacao.png)
```

Assim fica clicável direto no README do GitHub.

---

Se você quiser, posso **refazer toda a tabela final com links clicáveis das evidências** para GitHub, pronta para colar e usar, sem precisar editar depois.

Quer que eu faça isso?
