# ML_dataset

Open datasets from Machine Learning Project

## Statistics Poland ECOICOP dataset

* Description: Excel sheet of the names of 17,099 products from three online shops (webscrapped). The products were classified to European Classification of Individual Consumption according to Purpose (ECOICOP) categories manually by non-experts. Original dataset was in Polish and was translated into English and French by google-translator.
* Source: Statistics Poland
* Preview (header and first three rows)
<table >
<tbody>
  <tr>
    <td> Desc_P</td> <td> Code_P	 </td> <td> Desc_E </td> <td> Code_E </td> <td> Desc_F </td> <td>	Code_F   </td> 
  </tr>
  <tr>
    <td> owsianka brzoskwiniowa </td> <td> Pozostałe produkty mleczne </td>  <td> Peach Porridge </td>  <td>  	Other dairy products	</td>  <td> Bouillie de pêche	 </td> <td> Autres produits laitiers   </td>
  </tr>
  <tr>
    <td> Owsianka Truskawkowa Mlekovita </td> <td> 	Pozostałe produkty mleczne	 </td>  <td> Mlekovita Strawberry  </td>  <td> Porridge	Other dairy products </td>  <td> 	Bouillie de fraises Mlekovita </td> <td> 	Autres produits laitiers </td>
  </tr>
  <tr>
    <td> Owsianka wiśniowa	 </td> <td> 	Pozostałe produkty mleczne	 </td>  <td> Cherry Porridge </td>  <td> 	Other dairy products </td>  <td> 		Bouillie de cerise	</td> <td> 	Autres produits laitiers</td>
  </tr>  
  </tbody>
  </table>

* Example of reading the dataset in python

```
df = pd.read_excel('https://raw.githubusercontent.com/UNECE/ML_dataset/master/Stats%20Poland%20ECOICOP%20data.xlsx', sheet_name = 'Data')
```
