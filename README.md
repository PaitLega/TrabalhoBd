# TRABALHO 01:  Título do Trabalho
Trabalho desenvolvido durante a disciplina de BD1

# Sumário

### 1. COMPONENTES<br>
Integrantes do grupo<br>
Luiz Eduardo Gagno Amancio: luizgagnoamancio@gmail.com<br>
Rafael Xavier Braga: rafaelxavierbraga@gmail.com<br>
Rita da Silva Alves Guimarães: ritaalvesguimaraes@gmail.com<br>
...<br>

### 2.INTRODUÇÃO E MOTIVAÇÃO<br>
Este documento contém a especificação do projeto do banco de dados <Organize> <br>e motivação da escolha realizada. <br>

> O sistema "Organize" visa auxiliar seus usuários a terem um maior controle e organização de sua vida financeira, possibilitando uma melhor gerência sobre suas despesas e receitas com objetivo de uma vida com menos inadimplência, mais planejamento e consequentemente melhor qualidade de vida. Saber o quanto ganha e quais seus gastos facilita na administração das finanças de todos, muita das vezes não é uma renda que não é suficiente e sim uma renda que está sendo mal administrada por falta de uma melhor organização e certo desconhecimento sobre a destinação de seu dinheiro. Diante disso surgiu o interesse em desenvolver o sistema "organize" visando unir as informações relativas à todas as receitas e despesas em uma única ferramenta, com consulta de fácil acesso, em um mesmo local e sempre à mão, com o intuito de gerar relatórios e informar seus usuários quais valores o mesmo obteve como receita e quais foram suas destinações.

 

### 3.MINI-MUNDO<br>

>O sistema “Organize” conterá as informações aqui detalhadas. Da pessoa deverá ser armazenado o nome, cpf, data de nascimento, senha e contato, seja ele e-mail ou telefone. 
Do endereço serão armazenados descrição logradouro, logradouro, número, bairro, município, cep e estado. Cada pessoa deve possuir pelo menos um contato e pelo menos um endereço. 
Em relação às transações serão armazenados: tipo, descrição, valor, data da operação e o código. Os dados relativos ao tipo deverão possuir código e descrição do tipo de transação. 
É importante destacar que cada pessoa pode possuir nenhuma ou várias transações, mas uma transação está associada apenas a uma única  pessoa. Em relação ao tipo de transação vale ressaltar que cada tipo pode ou não está associado a uma transação, mas cada transação deve possuir um tipo. 

 


### 4.PROTOTIPAÇÃO, PERGUNTAS A SEREM RESPONDIDAS E TABELA DE DADOS<br>
#### 4.1 RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
Neste ponto a codificação não e necessária, somente as ideias de telas devem ser criadas, o princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>

![Alt text](https://github.com/discipbd1/trab01/blob/master/balsamiq.png?raw=true "Title")
![Arquivo PDF do Protótipo Balsamiq feito para Empresa Devcom](https://github.com/discipbd1/trab01/blob/master/arquivos/EmpresaDevcom.pdf?raw=true "Empresa Devcom")

![Arquivo PDF do Protótipo Balsamiq feito para o Sistema Organize](https://github.com/PaitLega/TrabalhoBd/blob/master/Prototipo%20-%20Luiz%20Gagno%2C%20Rafael%20Xavier%20e%20Rita%20Guimaraes.pdf?raw=true "Sistema 
Organize")

#### 4.2 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    a) O sistema proposto poderá fornecer quais tipos de relatórios e informaçes? 
    b) Crie uma lista com os 5 principais relatórios que poderão ser obtidos por meio do sistema proposto!
    
> A Empresa DevCom precisa inicialmente dos seguintes relatórios:
* Relatório que mostre o nome de cada supervisor(a) e a quantidade de empregados supervisionados.
* Relatório relativo aos os supervisores e supervisionados. O resultado deve conter o nome do supervisor e nome do supervisionado além da quantidade total de horas que cada supervisionado tem alocada aos projetos existentes na empresa.
* Relatorio que mostre para cada linha obtida o nome do departamento, o valor individual de cada salario existente no  departamento e a média geral de salarios dentre todos os empregados. Os resultados devem ser apresentados ordenados por departamento.
* Relatório que mostre as informações relacionadas a todos empregados de empresa (sem excluir ninguém). As linhas resultantes devem conter informações sobre: rg, nome, salario do empregado, data de início do salario atual, nomes dos projetos que participa, quantidade de horas e localização nos referidos projetos, numero e nome dos departamentos aos quais está alocado, informações do historico de salário como inicio, fim, e valores de salarios antigos que foram inclusos na referida tabela (caso possuam informações na mesma), além de todas informações relativas aos dependentes. 
>> ##### Observações: <br> a) perceba que este relatório pode conter linhas com alguns dados repetidos (mas não todos). <br>  b) para os empregados que não possuirem alguma destas informações o valor no registro deve aparecer sem informação/nulo. 
* Relatório que obtenha a frequencia absoluta e frequencia relativa da quantidade de cpfs únicos no relatório anterior. Apresente os resultados ordenados de forma decrescente pela frequencia relativa.

 
 
#### 4.3 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    
![Exemplo de Tabela de dados da Empresa Devcom](https://github.com/discipbd1/trab01/blob/master/arquivos/TabelaEmpresaDevCom_sample.xlsx?raw=true "Tabela - Empresa Devcom")
![Tabela de dados do Sistema Organize](https://github.com/PaitLega/TrabalhoBd/blob/master/TabelaSistemaOrganize.xlsx?raw=true "Tabela - Sitema Organize")    
    
### 5.MODELO CONCEITUAL<br>
    A) Utilizar a Notação adequada (Preferencialmente utilizar o BR Modelo 3)
    B) O mínimo de entidades do modelo conceitual pare este trabalho será igual a 3 e o Máximo 5.
        * informe quais são as 3 principais entidades do sistema em densenvolvimento<br>(se houverem mais de 3 entidades, pense na importância da entidade para o sistema)       
    C) Principais fluxos de informação/entidades do sistema (mínimo 3). <br>Dica: normalmente estes fluxos estão associados as tabelas que conterão maior quantidade de dados 
    D) Qualidade e Clareza
        Garantir que a semântica dos atributos seja clara no esquema (nomes coerentes com os dados).
        Criar o esquema de forma a garantir a redução de informação redundante, possibilidade de valores null, 
        e tuplas falsas (Aplicar os conceitos de normalização abordados).   
        
