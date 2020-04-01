# ML_dataset

Open datasets from Machine Learning Project

## Statistics Poland ECOICOP Dataset

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

## Belgium VITO Energy Balance Dataset

* Description: Excel sheet with quarterly electricity supplied (e.g. combustible, hyrdo, nuclear), economic indicator (e.g. GDP, GVA) and other variables (e.g. population, sunspots) from 2000 Q1 to 2019 Q1.
* Source: Buelens, Bart, & Goyens, Anneleen. (2020). Energy Balance Flanders quarterly and monthly data and related auxiliary data (Version 1.0.0) [Data set]. Zenodo. http://doi.org/10.5281/zenodo.3596695
* Preview (header and first three rows)
<table >
<tbody>
  <tr>    
    <td> Variable </td> <td> Full name		 </td> <td> 2000Q1	 </td> <td> 2000Q2	 </td> <td> 2000Q3	 </td> <td>	...  </td>  <td> 2019Q1 </td>
  </tr>
  <tr>
    <td> EnrgCombustibleFuels </td> <td>+ Combustible Fuels GWh	</td>  <td> 10108	</td>  <td>  	7739		</td>  <td> 6984	 </td> <td> ... </td> <td>8681.063 </td>
  </tr>
  <tr>
    <td>EnrgNuclearNuclear	</td> <td> 	+ Nuclear GWh	 </td>  <td>11087	 </td>  <td> 10770	</td>  <td> 	11154</td> <td> 	... </td> <td>9304.936 </td>
  </tr>
  <tr>
    <td> EnrgHydroHydro </td> <td> 		+ Hydro GWh	 </td>  <td> 	446	</td>  <td> 357	 </td>  <td> 		397 </td> <td> 	... </td> <td>346.173 </td>
  </tr>  
  </tbody>
  </table>

* Example of reading the dataset in python

```
df = pd.read_excel('https://zenodo.org/record/3596695/files/VITO_EnergyBalanceDataML.xlsx', sheet_name = 'quarterly_txt')
```
