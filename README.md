# # 📧 Disparo de E-mail Automático via Google Sheets + Apps Script

Este projeto contém um script do Google Apps Script que adiciona um menu personalizado no Google Sheets, permitindo o envio automatizado de e-mails personalizados com base nos dados da planilha.

---

## ⚙️ Funcionalidades

- Adiciona o menu **"Disparo E-mail"** ao abrir a planilha.
- Permite digitar o e-mail de um cliente e disparar um e-mail personalizado para ele.
- Marca na planilha se o e-mail foi enviado com sucesso ou se houve erro.
- Personaliza o conteúdo do e-mail com nome do cliente, nome do CS e data do onboarding.
- Inclui botão com link para formulário de feedback.

---

## 🧩 Estrutura esperada da planilha

A planilha ativa deve conter os seguintes dados (ajustáveis no código):

| Coluna | Conteúdo              |
|--------|------------------------|
| A      | Nome do cliente        |
| B      | E-mail do cliente      |
| D      | Nome do CS             |
| E      | Data do onboarding     |
| F      | Status do envio        |

---

## 🚀 Como usar

1. Abra seu Google Sheets com os dados dos clientes.
2. Vá em **Extensões > Apps Script**.
3. Copie e cole o conteúdo do arquivo `.gs` no editor.
4. Substitua os seguintes valores no script:
   - `LINK DA LOGO DA SUA EMPRESA`
   - `https://forms.gle/SEULINKAQUI`
5. Salve o projeto e recarregue a planilha.
6. Use o menu **Disparo E-mail > Enviar email por e-mail do cliente** para iniciar o envio.

---

## ✏️ Personalização

- Você pode modificar o HTML do corpo do e-mail para usar sua identidade visual.
- Pode também alterar os nomes das colunas no código, caso sua estrutura seja diferente.

---

## 📌 Observações

- O envio é feito com a função `GmailApp.sendEmail()`, que utiliza sua conta do Google para enviar.
- Para evitar spam ou bloqueios, respeite os limites diários do Gmail (envio de até 100 e-mails/dia em contas gratuitas).

---

## 📥 Exemplo de uso

> “Queríamos enviar uma pesquisa de satisfação para clientes que passaram pelo onboarding. Com esse script, ficou fácil disparar e acompanhar diretamente pelo Sheets, sem precisar sair da planilha.”

---

## 📄 Licença

Uso livre para fins pessoais e comerciais. Se modificar e melhorar, sinta-se à vontade para contribuir de volta 😉

---