![Alt text](https://github.com/discipbd1/trab01/blob/master/images/concept_sample.png?raw=true "Modelo Conceitual")
    
    
        
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]

#### 5.2 Descrição dos dados 
    PESSOA: Tabela que armazena as informações relativas a pessoa cliente da empresa.
    cpf: Campo que armazena o número de Cadastro de Pessoa Física para cada pessoa cliente da empresa.
    nome: Campo que armazena o nome de cada pessoa cliente da empresa.
    data_nascimento: Campo que armazena a data de nascimento de cada pessoa cliente da empresa.
    senha: Campo que armazena a senha de acesso de cada pessoa cliente da empresa.
    CONTATO: Tabela que armazena as informações relativas ao contato de uma pessoa cliente da empresa
    cod_contato: Campo que armazena o codigo do contato para cada pessoa cliente da empresa.
    contato: Campo que armazena qual o meio de contato para cada pessoa cliente da empresa.
    TRANSACAO: Tabela que armazena transações efetuadas pela pessoa cliente da empresa.
    cod_transacao: Campo que armazena o codigo da transação feita pela pessoa cliente da empresa.
    descricao_transacao: Campo que armazena a descrição da transação dada pela pessoa cliente da empresa.
    data_operacao: Campo que armazena a data que foi feita a transação pela pessoa cliente da empresa.
    valor: Campo que armazena o valor da transação feita pela pessoa cliente da empresa.
    TIPO: Tabela que armazena os tipos de operações possiveis para as transações.
    cod_tipo: Campo que armezena o codigo do tipo da transação.
    descricao_tipo: Campo que armazena qual o tipo da transação.
    ENDERECO: Tabela que armazena o endereço de cada pessoa cliente da empresa.
    descricao_logradouro: Campo que armazena a descrição do logradouro residencial.
    logradouro: Campo que armazena o logradouro residencial.
    numero: Campo que armazena o número residencial.
    bairro: Campo que armazena o bairro residencial.
    municipio: Campo que armazena o municipio residencial.
    cep: Campo que armazena o CEP residencial.
    estado: Campo que armazena o estado residencial.


### 6	MODELO LÓGICO<br>
        a) inclusão do esquema lógico do banco de dados
        b) verificação de correspondencia com o modelo conceitual 
        (não serão aceitos modelos que não estejam em conformidade)

### 7	MODELO FÍSICO<br>
        a) inclusão das instruções de criacão das estruturas em SQL/DDL 
        (criação de tabelas, alterações, etc..)
create table TIPO(cod_tipo int,descricao_tipo varchar(100),primary key (cod_tipo));

INSERT INTO TIPO values(1,'Saque'),(2,'Despesa'),(3,'Investimento'),(4,'Receita'),(5,'Depósito');

create table PESSOA(cpf bigint,nome varchar(100),data_nascimento date,senha varchar(100),primary key (cpf));
INSERT INTO PESSOA values(10104361234,'Ana Gomes','1995/01/11','123456'),(12945630790,'Sofia Salles','2000/04/22','675893'),(47345893011,'Fabio Nunes','1998/10/30','174524'),(58457731459,'João Almeida','1970/07/15','Joao123');

