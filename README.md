![4eddit](https://i.imgur.com/lYaRcNR.png)

> Status do Projeto: Em desenvolvimento :warning:

### Link de acesso
### http://falemais-andrius.surge.sh/

# 4eddit

#### A empresa de telefonia Telzir, especializada em chamadas de longa distância nacional, vai colocar um novo produto no mercado chamado FaleMais.
#### Normalmente um cliente Telzir pode fazer uma chamada de uma cidade para outra pagando uma tarifa fixa por minuto, com o preço sendo pré-definido em uma lista com os códigos DDDs de origem e destino:

Origem | Destino | $/min
------ | ------- | ------
011    | 016     | 1.90
016    | 011     | 2.90
011    | 017     | 1.70
017    | 011     | 2.70
011    | 018     | 0.90
018    | 011     | 1.90

#### Com o novo produto FaleMais da Telzir o cliente adquire um plano e pode falar de graça até um determinado tempo (em minutos) e só paga os minutos excedentes. Os minutos excedentes tem um acréscimo de 10% sobre a tarifa normal do minuto. Os planos são FaleMais 30 (30 minutos), FaleMais 60 (60 minutos) e FaleMais 120 (120 minutos).
#### A Telzir, preocupada com a transparência junto aos seus clientes, quer disponibilizar uma página na web onde o cliente pode calcular o valor da ligação. Ali, o cliente pode escolher os códigos das cidades de origem e destino, o tempo da ligação em minutos e escolher qual o plano FaleMais. O sistema deve mostrar dois valores: (1) o valor da ligação com o plano e (2) sem o plano. O custo inicial de aquisição do plano deve ser desconsiderado para este problema.

### Ex:
Origem | Destino | Tempo | Plano FaleMais | Com FaleMais | Sem FaleMais
------ | ------- | ----- | -------------- | ------------ | ------------ 
011    | 016     | 20    | FaleMais 30    | $ 0,00       | $ 38,00
011    | 017     | 80    | FaleMais 60    | $ 37,40      | $ 136,00
018    | 011     | 200   | FaleMais 120   | $ 167,20     | $ 380,00
018    | 017     | 100   | FaleMais 30    | -            | -

# Linguagens de programação e bibliotecas utilizadas

### - JavaScript
### - ReactJS
### - React-Router
### - MaterialUI
### - Jest
### - Enzyme

# Como iniciar o projeto

### Entre no diretório do projeto e execute:

### `npm install`

Instala as dependencias do projeto.

### `npm start`

Executa o aplicativo no modo de desenvolvimento.<br />
Abra [http://localhost:3000](http://localhost:3000) para visualizá-lo no navegador.

A página será recarregada se você fizer edições. <br />
Você também verá erros no console.

### `npm test`

Inicia o corredor de teste no modo de observação interativo.<br />
Os testes foram realizados com jest e enzyme.

### `npm run build`

Cria o aplicativo para produção na pasta `build`. <br />
Ele agrupa corretamente o React no modo de produção e otimiza a construção para o melhor desempenho.

A compilação é minificada e os nomes de arquivos incluem os hashes. <br />
Seu aplicativo está pronto para ser implantado!

