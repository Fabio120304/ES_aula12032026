# Casos de Uso para Sistema de Gestão de Academia FitPass

## 1. Cadastro de Usuário  
**Ator Principal:** Usuário  
**Objetivo:** O usuário deseja criar uma conta no sistema.  
**Pré-condições:** O usuário não deve ter uma conta existente.  
**Pós-condições:** O usuário é cadastrado no sistema.  
**Fluxo Principal:**  
1. O usuário acessa a página de cadastro.  
2. O usuário preenche os dados solicitados.  
3. O usuário confirma o cadastro.  
4. O sistema valida e registra o usuário.  
**Fluxos Alternativos:**  
- A1: Se os dados forem inválidos, o sistema exibe error.  

**RF Relacionados:** RF001 - Cadastro de Usuário  
**RNF Relacionados:** RNF001 - O sistema deve ser responsivo.  
**RN Relacionadas:** RN001 - O sistema deve aceitar cadastros com email válido.

## 2. Login do Usuário  
**Ator Principal:** Usuário  
**Objetivo:** O usuário deseja acessar sua conta.  
**Pré-condições:** O usuário deve estar cadastrado.  
**Pós-condições:** O usuário é autenticado no sistema.  
**Fluxo Principal:**  
1. O usuário acessa a página de login.  
2. O usuário insere seu email e senha.  
3. O sistema valida as credenciais.  
4. O usuário é redirecionado para a página inicial.  
**Fluxos Alternativos:**  
- A1: Se as credenciais estiverem incorretas, o sistema exibe mensagem de erro.  

**RF Relacionados:** RF002 - Login do Usuário  
**RNF Relacionados:** RNF002 - O sistema deve ter alta disponibilidade.  
**RN Relacionadas:** RN002 - O sistema deve expirar a sessão em 30 minutos de inatividade.

## 3. Agendamento de Aulas  
**Ator Principal:** Usuário  
**Objetivo:** O usuário deseja agendar uma aula na academia.  
**Pré-condições:** O usuário deve estar logado.  
**Pós-condições:** A aula é agendada no sistema.  
**Fluxo Principal:**  
1. O usuário acessa a página de agendamentos.  
2. O usuário escolhe a data e a aula.  
3. O usuário confirma o agendamento.  
4. O sistema registra o agendamento.  
**Fluxos Alternativos:**  
- A1: Se a aula estiver cheia, o sistema notifica o usuário.  

**RF Relacionados:** RF003 - Agendamento de Aulas  
**RNF Relacionados:** RNF003 - O sistema deve enviar notificações.  
**RN Relacionadas:** RN003 - O sistema deve permitir agendar aulas com 7 dias de antecedência.

## 4. Cancelamento de Aulas  
**Ator Principal:** Usuário  
**Objetivo:** O usuário deseja cancelar um agendamento de aula.  
**Pré-condições:** O usuário deve ter uma aula agendada.  
**Pós-condições:** A aula é cancelada no sistema.  
**Fluxo Principal:**  
1. O usuário acessa a lista de agendamentos.  
2. O usuário seleciona a aula a ser cancelada.  
3. O usuário confirma o cancelamento.  
4. O sistema atualiza o status do agendamento.  
**Fluxos Alternativos:**  
- A1: Se a aula já tiver acontecido, o sistema exibe mensagem de erro.  

**RF Relacionados:** RF004 - Cancelamento de Aulas  
**RNF Relacionados:** RNF004 - O sistema deve manter histórico de cancelamentos.  
**RN Relacionadas:** RN004 - O sistema deve permitir cancelamentos até 2 horas antes da aula.

## 5. Consulta de Resultados  
**Ator Principal:** Usuário  
**Objetivo:** O usuário deseja consultar seus resultados em atividades físicas.  
**Pré-condições:** O usuário deve estar logado.  
**Pós-condições:** Os resultados são exibidos.  
**Fluxo Principal:**  
1. O usuário acessa a página de resultados.  
2. O sistema exibe os resultados registrados.  
3. O usuário pode filtrar por data ou tipo de atividade.  
**Fluxos Alternativos:**  
- A1: Se não houver resultados, o sistema informa ao usuário.  

**RF Relacionados:** RF005 - Consulta de Resultados  
**RNF Relacionados:** RNF005 - O sistema deve ser intuitivo.  
**RN Relacionadas:** RN005 - O sistema deve permitir a comparação de resultados ao longo do tempo.

