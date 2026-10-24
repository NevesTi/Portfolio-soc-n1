# Análise de Alerta Suspeito — Exercício Simulado

## 1. Objetivo

Praticar a triagem inicial de um alerta de segurança, identificando informações relevantes, possíveis riscos e próximos passos para investigação.

## 2. Cenário

Um sistema de monitoramento (SIEM) identificou conexões repetidas de um computador interno para um endereço IP externo desconhecido, utilizando a porta TCP 443.

## 3. Informações disponíveis

- **Origem:** computador interno.
- **Destino:** endereço IP externo ainda não verificado.
- **Porta de destino:** 443.
- **Protocolo:** TCP.
- **Frequência:** conexões repetidas.
- **Processo responsável:** ainda não identificado.

## 4. Análise inicial

A porta 443 é normalmente utilizada para comunicação HTTPS. Entretanto, seu uso não garante que a conexão seja legítima.

As conexões repetidas justificam uma investigação, mas não comprovam, isoladamente, uma infecção por malware ou comprometimento do computador.

## 5. Próximas ações

1. Identificar o processo responsável pelas conexões.
2. Verificar a reputação e o contexto do endereço IP de destino.
3. Analisar os horários e a frequência das conexões.
4. Correlacionar os eventos com logs do sistema e outros alertas.
5. Registrar as evidências encontradas.
6. Escalonar o caso conforme os procedimentos e as permissões da equipe.

## 6. Conclusão

**Classificação inicial:** evento suspeito que necessita de investigação.

Com as informações disponíveis, não é possível confirmar comprometimento. A decisão final dependerá das evidências coletadas e da correlação com outros eventos.

## 7. Tipo de atividade

Exercício simulado para fins de estudo de SOC N1.
