# automacao
Repositório para lancamento automático de dados no diario escolar. diario escolar usado para lancamento de aulas lecionadas e notas

    www.diarioescolardigital.educacao.mg.gov.br/

Diario escolar usado por professores para lancamento de aulas lecionadas e notas de alunos da rede estadual de ensino de Minas Gerais, aulas e conteudos pela secretaria de estado e educação do estado de minas gerais.
Bot criado para Diário Escolar Digital - DED | Versão: 4.3.152.
O bot transforma o diario escolar digital que atualmente é formado por varios formulário, um para cada dia de aula, em uma planilha de excel.
É extremamente mais facil lançar os dados necessarios em uma planilha do que em um formulário.

A parte feita inicialmente foi do lancamento de aulas. FEITO

Nas proximas etapas do projeto a automação lancará as notas em seguida tentarei automatirar o lancamento de faltas dos alunos.
  Etapa 1: lancamento de aulas.
  Etapa 2: lancamento de atividades avaliativas.
  Etapa 3: lancamento de faltas.

Com a comclusao da etapa 1 o professor já tera em maos o diário com todas as aulas lançadas.

Como usar o Bot:
  Instalar as bibliotecas necessárias:
    -pandas
    -selenium
    -time
    
  Instalar o geckodriver:
    deve ser colocado no computador o geckodriver esse arquivo permite que o selenium abra o navegador. (é necessario saber qual versão do navegador será usado)
        Futuramente pretendo colocar um texto e um zip, para ajudar a instalaçao desse drive, no zip haverá varios drivers para varios navegadores e versoes.
        No link abaixo tem alguns drives necessarios para utilizacao do google chrome.
        
        https://chromedriver.chromium.org/home
        
  Atualizar a planilha Diario.xlsx:
    a planilha deve ter os dados na mesma forma que é esperada pelo diário.
    
      exemplo:
      
        Turma	                             Disciplina	                     EtapadaMatrícula	  Bimestre          Data	                  ConteudoLecionado	
        2º EM REG 1 - (NOMEDAESCOLA), 888	 (2º) FÍSICA - 2º EM REG 1	     2º	                2º BIMESTRE	      25/05/2022	            física térmica 
        
        No exemplo acima seria lançado uma aula no segundo bimestre, dia: 25/05/2022, para a turma: 2° reg 1, com conteudo: física térmica.
     
 
  Rodar o código:
    Ao rodar o códido abrirá uma página do navegador no site do diário.
    voce deve colocar seu login, senha e captcha.
    Nao click em entrar, volte ao codigo e responda a pergunta com apenas um s
      O bot escreverá a seginte frase: 
                                        "digite  s  ao terminar: " s
    após confirmar que concluiu o preenchimento das informaçoes para login o bot perguntará se quer lançar aulas de novo ensino medio:
      O bot escreverá a seginte frase:  
                                         "quer lancar aulas no novo ensino medio? 
                                          se sim entao responda com s 
                                          caso contrario responda com n"
      Para resonder lembre-se que será usado as informacoes que foram colocadas na planilha "diario.xlsx"
      responda com s para novo ensino medio e n para ensino medio 
        (O bot foi criado em 2022 as as turmas de 1° ano estavam no novo ensino medio, turmas de 2° e 3° ainda cumpriam o curriculo antigo.)
      Após responder com s ou n basta esperar. 
      Ao final aparecerá a mensagem FEITO!!!
                                                                                               Alex Furtado Vilela Costa - Professor de física  
    
    
    
