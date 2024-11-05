# desafio_IA_RocketSeat

Este é o primeiro desafio proposto pela RocketSeat no módulo de IA.

O primeiro desafio proposto tem a finalidade de botar em prática alguns conceitos em estatística e transformar dados em gráficos na linguagem Python.

<br>

## Enunciado

> Com base nas aulas do módulo de Estatística, utilize os métodos da biblioteca Pandas para tratar o dicionário abaixo e:
>- Trazer a média das vendas;
>- Criar um gráfico de barras vertical mostrando o mês de referência e o valor;
>- Criar um gráfico de linhas mostrando o mês de referência e o valor.

____

<br>

## Base de Dados
### Python
````
dict_faturamento = {
    'data_ref': [
        '2023-01-01', 
        '2020-02-01', 
        '2021-03-01', 
        '2022-04-01', 
        '2023-05-01',
        '2023-06-01', 
        '2020-07-01', 
        '2021-08-01', 
        '2022-09-01', 
        '2023-10-01',
        '2022-11-01', 
        '2023-12-01'
    ],
    'valor': [
        400000, 
        890000, 
        760000, 
        430000, 
        920000,
        340000, 
        800000, 
        500000, 
        200000, 
        900000,
        570000, 
        995000
    ]
}
````

<br>

Com a base proposta, transformei o dicionário em um DataFrame

<br>

````
df_faturamento = pd.DataFrame.from_dict(dict_faturamento)
````

E a base ficou da seguinte forma:

<div>
<style scoped>
    .dataframe tbody tr th:only-of-type {
        vertical-align: middle;
    }

    .dataframe tbody tr th {
        vertical-align: top;
    }

    .dataframe thead th {
        text-align: right;
    }
</style>
<table border="1" class="dataframe">
  <thead>
    <tr style="text-align: right;">
      <th></th>
      <th>data_ref</th>
      <th>valor</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <th>0</th>
      <td>2023-01-01</td>
      <td>400000</td>
    </tr>
    <tr>
      <th>1</th>
      <td>2020-02-01</td>
      <td>890000</td>
    </tr>
    <tr>
      <th>2</th>
      <td>2021-03-01</td>
      <td>760000</td>
    </tr>
    <tr>
      <th>3</th>
      <td>2022-04-01</td>
      <td>430000</td>
    </tr>
    <tr>
      <th>4</th>
      <td>2023-05-01</td>
      <td>920000</td>
    </tr>
    <tr>
      <th>5</th>
      <td>2023-06-01</td>
      <td>340000</td>
    </tr>
    <tr>
      <th>6</th>
      <td>2020-07-01</td>
      <td>800000</td>
    </tr>
    <tr>
      <th>7</th>
      <td>2021-08-01</td>
      <td>500000</td>
    </tr>
    <tr>
      <th>8</th>
      <td>2022-09-01</td>
      <td>200000</td>
    </tr>
    <tr>
      <th>9</th>
      <td>2023-10-01</td>
      <td>900000</td>
    </tr>
    <tr>
      <th>10</th>
      <td>2022-11-01</td>
      <td>570000</td>
    </tr>
    <tr>
      <th>11</th>
      <td>2023-12-01</td>
      <td>995000</td>
    </tr>
  </tbody>
</table>
</div>


## Média do Faturamento

