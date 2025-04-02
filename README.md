# Conflitos no Brasil entre 2018 e janeiro de 2023

## A partir do dataset Brazil Conflict Tracker, o objetivo do projeto era visualizar a incidência de conflitos, de cunho violento ou não no Brasil, entre 2018 e 2023.

### O dataset foi extraído do [Kaggle](https://www.kaggle.com/datasets/justin2028/brazil-conflict-tracker-20182023) feito pelo estudante de Stanford, Justin Oh. Os dados partem da Armed Conflict Location & Event Data Project (ACLED), que coleta, dentre outros, informações sobre eventos de violência, demonstrações de violência e atos politicamente relevantes em uma escala global.

## Estrutura do Dataset

### O dataset é composto por duas tabelas, a primeira foi obtida através do Kaggle. Em relação a segunda, essa foi feita por mim com o intuito de ampliar o escopo da visualização, adicionando o estado no qual do ocorrido, a sua população em 2022 e a respectiva macrorregião.
### Apesar da maior parte do trabalho de limpeza e transformação estar concluído, para incluir o estado que do conflito e fazer a conexão com a tabela das informações adicionais, foi necessário alterar o dataset original utilizando a biblioteca Pandas no Python. 
### Devido ao fato de que a grande maioria dos estados estava exposto nas notas (61 mil observações de 62 mil totais), a inclusão de uma nova coluna se deu da seguinte maneira:

![image](https://github.com/user-attachments/assets/7fc97753-014c-40f2-8e1f-fb664708c37a)
### Após o ajuste, o dataset ficou estruturado dessa forma:

![image](https://github.com/user-attachments/assets/a1647e21-16f2-4429-b518-a885b97c4780)

## Dashboards Utilizando o Tableau
### Depois da conexão esbelecida nas tabelas entre as colunas "Brazil_Political_Violence.ESTADO" e "Estados_info.nome". Além disso, foi necessária a criação de uma hierarquia entre a Região, a Unidade Federativa e o tipo de evento.
### O primeiro dashboard consiste em um mapa interativo com dois filtros - um para seperar os tipos de conflitos e o outro para definir o ano -, no canto inferior direito a tabela foi colocada com o intuito de detalhar os eventos por Unidade Federativa. [Clique para visualizar.](https://public.tableau.com/views/MapadeConflitosnoBrasil2018-2023/MapadeConflitosnoBrasil?:language=pt-BR&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

![image](https://github.com/user-attachments/assets/040c23af-19c3-4d32-bc31-9f99194f71b9)

### O segundo dashboard busca expor a evolução de cada tipo de conflito por UF. [Clique para visualizar.](https://public.tableau.com/views/EvoluodosConflitosnoBrasil2018-2022/EvoluodosConflitos2018-2022?:language=pt-BR&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link)

![image](https://github.com/user-attachments/assets/c7d6e1d0-3838-495a-b7d6-8ebb206ae917)

## Conclusões
### • O estado do Rio de Janeiro lidera o país os em número de ocorrências, isso se dá principalmente pelo que a ACLED considera como "Battles" - disputas entre grupos armados entre si ou contra a polícia -.
### • Retirando a batalhas da análise percebe-se que o estado do São Paulo toma a liderança, puxado pelo número de protestos e pela violência contra civis. Nessa linha, o estado do Amazonas também aparece no topo da lista com um número expressivo da violência contra a população.
### • Entretanto, caso analisarmos o número de conflitos por 10 mil habitantes a Região Norte se destaca negativamente e a Região Sul positivamente.
### • Por fim, observando o dashboard de evolução dos tipos de conflitos, percebe-se que dentre os três eventos mais reportados (Batalhas, Protestos e Violência contra Civis), o dois primeiros indicam uma leve queda e, por sua vez, a Violência contra Civis mostra uma tendência de alta. 


