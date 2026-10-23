# Desafio Criativo DIO — Planejando Automações com N8N Usando Apenas Bons Prompts

## Prompt Final

Atue como um especialista em N8N.

Crie uma automação para registrar automaticamente leads recebidos por formulário e qualificá-los antes de enviar ao time comercial.

Público:
Equipe comercial e equipe de marketing.

Ferramentas envolvidas:
Google Forms, Google Sheets, Gmail e Slack.

Fluxo:
1. Receber uma nova resposta do Google Forms (gatilho).
2. Validar se o e-mail informado é válido e se o campo "interesse" foi preenchido.
3. Registrar os dados do lead em uma planilha do Google Sheets.
4. Enviar um e-mail de confirmação automática para o lead.
5. Se o lead for classificado como "alto interesse", enviar uma notificação no canal do Slack do time comercial.
6. Caso o e-mail seja inválido, registrar o erro em uma aba separada da planilha e não notificar o time.

Regras:
- Ignorar registros sem e-mail válido (usar validação de formato de e-mail).
- Não enviar e-mail de confirmação duplicado para o mesmo endereço em menos de 24 horas.
- Leads com interesse "alto" devem gerar notificação no Slack em até 1 minuto após o registro.
- Todos os dados devem ser armazenados na planilha, mesmo os inválidos, para fins de auditoria.

Explique quais nós do N8N devem ser utilizados e a lógica de funcionamento do workflow.
