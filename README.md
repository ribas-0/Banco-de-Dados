# Banco-de-Dados

Estrutura do Banco de Dados
Tabelas
PROFESSORES: Armazena informações sobre os professores (ID, nome).
TURMAS: Armazena informações sobre as turmas (ID, nome da turma, ID do professor).
DISCIPLINAS: Armazena informações sobre as disciplinas (ID, nome, ID do professor).
ALUNOS: Armazena informações sobre os alunos (ID, nome, data de nascimento).
MATRICULAS: Armazena as matrículas dos alunos nas disciplinas e turmas (ID, aluno, disciplina, turma, nota).
Pacotes PL/SQL
PKG_PROFESSOR: Contém funções para obter o total de turmas por professor, o total de turmas de um professor específico e o nome do professor associado a uma disciplina.
PKG_ALUNO: Contém procedimentos para excluir alunos e cursos (ALUNOS_MAIORES_18, ALUNOS_POR_CURSO), e ações relacionadas ao gerenciamento de alunos.
PKG_DISCIPLINA: Contém procedimentos para cadastrar disciplinas, listar alunos de uma disciplina, calcular a média de idade dos alunos de uma disciplina e consultar o total de alunos por disciplina.
Funcionalidades
PKG_PROFESSOR:

TOTAL_TURMAS_POR_PROFESSOR: Retorna um cursor com o total de turmas para cada professor que leciona mais de uma turma.
TOTAL_TURMAS_PROFESSOR: Retorna o total de turmas de um professor específico.
PROFESSOR_DISCIPLINA: Retorna o nome do professor associado a uma disciplina.
PKG_ALUNO:

EXCLUIR_ALUNO: Exclui um aluno e suas respectivas matrículas.
ALUNOS_MAIORES_18: Cursor que retorna alunos maiores de 18 anos.
ALUNOS_POR_CURSO: Cursor que retorna alunos matriculados em uma disciplina específica.
PKG_DISCIPLINA:

CADASTRAR_DISCIPLINA: Insere uma nova disciplina no banco de dados.
LISTAR_ALUNOS_DISCIPLINA: Exibe a lista de alunos matriculados em uma disciplina específica.
MEDIA_IDADE_DISCIPLINA: Retorna a média de idade dos alunos matriculados em uma disciplina.
TOTAL_ALUNOS_DISCIPLINAS: Cursor que retorna disciplinas com mais de 10 alunos matriculados.
