# PI_SENAC

**Projeto Gestão de Dados**

## RESUMO 

O propósito deste projeto é desenvolver um modelo lógico de um Sistema Orientado a Objetos destinado a representar a gestão de uma escola. A linguagem de modelagem unificada (UML) oferece diversos tipos de diagramas, como os de casos de uso, de classes e de sequência, cada um focalizando um aspecto diferente do sistema. Foram elaborados e detalhados os diagramas de casos de uso e de classes da UML. Esses diagramas facilitam a comunicação e compreensão entre os membros da equipe, permitindo-lhes visualizar claramente a estrutura, o comportamento e as interações do sistema. Ao seguir as diretrizes da UML, podemos colaborar de maneira mais eficiente, garantindo que todos tenham uma compreensão compartilhada do software em desenvolvimento, além de facilitar a manutenção e a evolução contínua do sistema ao longo do tempo.
       
## INTRODUÇÃO

O Unified Modeling Language (UML) é uma linguagem de modelagem que tem como objetivo padronizar a representação de projetos de software, facilitando assim a visualização, compreensão e colaboração entre os membros da equipe. É utilizada para especificar, documentar e facilitar processos de visualização lógica de sistemas de informação. A UML oferece uma variedade de diagramas que abrangem diferentes aspectos do desenvolvimento de software, como estrutura, comportamento, interação, processo e distribuição. A padronização promovida pela UML facilita a compreensão e a colaboração, proporcionando uma linguagem comum para expressar ideias e conceitos relevantes para o sistema em desenvolvimento. Além disso, a UML desempenha um papel crucial na documentação de sistemas de software, garantindo que o conhecimento crítico seja capturado e preservado ao longo do tempo. Sua versatilidade a torna amplamente adotada na indústria de software e é ensinada em cursos de engenharia de software e ciência da computação em todo o mundo. O uso eficaz da UML pode resultar em uma melhor compreensão dos requisitos do sistema, projetos mais robustos e uma comunicação mais eficaz entre os membros da equipe, contribuindo para sistemas de software de maior qualidade. Este método foi empregado no presente trabalho.

**DIAGRAMA DE CASO DE USO**

