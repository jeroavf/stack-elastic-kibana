# stack-elastic-kibana
Atencao para o erro que acontece na subida do docker-compose: O elastic emite o erro  "max virtual memory areas vm.max_map_count [65530] is too low, increase to at least [262144]". O elastic não sobe e kibana tambem nao . A mensagem de erro aparece no meio do monte de log gerado na subida do stack 

Solução para S.O. Linux:
sudo sysctl -w vm.max_map_count=262144
