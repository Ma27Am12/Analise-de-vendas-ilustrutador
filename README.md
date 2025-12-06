# Análise de Vendas de um Ilustrador
## Objetivo
O objetivo deste projeto foi analisar os dados de vendas de ilustrações ao longo de uma semana, avaliando o desempenho das vendas.

## Introdução
Os dados são sintéticos e servem para simular as vendas de um artista. Primeiramente, 
foi criada a base de dados em uma planilha no Google Sheets. Em seguida, realizou‑se o tratamento e a transformação dos dados com Python, 
utilizando a biblioteca Pandas. Depois foi feita a análise exploratória e, por fim, desenvolvido o dashboard no Power BI.

## Desenvolvimento
No Google Sheets, criei a base de dados com as vendas do período de 26/10/2025 a 01/11/2025. 
Foram criados quatro campos: Tipo de comissão, Quantidade, Valor e Data. Em seguida, com Python, visualizei inicialmente a estrutura e os tipos de dados de cada campo.

<img width="558" height="224" alt="image" src="https://github.com/user-attachments/assets/594d891c-fdc0-46ae-aa27-f835faa7859b" />

Alguns campos estavam com tipo de dados errado. Foi o caso das colunas Quantidade e Valor, ambas com o tipo de dado object. Verifiquei se havia dados nulos ou duplicados.

<img width="407" height="308" alt="image" src="https://github.com/user-attachments/assets/0fb478d8-c913-4538-b30e-1ca972714782" />

Ao tentar realizar a conversão de Quantidade para int e Valor para float, descobri que em ambos os campos os dados faltantes ou vazios estavam preenchidos com "-". Com isso, utilizei a função replace para trocar "-" por 0.

<img width="1198" height="193" alt="image" src="https://github.com/user-attachments/assets/c75e3773-d609-41ee-bb31-e80d5b25a3d3" />

Em seguida, realizei a conversão de Quantidade para int e Valor para float.

<img width="706" height="87" alt="image" src="https://github.com/user-attachments/assets/d37889d4-6d1a-47b9-8ead-0aadc385688d" />

Com os dados tratados, avancei para a etapa da análise exploratória. Primeiro utilizei o comando describe para visualizar medidas gerais.

<img width="428" height="301" alt="image" src="https://github.com/user-attachments/assets/10787ca8-ed76-4cbc-859d-4d3634d7eb0c" />

Depois utilizei gráficos de caixa para observar a dispersão dos dados.

<img width="644" height="385" alt="image" src="https://github.com/user-attachments/assets/3aa9f2fc-7a64-48d6-8109-0a5978c3ec61" />

<img width="659" height="395" alt="image" src="https://github.com/user-attachments/assets/4daf8336-8e93-4ee5-a453-26dfe71db48f" />

Criei gráficos com a média de Quantidade e Valor.

<img width="654" height="356" alt="image" src="https://github.com/user-attachments/assets/0a7ee5c9-16d6-4109-8c43-25ab526ab621" />

<img width="586" height="354" alt="image" src="https://github.com/user-attachments/assets/49941210-297e-45cb-bea5-20d1d12549d9" />

E, por fim, criei histogramas para Quantidade e Valor.

<img width="833" height="547" alt="image" src="https://github.com/user-attachments/assets/c8533d52-4883-4f1a-8f91-5649d4fab1c0" />

<img width="833" height="547" alt="image" src="https://github.com/user-attachments/assets/f09593c7-c9ab-4280-bb64-6248f317ecfb" />

No dashboard, criei duas páginas: uma com a visão geral dos dados e outra com a visão ao longo do tempo. Primeiro apresentei a visão geral. Nela utilizei quatro visuais: um gráfico de colunas, um de barras, um de setores e um de rosca. Observando os gráficos, é possível perceber que as ilustrações do tipo full-body foram as que mais renderam, alcançando o valor de R$ 19.200,00. Porém, as ilustrações do tipo half-body foram as que mais venderam, mesmo rendendo menos, totalizando R$ 13.580,00. Isso se explica pelo preço unitário de cada tipo de ilustração: uma ilustração full-body custa R$ 240,00, enquanto uma half-body custa R$ 140,00.

<img width="872" height="493" alt="image" src="https://github.com/user-attachments/assets/6f12e953-f9f3-4ac6-a1a3-33769e1fd5ed" />

Na segunda página, intitulada "visão ao longo do tempo", utilizei dois gráficos de linhas para mostrar a variação de vendas e de quantidade ao decorrer da semana de 26/10/2025 a 01/11/2025.

<img width="869" height="493" alt="image" src="https://github.com/user-attachments/assets/876ba5af-fc0f-4a47-b0aa-04241b5d780b" />

Observando os dois gráficos, é possível perceber um grande crescimento das vendas e do rendimento nos dias 30 e 31 de outubro, datas referentes ao Halloween. Nesse período, as ilustrações full-body venderam mais e renderam mais. O que fez com que as half-body vendessem mais foi a alta quantidade consistente de vendas ao longo do tempo.

## Conclusão
Esse tipo de projeto pode ajudar um ilustrador a compreender o desempenho de suas comissões e o perfil de seus clientes, além de subsidiar decisões sobre seus produtos.