## 6. Atualização de Perfil  
**Ator Principal:** Usuário  
**Objetivo:** O usuário deseja atualizar suas informações pessoais.  
**Pré-condições:** O usuário deve estar logado.  
**Pós-condições:** As informações do perfil são atualizadas.  
**Fluxo Principal:**  
1. O usuário acessa a página de perfil.  
2. O usuário modifica as informações desejadas.  
3. O usuário confirma as alterações.  
4. O sistema atualiza as informações.  
**Fluxos Alternativos:**  
- A1: Se o usuário tentar usar um email já cadastrado, o sistema exibe erro.  

**RF Relacionados:** RF006 - Atualização de Perfil  
**RNF Relacionados:** RNF006 - O sistema deve ser seguro.  
**RN Relacionadas:** RN006 - O sistema deve permitir alterações de dados pessoais apenas ao próprio usuário.

## 7. Pagamento de Mensalidade  
**Ator Principal:** Usuário  
**Objetivo:** O usuário deseja pagar a mensalidade da academia.  
**Pré-condições:** O usuário deve estar logado e ter uma mensalidade pendente.  
**Pós-condições:** A mensalidade é considerada paga.  
**Fluxo Principal:**  
1. O usuário acessa a página de pagamentos.  
2. O usuário escolhe o método de pagamento.  
3. O usuário confirma o pagamento.  
4. O sistema registra a transação.  
**Fluxos Alternativos:**  
- A1: Se o pagamento falhar, o sistema notifica o usuário.  

**RF Relacionados:** RF007 - Pagamento de Mensalidade  
**RNF Relacionados:** RNF007 - O sistema deve oferecer várias formas de pagamento.  
**RN Relacionadas:** RN007 - O sistema deve emitir um comprovante de pagamento.

## 8. Cadastro de Funcionário  
**Ator Principal:** Administrador  
**Objetivo:** O administrador deseja cadastrar um novo funcionário.  
**Pré-condições:** O administrador deve estar logado.  
**Pós-condições:** O funcionário é cadastrado no sistema.  
**Fluxo Principal:**  
1. O administrador acessa a página de cadastro de funcionários.  
2. O administrador preenche os dados do funcionário.  
3. O usuário confirma o cadastro.  
4. O sistema registra o novo funcionário.  
**Fluxos Alternativos:**  
- A1: Se os dados forem inválidos, o sistema exibe erro.  

**RF Relacionados:** RF008 - Cadastro de Funcionário  
**RNF Relacionados:** RNF008 - O sistema deve manter dados históricos dos funcionários.  
**RN Relacionadas:** RN008 - O sistema deve requerer validação de dados do funcionário.

## 9. Alteração de Cadastro de Funcionário  
**Ator Principal:** Administrador  
**Objetivo:** O administrador deseja modificar o cadastro de um funcionário.  
**Pré-condições:** O administrador deve estar logado e selecionar um funcionário.  
**Pós-condições:** As informações do funcionário são atualizadas.  
**Fluxo Principal:**  
1. O administrador acessa a lista de funcionários.  
2. O administrador seleciona um funcionário.  
3. O administrador modifica as informações desejadas.  
4. O sistema atualiza as informações.  
**Fluxos Alternativos:**  
- A1: Se não encontrar o funcionário, o sistema exibe mensagem de erro.  

**RF Relacionados:** RF009 - Alteração de Cadastro de Funcionário  
**RNF Relacionados:** RNF009 - O sistema deve permitir a exclusão de funcionários.  
**RN Relacionadas:** RN009 - O sistema deve garantir a segurança nas informações do funcionário.

## 10. Relatório de Atendimento  
**Ator Principal:** Administrador  
**Objetivo:** O administrador deseja gerar um relatório de atendimentos.  
**Pré-condições:** O administrador deve estar logado.  
**Pós-condições:** O relatório é gerado.  
**Fluxo Principal:**  
1. O administrador acessa a página de relatórios.  
2. O administrador escolhe o tipo de relatório.  
3. O sistema gera o relatório solicitado.  
**Fluxos Alternativos:**  
- A1: Se não houver dados, o sistema exibe mensagem de alerta.  

**RF Relacionados:** RF010 - Relatório de Atendimento  
**RNF Relacionados:** RNF010 - O sistema deve permitir exportação dos dados do relatório.  
**RN Relacionadas:** RN010 - O sistema deve gerar relatórios em formato PDF.

