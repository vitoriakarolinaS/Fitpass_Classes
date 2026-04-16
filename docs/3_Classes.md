***Aluno***
RF01, RF04, RF05, RF06, RF10
- idAluno
- nome
- cpf
- email
- telefone
- endereco
- rfid
- status
- contratarPlano()
- agendarAula()
- cancelarAgendamento()
- atualizarStatus()
- registrarAcesso()
- receberNotificação()

***Plano***
RF01, RF02, RF04
- idPlano
- nome
- tipo
- valor
- ativo
- ativar()
- desativar()
- alterarValor()

***Pagamento***
RF03, RF04, RF09
- idPagamento
- data
- valor
- formaPagamento
- status
- realizar()
- cancelar()
- gerarComprovante()
- consultarStatus()

***Acesso***
RF05, RF09
- idAcesso
- dataHora
- autorizado
- registrarEntrada()
- registrarSaida()
- validarAcesso()
- consultarHistorico()

***Aula***
RF06, RF07, RF09
- idAula
- nome
- horario
- capacidadeMaxima
- cadastrarAula()
- atualizarAula()
- cancelarAula()
- listarAlunos()

***Agendamento***
RF06, RF10
- idAgendamento
- dataReserva
- status
- agendar()
- cancelar()
- reagendar()
- confirmarPresenca()

***Presenca***
RF07
- idPresenca
- data
- presente
- registrarPresenca()
- justificarFalta()
- consultarPresenca()

***AvaliacaoFisica***
RF08, RF10
- idAvaliacao
- data
- peso
- imc
- percentualGordura
- observacoes
- anexo
- registrarAvaliacao()
- atualizarAvaliacao()
- consultarResultados()
- gerarRelatorio()

***Notificacao***
RF10
- idNotificacao
- tipo
- dataEnvio
- status
- mensagem
- enviarNotificacao()
- agendarNotificacao()
- cancelarNotificacao()
- visualizarNotificacao()

***Instrutor***
RF07, RF08
- idInstrutor
- nome
- especialidade
- cadastrarAula()
- registrarPresenca()
- realizarAvaliacao()

***Recepcionista***
RF01, RF03
- idRecepcionista
- nome
- cadastrarAluno()
- registrarPagamento()
- agendarAula()

***Gerente***
RF02, RF09
- idGerente
- nome
- gerarRelatorio()
- gerenciarFuncionarios()
- analisarDesempenho()
