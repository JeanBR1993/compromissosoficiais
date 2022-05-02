# compromissosoficiais PT-BR
Web Scrapper + análise de dados dos compromissos oficiais presidenciais</br></br>
Esse código tem o intuito de extrair dados pertinentes à compromissos oficiais do presidente brasileiro desde 01/01/2019 à 19/04/2022, tais valores podem ser mudados alterando as variáveis 'diainicio' e 'diafinal'.</br>
A página a qual utilizei como base é 'https://www.gov.br/planalto/pt-br/acompanhe-o-planalto/agenda-do-presidente-da-republica/', se tal página mudar de endereço é só mudar a variável 'url' no loop.</br>
O WebScrapper foi escrito para determinada estrutura de página, é um projeto altamente customizado, se a página mudar de estrutura ele parará de funcionar.</br>
O algoritmo extrai dados de data, horário e descrição do compromisso, guardadas nas variáveis do tipo lista 'data', 'horario', 'descricao'.</br>
Após isso descobri que alguns dias não conseguem ser extraídos por mudança na estrutura da página, são adicionados valores estimados para cada dia faltante.</br>
São tratados os dados usando-se a library pandas até se chegar em três valores: média com todos os dias, média sem o domingo, média sem sábado e domingo.</br>
Depois são plotados os valores em um gráfico de barras para melhor visualização gráfica.</br></br>


# compromissosoficiais EN-US
Web scrapper + official presidential appointments data analysis</br></br>
This code has the intention of extracting data from Brazilian official presidential appointments from 2019/01/01 to 2019/04/19, those value can be changed if you change the 'diainicio' e 'diafinal' variables.</br>
The webpage which I used as basis is 'https://www.gov.br/planalto/pt-br/acompanhe-o-planalto/agenda-do-presidente-da-republica/', if the address change you have to alter 'url' variable inside the loop.</br>
The Web scrapper has been coded with the determined structure of that webpage, it's a highly customized project, if the page's structure change it'll cease to function properly.</br>
The algorithm extract dates, schedule and description data, stored in list type variables 'data', 'horario', 'descricao'.</br>
After that I discovered that some days couldn't be extracted because of changes in page's structure, estimated values are added for every missing day.</br>
The pandas library is used for the data wrangling until the calculation of three variables: Average 7-day Week, Average 6-day Week, Average 5-day Week.</br>
And for the finish the last variables are plotted into a bar chart to improve graphic visualization.</br>
