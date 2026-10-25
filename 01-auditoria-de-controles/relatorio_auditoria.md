Relatório de Auditoria — FIN-SRV01

Tipo: Atividade acadêmica de Auditoria Forense de Sistemas Digitais
Ambiente: Simulação de servidor financeiro

Objetivo

Identificar possíveis falhas de segurança na configuração de contas e permissões de arquivos.

Verificações realizadas

1. Contas com UID 0

root — UID 0

suporte — UID 0

Resultado: a conta suporte possui privilégio máximo indevido segundo os critérios da atividade.

2. Conta sem senha

suporte

Resultado: a conta aparece sem senha configurada no arquivo simulado.

3. Permissão de escrita

saida/servidor/financeiro/pagamentos.csv

Resultado: o arquivo permite escrita para outros usuários.

4. Conta de funcionário desligado

estagiario2024

Resultado: a conta permanece na configuração simulada, embora a descrição indique desligamento em 2024.

Recomendações

Restringir o UID 0 à conta root.

Configurar autenticação adequada para a conta de suporte.

Corrigir as permissões do arquivo financeiro.

Revisar e desativar contas de funcionários desligados.

Integridade da evidência

Hash SHA-256 do relatório gerado no ambiente de auditoria:

4430b77ab3fbef5408733319d3ecefd49c75566005d32a1fdc47b3ca850718ef

Observação: atividade realizada em ambiente simulado para fins educacionais. 
