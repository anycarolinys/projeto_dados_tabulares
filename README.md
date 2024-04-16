## Análise do Impacto da Poluição Atmosférica na Temperatura Terrestre

Foram selecionadas cinco cidades com alto fluxo marítimo para analisar medidas relativas a temperatura e qualidade do ar de janeiro de 2022 a março de 2024.
As cidades selecionadas foram:
- Shenzhen - China  
- Manila - Filipinas  
- São Francisco - Estados Unidos
- Taipei - Taiwan  
- Cidade do Panamá - Panamá  

### Contextualização

Um estudo realizado pelo Carbon Brief¹ afirma o seguinte:
>"Em 2020, as regulamentações internacionais para reduzir a poluição atmosférica proveniente do transporte marítimo impuseram limites estritos ao teor de enxofre dos combustíveis navais.  
> As regras da Organização Marítima Internacional (IMO) tiveram algum sucesso na melhoria da saúde pública. Como resultado, as emissões globais de dióxido de enxofre (SO2) – um poluente atmosférico prejudicial à saúde – diminuíram cerca de 10%.[...]  
>As partículas de enxofre contidas nos gases de escape dos navios têm neutralizado parte do aquecimento proveniente dos gases com efeito de estufa. Mas a redução do teor de enxofre do combustível marítimo enfraqueceu o efeito de mascaramento, dando efetivamente um impulso ao aquecimento.  
>Alguns investigadores propuseram que a queda no SO2 como resultado dos regulamentos sobre ar limpo da IMO poderia estar por detrás de um recente aumento na temperatura global da superfície do mar." 

Sendo assim, o objetivo do presente estudo é avaliar o aumento da **temperatura terrestre** dada a suposta diminuição da emissão de enxofre.

![City Photography during Nightfall](https://images.pexels.com/photos/1182383/pexels-photo-1182383.jpeg)
Fonte: Pexels (2018)

### Objetivo
- A partir da API Open-Meteo² obter dados de temperatura³ e qualidade do ar⁴
- Realizar uma análise exploratória no conjunto de dados
- Analisar a evolução da temperatura
- Anaisar a evolução da concentração de gases e partículas poluentes
- Criar um modelo de predição para temperatura baseado nas varíaveis relativas a qualidade do ar

### Descrição do repositório
1. **daily_weather_ETL.ipynb**: script de ETL para geração dos dados
3. **daily_climate.csv**: dados climáticos gerados com o ETL
2. **daily_air_quality.csv**: dados de qualidade do ar gerados com o ETL
4. **weather.csv**: dados obtidos a partir da junção de 2 e 3
5. **daily_weather_EDA.ipynb**: análise exploratória dos dados em 4
6. **countries.csv**: dados das cidades e países a serem analisados

#### Referências
¹ https://www.carbonbrief.org/analysis-how-low-sulphur-shipping-rules-are-affecting-global-warming/  
² https://open-meteo.com/  
³ https://open-meteo.com/en/docs/historical-weather-api  
⁴ https://open-meteo.com/en/docs/air-quality-api  