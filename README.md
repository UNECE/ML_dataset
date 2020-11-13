# ML_dataset

Open datasets from Machine Learning Project

## Statistics Poland ECOICOP Dataset

* Description: Excel sheet of the names of 17,099 products that were web scraped and anonymized from three online shops. The products were classified to European Classification of Individual Consumption according to Purpose (ECOICOP) categories manually by non-experts. Original dataset was in Polish and was translated to different languages provided in different sheets. The translation was carried out using an on-line translator and was not reviewed for accuracy or appropriateness.
* Source: Statistics Poland
* Preview - Sheet "Polish" (header and first three rows)
<table>
<tbody>
  <tr>
    <td> produkt </td> <td> kategoria	 </td> 
  </tr>
  <tr>
    <td> Hejki - Emotki lizaki ręcznie robione o smakach owocowych </td> <td> Wyroby cukiernicze </td>  
  </tr> 
  <tr>
    <td>100% Pur jus d orange sok pomarańczowy z miąższe... </td> <td>Soki owocowe i warzywne  </td>  
  </tr>  
  
  <tr>
    <td>100% sukraloza bez cukru (substancje słodzące) </td> <td> Sztuczne substytuty cukru </td>  
  </tr>  
  </tbody>
  </table>


* Preview - Sheet "English" (header and first three rows)
<table>
<tbody>
  <tr>
    <td> produkt </td> <td> kategoria	 </td> 
  </tr>
  <tr>
    <td> Hejki - Emotes handmade lollipops with fruit flavors </td> <td> Confectionery products </td>  
  </tr> 
  <tr>
    <td> 100% Pur jus d orange orange juice with pulp ... </td> <td> Fruit and vegetable juices </td>  
  </tr>  
  
  <tr>
    <td> 100% sucralose without sugar (sweeteners) </td> <td> Artificial sugar substitutes </td>  
  </tr>  
  </tbody>
  </table>


* Example of reading the dataset in python

```
df = pd.read_excel('https://raw.githubusercontent.com/UNECE/ML_dataset/master/Stats%20Poland%20ECOICOP%20data.xlsx', sheet_name = 'Polish')
```
You can choose data in: Dutch, English, French, German, Italian, Polish or Spanish, by changing the value of the parameter sheet_name.


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