create table CONTATO(cpf_pessoa bigint,contato varchar(100),foreign key (cpf_pessoa) references PESSOA (cpf));
INSERT INTO CONTATO values(10104361234,'anagomes@gmail.com'),(10104361234,'27997648129'),(47345893011,'27998524459'),(47345893011,'fNunes@gmail.com'),(12945630790,'27998562473'),(58457731459,'JAlmeida@gmail.com');

create table ENDERECO(cpf_pessoa bigint,logradouro varchar(100),descricao_logradouro varchar(100),numero int,bairro varchar(100),municipio varchar(100),cep int,estado char(2),foreign key (cpf_pessoa) references PESSOA(cpf));
INSERT INTO ENDERECO values (10104361234,'Rua','Sabino Alves', 1122, 'Feu Rosa', 'Serra',29100200, 'ES'),(12945630790,'Avenida', 'Pedro Nolasco', 1123, 'Colina da Serra', 'Serra' ,29100201, 'ES'),(47345893011,'Rua', 'Beija Flor', 67, 'Laranjeiras', 'São Paulo',29100202, 'SP'),(58457731459,'Rua', 'Herman Stern', 235, 'Jacaraipe', 'Serra',29100203, 'ES');

create table TRANSACAO(cod_transacao int,cpf_pessoa bigint,tipo int,descricao varchar(100),data_operacao date,valor float,primary key (cod_transacao), foreign key (cpf_pessoa) references PESSOA (cpf),foreign key (tipo) references TIPO(cod_tipo));
INSERT INTO TRANSACAO values(1000,47345893011,4,'salario','2020/07/01',14500.00),(1102,10104361234,4,'recebimento aluguel','2020/07/05',2224.00),(1006,12945630790,2,'pagamento IPVA','2020/07/08',803.00),(1010,47345893011,2,'pagamento cartao de crédito','2020/07/10',6125.00),(1132,47345893011,3,'tesouro direto','2020/01/11',5000.00),(1360,47345893011,3,'bolsa de valores','2020/06/11',3000.00),(1456,58457731459,5,'poupança Itaú','2020/07/14',2500.00),(1589,12945630790,5,'poupança Caixa','2020/07/15',1500.00);

        
       
### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
        a) inclusão das instruções de inserção dos dados nas tabelas criadas pelo script de modelo físico
        (Drop para exclusão de tabelas + create definição de para tabelas e estruturas de dados + insert para dados a serem inseridos)
        b) Criar um novo banco de dados para testar a restauracao 
        (em caso de falha na restauração o grupo não pontuará neste quesito)
        c) formato .SQL


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>

># Marco de Entrega 01: Do item 1 até o item 9.1<br>

#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>
#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas

#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.

#### 9.5	INSTRUÇÕES APLICANDO ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>
    a) Criar minimo 3 de exclusão
    b) Criar minimo 3 de atualização

#### 9.6	CONSULTAS COM INNER JOIN E ORDER BY (Mínimo 6)<br>
    a) Uma junção que envolva todas as tabelas possuindo no mínimo 2 registros no resultado
    b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho

#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>
    a) Criar minimo 2 envolvendo algum tipo de junção

#### 9.8	CONSULTAS COM LEFT, RIGHT E FULL JOIN (Mínimo 4)<br>
    a) Criar minimo 1 de cada tipo

#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join (caso não ocorra na base justificar e substituir por uma view)
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho

#### 9.10	SUBCONSULTAS (Mínimo 4)<br>
     a) Criar minimo 1 envolvendo GROUP BY
     b) Criar minimo 1 envolvendo algum tipo de junção

># Marco de Entrega 02: Do item 9.2 até o ítem 9.10<br>

### 10 RELATÓRIOS E GRÁFICOS

#### a) análises e resultados provenientes do banco de dados desenvolvido (usar modelo disponível)
#### b) link com exemplo de relatórios será disponiblizado pelo professor no AVA
#### OBS: Esta é uma atividade de grande relevância no contexto do trabalho. Mantenha o foco nos 5 principais relatórios/resultados visando obter o melhor resultado possível.

    

### 11	AJUSTES DA DOCUMENTAÇÃO, CRIAÇÃO DOS SLIDES E VÍDEO PARA APRESENTAÇAO FINAL <br>

#### a) Modelo (pecha kucha)<br>
#### b) Tempo de apresentação 6:40 

># Marco de Entrega 03: Itens 10 e 11<br>
<br>
<br>
<br> 



### 12 FORMATACAO NO GIT:<br> 
https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
    
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/
#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

    
### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. <strong>Caso existam arquivos com conteúdos sigilosos<strong>, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário do git "profmoisesomena", para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://www.sis4.com/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")


