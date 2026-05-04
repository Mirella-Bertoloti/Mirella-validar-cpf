Validador de CPF em Java

Este projeto é um programa simples em Java que realiza a validação de um CPF (Cadastro de Pessoas Físicas) com base no cálculo dos dígitos verificadores.
Funcionalidade

O programa:
Solicita ao usuário que digite um CPF
Calcula os dígitos verificadores com base nos primeiros números
Informa se o CPF é válido ou inválido

Lógica de Validação:
O CPF possui 11 dígitos, sendo os dois últimos verificadores. O algoritmo realiza:
Cálculo do primeiro dígito verificador:
Multiplica os 9 primeiros dígitos por pesos decrescentes de 10 a 2
Soma os resultados
Aplica a fórmula: 11 - (soma % 11)
Se o resultado for maior ou igual a 10, considera 0
Cálculo do segundo dígito verificador:
Multiplica os 10 primeiros dígitos por pesos de 11 a 2
Repete o mesmo processo do primeiro dígito
Compara os dígitos calculados com os informados no CPF

Observações:
O código não verifica se o CPF possui caracteres inválidos (como letras ou símbolos)
Não trata CPFs com formatação (ex: 123.456.789-09)
Recomenda-se validar o tamanho da string e limpar caracteres não numéricos antes da validação

Melhorias Futuras:
Remover caracteres não numéricos automaticamente
Validar tamanho do CPF
Rejeitar CPFs com todos os dígitos iguais (ex: 11111111111)
Criar interface gráfica ou API para integração