## 11. Cadastro de Equipamento  
**Ator Principal:** Administrador  
**Objetivo:** O administrador deseja registrar um novo equipamento na academia.  
**Pré-condições:** O administrador deve estar logado.  
**Pós-condições:** O equipamento é cadastrado no sistema.  
**Fluxo Principal:**  
1. O administrador acessa a página de equipamentos.  
2. O administrador registra os dados do equipamento.  
3. O sistema confirma o cadastro.  
**Fluxos Alternativos:**  
- A1: Se os dados forem inválidos, o sistema exibe erro.  

**RF Relacionados:** RF011 - Cadastro de Equipamento  
**RNF Relacionados:** RNF011 - O sistema deve controlar o histórico de manutenções.  
**RN Relacionadas:** RN011 - O sistema deve permitir o registro de equipamentos em manutenção.

## 12. Atualização de Equipamento  
**Ator Principal:** Administrador  
**Objetivo:** O administrador deseja atualizar as informações de um equipamento.  
**Pré-condições:** O administrador deve estar logado e selecionar um equipamento.  
**Pós-condições:** As informações do equipamento são atualizadas.  
**Fluxo Principal:**  
1. O administrador acessa a lista de equipamentos.  
2. O administrador seleciona um equipamento.  
3. O administrador modifica as informações.  
4. O sistema atualiza as informações.  
**Fluxos Alternativos:**  
- A1: Se não encontrar o equipamento, o sistema exibe mensagem de erro.  

**RF Relacionados:** RF012 - Atualização de Equipamento  
**RNF Relacionados:** RNF012 - O sistema deve garantir a segurança nas informações do equipamento.  
**RN Relacionadas:** RN012 - O sistema deve permitir que somente administradores cadastrem e alterem informações de equipamentos.

## 13. Controle de Acesso ao Centro  
**Ator Principal:** Funcionário  
**Objetivo:** O funcionário deseja registrar a entrada e saída de usuários no centro.  
**Pré-condições:** O funcionário deve estar logado.  
**Pós-condições:** As entradas e saídas são registradas.  
**Fluxo Principal:**  
1. O funcionário acessa a página de controle de acesso.  
2. O funcionário registra a entrada de um usuário.  
3. O sistema confirma a entrada.  
4. O funcionário registra a saída de um usuário.  
5. O sistema confirma a saída.  
**Fluxos Alternativos:**  
- A1: Se o usuário não estiver cadastrado, o sistema exibe mensagem de erro.  

**RF Relacionados:** RF013 - Controle de Acesso ao Centro  
**RNF Relacionados:** RNF013 - O sistema deve registrar os horários exatos de entrada e saída.  
**RN Relacionadas:** RN013 - O sistema deve permitir consultar os registros de acesso pelo administrador.

## 14. Avaliação Física  
**Ator Principal:** Funcionário  
**Objetivo:** O funcionário deseja registrar a avaliação física de um usuário.  
**Pré-condições:** O funcionário deve estar logado e o usuário deve estar cadastrado.  
**Pós-condições:** A avaliação física é registrada.  
**Fluxo Principal:**  
1. O funcionário acessa a página de avaliações.  
2. O funcionário seleciona um usuário.  
3. O funcionário registra os dados da avaliação.  
4. O sistema confirma a avaliação.  
**Fluxos Alternativos:**  
- A1: Se os dados forem inconsistentes, o sistema exibe erro.  

**RF Relacionados:** RF014 - Avaliação Física  
**RNF Relacionados:** RNF014 - O sistema deve manter um histórico de avaliações para cada usuário.  
**RN Relacionadas:** RN014 - O sistema deve permitir que os resultados das avaliações sejam exportados.

## 15. Criação de Planos de Treino  
**Ator Principal:** Funcionário  
**Objetivo:** O funcionário deseja criar planos de treino personalizados para usuários.  
**Pré-condições:** O funcionário deve estar logado.  
**Pós-condições:** Os planos de treino são registrados.  
**Fluxo Principal:**  
1. O funcionário acessa a página de planos de treino.  
2. O funcionário seleciona um usuário.  
3. O funcionário registra os detalhes do plano.  
4. O sistema confirma o registro do plano.  
**Fluxos Alternativos:**  
- A1: Se não conseguir criar o plano, o sistema exibe erro.  

**RF Relacionados:** RF015 - Criação de Planos de Treino  
**RNF Relacionados:** RNF015 - O sistema deve permitir a edição de planos de treino existentes.  
**RN Relacionadas:** RN015 - O sistema deve garantir que os planos tenham uma duração mínima.