![Imagem1](https://github.com/Rcffeitosa/PT---SENAC-2024/assets/132168781/456fc270-848e-4a23-98ae-508647c50010)

## Caso de Uso: Acessar sistema

- **Atores:** Professor, Aluno e Fornecedor
- **Pré-Condição:** Estar cadastrado no sistema da universidade
- **Cenário Principal:**
  1. O Professor, Aluno ou Fornecedor acessa o sistema.
  2. Seleciona a opção “Acessar”.
  3. Informa os dados para login.
  4. O sistema realiza a autenticação.
  5. O acesso do ator é liberado.
- **Cenário Alternativo 1:** Login Inválido.
- **Cenário Alternativo 2:** Ator sem cadastro.
- **Pós-Condição:** O ator acessa o seu perfil dentro do sistema da universidade.

## Caso de Uso: Criar cadastro de aluno

- **Atores:** Fornecedor
- **Pré-Condição:** O Fornecedor deve estar identificado e autenticado
- **Cenário Principal:**
  1. O Fornecedor efetua o login no sistema da universidade.
  2. O Fornecedor seleciona a opção “Cadastrar Aluno” no sistema da universidade.
  3. O Fornecedor informa ao sistema os dados do Aluno a ser cadastrado.
  4. O sistema efetua a validação dos dados do Aluno.
  5. O sistema confirma a inclusão do Aluno.
- **Cenário Alternativo 1:** Dados inválidos.
- **Cenário Alternativo 2:** Cadastro já existente.
- **Pós-Condição:** O sistema exibe uma mensagem “Dados inseridos com sucesso”.

- # Caso de Uso: Registrar Nota
- **Atores:** Professor
- **Pré-Condição:** Estar cadastrado no sistema da universidade
## Cenário Principal:
1. O Professor efetua o login no sistema da universidade usando suas credenciais fornecidas pela instituição.
2. O Professor seleciona a opção “Registrar Nota”.
3. O sistema exibe as turmas e disciplinas vinculadas ao Professor.
4. O Professor seleciona a turma e a disciplina para registrar a nota.
5. O sistema exibe a lista de Alunos matriculados na turma selecionada.
6. O Professor seleciona o Aluno que deseja incluir as notas.
7. O Professor insere as notas e os itens de avaliação (trabalhos, participação, etc.) diretamente em campos de entrada designado para o Aluno específico.
8. O sistema verifica se as notas inseridas estão dentro das faixas predefinidas. Por exemplo, se uma determinada avaliação tem um valor máximo de 10 pontos, o sistema verifica se a nota inserida está entre 0 e 10.
9. O sistema confirma a inclusão da nota do Aluno.
10. O sistema atualiza as médias de acordo com as fórmulas de cálculo estabelecidas.
11. O sistema exibe a mensagem “Nota registrada com sucesso”.
## Cenário Alternativo 1: Nota incorreta.
- **Passos:**
  1. O sistema exibe uma mensagem de erro dizendo que as notas registradas estão fora do limite permitido.
  2. O Professor é direcionado para o passo 7, para informar os dados das notas corretos.
## Cenário Alternativo 2: Problema técnico.
- **Passos:**
  1. O sistema exibe a mensagem “Alerta, Alunos não localizados”.
  2. O Professor deverá entrar em contato com o Fornecedor.
- **Pós-Condição:** As notas do aluno selecionado são inseridas e devidamente registradas no sistema.

# Caso de Uso: Visualizar boletim
- **Atores:** Aluno
- **Pré-Condição:** Estar cadastrado no sistema da universidade
## Cenário Principal:
1. O Aluno efetua o login no sistema da universidade usando seus dados.
2. O Aluno seleciona a opção “Boletim”.
3. O sistema disponibiliza o quadro de notas contendo a soma das atividades e provas efetuadas do Aluno.
## Cenário Alternativo 1: Erro no sistema.
- **Passos:**
  1. O sistema exibe uma mensagem “Erro no sistema”.
  2. O Aluno deverá contatar o suporte técnico.
## Cenário Alternativo 2: Boletim indisponível.
- **Passos:**
  1. O sistema exibe uma mensagem de “Boletim indisponível”.
  2. O Aluno deverá aguardar até que seja realizada o lançamento das notas em seu boletim.
- **Pós-Condição:** O Aluno tem acesso ao seu boletim dentro do sistema da universidade.

# Caso de Uso: Realizar avaliação
- **Atores:** Aluno
- **Pré-Condição:** Estar cadastrado no sistema da universidade
## Cenário Principal:
1. O Aluno realiza seu login no sistema inserindo seus dados.
2. Seleciona a opção “Ambiente de Avaliação”.
3. O sistema disponibiliza as disciplinas que o Aluno deverá realizar a prova.
4. O Aluno escolhe a disciplina que vai realizar a prova.
5. O sistema exibe o formulário com as questões.
6. O Aluno responde as questões e ao terminar a prova deverá selecionar “Enviar”.
7. O sistema exibe a mensagem “Prova enviada com sucesso”.
8. O sistema disponibilizará a avaliação para o Professor responsável da disciplina.
## Cenário Alternativo 1: Avaliação Indisponível.
- **Passos:**
  1. O sistema exibe uma mensagem de “Prova indisponível”.
  2. O Aluno deverá contatar o Fornecedor o mais rápido possível.
## Cenário Alternativo 2: Avaliação já realizada.
- **Passos:**
  1. O sistema exibe uma mensagem de “Prova realizada”.
  2. O Aluno deverá selecionar a opção “Sair”, pois já efetuou todas as avaliações.
- **Pós-Condição:** O Aluno realiza sua avaliação com sucesso efetuando seu envio.

## DIAGRAMA DE CLASSE 

 **Diagrama de classe de um sistema de gestão escolar**

![Imagem2](https://github.com/Rcffeitosa/PT---SENAC-2024/assets/132168781/c62fa9ea-1bf8-4aa2-b51e-164a776380e5)


## Desenvolvendo um protótipo, usando ferramentas Figma.

<https://www.figma.com/file/TLXGpdSqQkhV9YYFzzLsW8/PI?type=design&node-id=0-1&mode=design&t=uNidKebjWTLqv90r-0)>

![PI](https://github.com/Rcffeitosa/PI_SENAC-/assets/132168781/b71281e4-bbbd-4328-9a2a-3d5714fe55fb)



