# iGiota — protótipo inicial

## O que esta versão já permite
- Cadastrar pessoas e dívidas em reais.
- Guardar a cotação BRL→EUR da data da dívida quando o serviço de câmbio responder.
- Consultar o equivalente em euros pela cotação atual.
- Registrar pagamentos parciais e totais.
- Ver o histórico de pagamentos por dívida.
- Ver resumo geral e saldo por pessoa.
- Exportar e importar um backup JSON.
- Funcionar como web app instalável (PWA), quando servido por HTTPS.

## Limitações importantes desta primeira versão
- Os dados ficam somente no armazenamento local do navegador/aparelho. Ainda NÃO existe conta, login, sincronização entre iPhone e iPad nem backup automático na nuvem.
- O boletim mensal por e-mail/PDF ainda não está implementado.
- A cotação vem da API pública Frankfurter, baseada em taxas de referência; pode não refletir a taxa efetiva de uma operação bancária e pode não estar disponível em todos os momentos.
- Não é uma aplicação publicada na App Store.

## Como testar
1. Hospede os arquivos em um serviço de hospedagem estática com HTTPS.
2. Abra o endereço no Safari do iPhone.
3. Use Compartilhar → Adicionar à Tela de Início.
4. Faça um cadastro de teste e exporte um backup para guardar os dados.

Para habilitar nuvem e sincronização, a próxima etapa é criar o projeto Supabase, configurar autenticação e migrar o armazenamento local para uma base de dados protegida por usuário.
