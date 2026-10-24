# Análise de Logs do Linux — Exercício Simulado

## 1. Objetivo

Praticar a leitura de logs de autenticação para identificar atividades que merecem investigação em um ambiente Linux.

## 2. Cenário

Durante uma verificação de rotina, foram identificados os seguintes eventos fictícios no log de autenticação:

- 09:10 — Falha de autenticação para um usuário.
- 09:12 — Nova falha de autenticação para o mesmo usuário.
- 09:14 — Terceira falha de autenticação.
- 09:16 — Login realizado com sucesso para esse usuário.

## 3. Análise inicial

A sequência de falhas seguida por um login bem-sucedido pode indicar uma tentativa de acesso indevido. Entretanto, também pode ocorrer por erro de digitação ou esquecimento de senha.

Os eventos disponíveis, isoladamente, não comprovam uma invasão.

## 4. Próximas ações

1. Identificar o usuário envolvido.
2. Verificar o endereço IP de origem, se disponível.
3. Conferir se o login bem-sucedido ocorreu a partir da mesma origem.
4. Verificar o horário, o equipamento e outros eventos relacionados.
5. Investigar se houve criação de usuários, elevação de privilégios ou execução de processos suspeitos.
6. Registrar as evidências e escalar o caso conforme os procedimentos da equipe.

## 5. Classificação inicial

**Status:** atividade suspeita em investigação.

**Prioridade:** depende do contexto, da origem do acesso e dos eventos correlacionados.

## 6. Conclusão

As falhas de autenticação seguidas de sucesso justificam uma investigação adicional. É necessário correlacionar os registros antes de concluir se houve comprometimento da conta.

## 7. Tipo de atividade

Exercício simulado para fins de estudo de SOC N1. Os horários e eventos são fictícios.
