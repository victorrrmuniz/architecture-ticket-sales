
O processo de venda de ingressos precisa garantir a integridade da venda para que transações não sejam realizadas sem que haja ingressos disponíveis.

Como esse tipo de operação demanda milhares de usuário tentando acessar o site ao mesmo tempo. É necessário que haja uma fila para a entrada dos usuários
onde é distribuida uma senha aleatória na fila a partir de determinado horário e dali em diante, a entrada é por ordem de chegada garantindo que o site não
se sobrecarregue. Também dessa forma, é garantido que qualquer pessoa acessando qualquer dispositivo terá a mesma chance de conseguir o ingresso.

É possível também implementar um sistema de sessão única, garantindo que uma mesma pessoa não entrará na fila por diversos dispositivos ou browsers ao mesmo tempo
engargalando ainda mais o sistema.

Após isso, quando o usuário consegue entrar na lista de ingressos disponíveis, é possível fazer o travamento desse ingresso por algum tempo pré-definido, assim
garantindo que o usuário não fará todo o processo para no final descobrir que os ingressos se esgotaram.

Na parte do pagamento, o serviço deve ser lockado e a transação só realmente poderá ser finalizada quando estiver garantido que existem ingressos disponíveis
