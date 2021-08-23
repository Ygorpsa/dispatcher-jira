# dispatcher-jira
API para fazer o dispatcher do Jira


DOCUMENTAÇÃO DO JIRA -DISPACHER:

Foram importados os pacotes: 

Fmt: Biblioteca de entrada e saída de dados do golang
Encoding/base 64: https://pkg.go.dev/encoding/base64
Encoding/json: O pacote json implementa codificação e decodificação de JSON conforme definido na RFC 7159. O mapeamento entre os valores JSON e Go está descrito na documentação para as funções Marshal e Unmarshal.
json · codificação/json · pkg.go.dev
log: O registro do pacote implementa um pacote de registro simples. Define um tipo, Logger, com métodos para formatação de saída. Ele também tem um Logger 'padrão' pré-definido acessível através das funções de ajudante Print[f|ln], Fatal[f|ln], e Panic[f|ln], que são mais fáceis de usar do que criar um Logger manualmente. Esse madeireiro escreve para erro padrão e imprime a data e a hora de cada mensagem registrada. Cada mensagem de registro é saída em uma linha separada: se a mensagem que está sendo impressa não terminar em uma linha nova, o madeireiro adicionará uma. As funções fatais chamam os. Sair(1) após escrever a mensagem de registro. As funções do Pânico chamam de pânico depois de escrever a mensagem de registro.
https://pkg.go.dev/log

"net/http: O pacote http fornece implementações de clientes e servidores HTTP.
Get, Head, Post, and PostForm make HTTP (or HTTPS) requests:
https://pkg.go.dev/net/http

“OS”: O sistema operacional de pacotes fornece uma interface independentemente da plataforma para a funcionalidade do sistema operacional. O design é semelhante ao Unix, embora o tratamento de erros seja semelhante ao Go-like; falha chamadas valores de retorno de erro de tipo em vez de números de erro. Muitas vezes, mais informações estão disponíveis dentro do erro. Por exemplo, se uma chamada que leva um nome de arquivo falhar, como abrir ou Stat, o erro incluirá o nome do arquivo que falha quando impresso e será do tipo *PathError, que pode ser desembalado para obter mais informações.
A interface do sistema operacional destina-se a ser uniforme em todos os sistemas operacionais. Os recursos não disponíveis geralmente aparecem na chamada de pacote específica do sistema.
os · os · pkg.go.dev


Basicamente a função principal do código é entrar no jira e enviar os dados para plataforma via as regras Json.

