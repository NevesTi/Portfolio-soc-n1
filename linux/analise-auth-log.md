# Análise de Logs de Autenticação Linux

## Objetivo

Praticar a consulta e interpretação de registros de autenticação em um ambiente Ubuntu.

## Ambiente

- Sistema operacional: Ubuntu Linux.
- Arquivo consultado: `/var/log/auth.log`.
- Ferramentas utilizadas: `sudo`, `grep` e `tail`.

## Atividade realizada

Foi executada uma pesquisa por mensagens relacionadas a falhas de autenticação:

```bash
sudo grep -i "failed password" /var/log/auth.log | tail -n 10
```

## Resultado observado

A saída apresentou dois registros relacionados à execução de comandos `sudo grep` pelo usuário local. Esses registros documentam a consulta ao arquivo de autenticação; não comprovam tentativas de invasão.

## Interpretação

A pesquisa inicial não apresentou, na saída compartilhada, registros explícitos de `Failed password`, `authentication failure` ou `invalid user`. Portanto, não é possível concluir, apenas com esse resultado, que houve ou não atividade maliciosa.

## Próximo passo da investigação

Executar uma pesquisa direcionada a diferentes mensagens de falha de autenticação e verificar se existem eventos relevantes no período analisado.

## Tipo de atividade

Prática realizada em laboratório próprio para fins de aprendizado de SOC N1.