## 16. Gerenciamento de Feedbacks  
**Ator Principal:** Funcionário  
**Objetivo:** O funcionário deseja visualizar e responder a feedbacks de usuários.  
**Pré-condições:** O funcionário deve estar logado.  
**Pós-condições:** Feedbacks são respondidos ou arquivados.  
**Fluxo Principal:**  
1. O funcionário acessa a página de feedbacks.  
2. O funcionário visualiza feedbacks recebidos.  
3. O funcionário responde ao feedback.  
4. O sistema registra a resposta.  
**Fluxos Alternativos:**  
- A1: Se o feedback estiver respondido, o sistema exibe mensagem de alerta.  

**RF Relacionados:** RF016 - Gerenciamento de Feedbacks  
**RNF Relacionados:** RNF016 - O sistema deve notificar o funcionário sobre novos feedbacks.  
**RN Relacionadas:** RN016 - O sistema deve permitir que feedbacks sejam enviados diretamente da página de resultados.

## 17. Envio de Notificações  
**Ator Principal:** Sistema  
**Objetivo:** O sistema deve enviar notificações para usuários sobre seus agendamentos e pagamentos.  
**Pré-condições:** O usuário deve estar cadastrado.  
**Pós-condições:** As notificações são enviadas.  
**Fluxo Principal:**  
1. O sistema verifica agendamentos e pagamentos pendentes.  
2. O sistema envia notificações pertinentes aos usuários.  
3. O usuário recebe as notificações.  
**Fluxos Alternativos:**  
- A1: Se a notificação falhar, o sistema registra o erro.  

**RF Relacionados:** RF017 - Envio de Notificações  
**RNF Relacionados:** RNF017 - O sistema deve enviar notificações por email e SMS.  
**RN Relacionadas:** RN017 - O sistema deve garantir que o usuário possa desativar notificações.

## 18. Gestão de Promoções  
**Ator Principal:** Administrador  
**Objetivo:** O administrador deseja criar promoções e ofertas para usuários.  
**Pré-condições:** O administrador deve estar logado.  
**Pós-condições:** As promoções são registradas.  
**Fluxo Principal:**  
1. O administrador acessa a página de promoções.  
2. O administrador cria uma nova promoção.  
3. O sistema confirma a criação da promoção.  
**Fluxos Alternativos:**  
- A1: Se as informações da promoção forem inválidas, o sistema exibe erro.  

**RF Relacionados:** RF018 - Gestão de Promoções  
**RNF Relacionados:** RNF018 - O sistema deve permitir editar ou excluir promoções.  
**RN Relacionadas:** RN018 - O sistema deve garantir que as promoções sigam as políticas de marketing da academia.

## 19. Relatório de Finanças  
**Ator Principal:** Administrador  
**Objetivo:** O administrador deseja gerar relatórios financeiros.  
**Pré-condições:** O administrador deve estar logado.  
**Pós-condições:** Os relatórios financeiros são gerados.  
**Fluxo Principal:**  
1. O administrador acessa a página de relatórios financeiros.  
2. O sistema gera o relatório financeiro solicitado.  
**Fluxos Alternativos:**  
- A1: Se não houver dados financeiros, o sistema exibe alerta.  

**RF Relacionados:** RF019 - Relatório de Finanças  
**RNF Relacionados:** RNF019 - O sistema deve permitir que relatórios sejam exportados em CSV.  
**RN Relacionadas:** RN019 - O sistema deve garantir a precisão contábil nos relatórios.

## 20. Acesso a Suporte  
**Ator Principal:** Usuário  
**Objetivo:** O usuário deseja acessar suporte técnico.  
**Pré-condições:** O usuário deve estar logado.  
**Pós-condições:** O usuário recebe assistência.  
**Fluxo Principal:**  
1. O usuário acessa a página de suporte.  
2. O usuário envia uma solicitação de suporte.  
3. A equipe de suporte responde à solicitação.  
**Fluxos Alternativos:**  
- A1: Se a solicitação não for clara, o sistema solicita mais informações.  

**RF Relacionados:** RF020 - Acesso a Suporte  
**RNF Relacionados:** RNF020 - O sistema deve permitir o acompanhamento do status das solicitações.  
**RN Relacionadas:** RN020 - O sistema deve responder a solicitações em até 24 horas.