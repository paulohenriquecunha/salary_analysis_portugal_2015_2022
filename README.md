📊 NOVO DASHBOARD: ANÁLISE DOS SALÁRIOS EM PORTUGAL (2015–2022)

📌 Visão Geral

Este projeto apresenta um dashboard de análise da evolução dos salários em Portugal entre 2015 e 2022.

O objetivo principal não foi produzir um estudo exaustivo, mas praticar ETL real, desenvolver um modelo de dados limpo e criar visualizações profissionais, trabalhando com dados públicos desafiadores — como acontece em muitos projetos reais de análise de dados.

Os dados foram obtidos a partir de várias tabelas públicas da Pordata, uma das principais plataformas estatísticas de Portugal.



📁 Fontes de Dados

As tabelas utilizadas foram extraídas de:

🔗 www.pordata.pt



A Pordata foi escolhida porque as fontes públicas mais completas (como INE, DGAEP, MTSSS, entre outras) apresentam um nível de complexidade muito maior, incluindo:

* Categorias altamente fragmentadas
* Combinações repetidas de dimensões
* Filtros pouco intuitivos
* Indicadores truncados
* Alterações estruturais ao longo dos anos
* Granularidades diferentes para variáveis semelhantes



Padronizar dados nesse nível exigiria um projeto dedicado exclusivamente ao tratamento das bases.



Mesmo assim, a Pordata possui algumas limitações:

* segmentação rígida
* categorias pouco claras
* lacunas nos anos mais recentes
* séries incompletas antes de 2015 e após 2022

Por isso, esta análise foca o período 2015–2022, por ser o mais consistente.



🔧 Processo de ETL (Python)

As bases brutas passaram por um pipeline completo de ETL:

* Limpeza e padronização das tabelas
* Seleção dos indicadores corretos
* Filtragem para Portugal continental
* Remoção de valores inconsistentes ou ausentes
* Normalização de colunas
* Exportação de CSVs limpos para modelagem



Bibliotecas utilizadas:

pandas, numpy, pathlib.



🧩 Modelagem de Dados (Power BI)

O modelo foi construído em esquema estrela (star schema), incluindo:

* DimAno (Dimensão Ano)
* Tabelas fato de salários por: sexo, idade, escolaridade, grupo profissional, 

setor, macrosetor, salário mínimo.



Etapas adicionais:

* Exclusão de anos incompletos
* Padronização das relações entre tabelas
* Criação de medidas em DAX
* Harmonização de granularidades diferentes entre fatos



📊 Visualizações e Principais Insights

O dashboard revela padrões importantes e tendências salariais em Portugal:



✔ Principais Insights

* O salário mínimo cresceu de forma contínua entre 2015 e 2022.
* O gap salarial entre homens e mulheres continua significativo e estável.
* A escolaridade é um dos fatores que mais influenciam o nível salarial.
* Setores tecnológicos, financeiros e especializados apresentam os valores mais elevados.
* Os menores salários concentram-se em serviços tradicionais e atividades de baixa qualificação.
* A faixa 65+ aparece com salários médios mais altos, refletindo maior tempo de carreira e progressão acumulada.



🛠️ Ferramentas Utilizadas

* Python (ETL)
* Power BI Desktop
* DAX
* Pordata (dados públicos)
* GitHub para versionamento e documentação



🎯 Competências Desenvolvidas

* ETL com dados reais
* Limpeza, normalização e padronização de bases públicas
* Modelagem dimensional
* Criação de dashboards profissionais
* Storytelling analítico
* Tratamento de dados incompletos e estruturas complexas



📬 Contacto

Para sugestões, dúvidas ou colaboração:

PC Data Insights – www.pcdatainsights.com



📝 Nota

Este dashboard foi criado para fins educacionais e de portfólio, utilizando dados públicos que podem conter lacunas ou inconsistências naturais.

