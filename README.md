# Conflitos no Brasil entre 2018 e janeiro de 2023

## A partir do dataset Brazil Conflict Tracker, o objetivo do projeto era visualizar a incidência de conflitos, de cunho violento ou não no Brasil, entre 2018 e 2023.

### O dataset foi extraído do Kaggle feito pelo estudante de Stanford, Justin Oh. Os dados partem da Armed Conflict Location & Event Data Project (ACLED), que coleta, dentre outros, informações sobre eventos de violência, demonstrações de violência e atos politicamente relevantes em uma escala global.

## Estrutura do Dataset

### O dataset é composto por duas tabelas, a primeira foi obtida através do Kaggle. Em relação a segunda, essa foi feita por mim com o intuito de ampliar o escopo da visualização, adicionando o estado no qual do ocorrido, a sua população em 2022 e a  respectiva macrorregião.
### Apesar da maior parte do trabalho de limpeza e transformação estar concluído, para incluir o estado que do conflito e fazer a conexão com a tabela das informações adicionais, foi necessário alterar o dataset original utilizando a biblioteca pandas no python. 
### Devido ao fato de que a grande maioria dos estados estava exposto nas notas (61 mil observações de 62 mil totais), a inclusão de uma nova coluna se deu da seguinte maneira:

![image](https://github.com/user-attachments/assets/7fc97753-014c-40f2-8e1f-fb664708c37a)
### Após o ajuste, o dataset ficou estruturado dessa forma:

![image](https://github.com/user-attachments/assets/c8583a60-5bab-4068-a73a-815b4f3438d0)

