# Tableau_function
Functions and calculate in tableau


# DailyStudy

![GitHub repo size](https://img.shields.io/github/repo-size/iuricode/README-template?style=for-the-badge)
![GitHub language count](https://img.shields.io/github/languages/count/iuricode/README-template?style=for-the-badge)
![GitHub forks](https://img.shields.io/github/forks/iuricode/README-template?style=for-the-badge)
![Bitbucket open issues](https://img.shields.io/bitbucket/issues/iuricode/README-template?style=for-the-badge)
![Bitbucket open pull requests](https://img.shields.io/bitbucket/pr-raw/iuricode/README-template?style=for-the-badge)

1 STEP: To create a filter, you need to create a parameter with all the items you want to show. After that, the filter will appear on the right side.

<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="Captura de Tela 2025-02-25 às 22.29.36.png" width="500" alt="Tableau's Dashboard"/><br>
      </a>
    </td>
  </tr>
</table>



<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="Captura de Tela 2025-02-25 às 22.29.49.png" width="500" alt="Tableau's Dashboard"/><br>
      </a>
    </td>
  </tr>
</table>


2 STEP: Identify places in the file without information.


<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="Captura de Tela 2025-02-25 às 22.36.05.png" width="500" alt="Tableau's Dashboard"/><br>
      </a>
    </td>
  </tr>
</table>



<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="Captura de Tela 2025-02-25 às 22.36.15.png" width="500" alt="Tableau's Dashboard"/><br>
      </a>
    </td>
  </tr>
</table>





```
CASE [Country]
WHEN 'Afghanistan' THEN 'Southern Asia'
WHEN 'Albania' THEN 'Central and Eastern Europe'
WHEN 'Algeria' THEN 'Middle East and Northern Africa'
WHEN 'Angola' THEN 'Sub-Saharan Africa'
END
```

3 STEP: Create a column

```
SPLIT(SPLIT([Dados],'<nome>',2),'</nome>',1)
SPLIT(SPLIT([Dados],'<profissao>',2),'</profissao>',1)
SPLIT(SPLIT([Dados],'<idade>',2),'</idade>',1)
```


```
###Split the pbone Number from the file. 
    REGEXP_EXTRACT([String of Data (String of Data)],'(\([0-9]{3}\)-[0-9]{3}-[0-9]{4})')
```

```
###The number 1 indicates that we are interested in the first part of the string (the part before the first space).
SPLIT([Diagnosis], " ", 1)
```

```
###Extracts a character from the [DX] column starting at position 2, and converts it into an integer.
INT(MID([DX], 2, 1))
```

```
###Checks if the value in the [Null Hunting] column is null.
ISNULL([Null Hunting])
```

```
### Removes the [DX] value (plus a space) from the [Diagnosis] column.
   REPLACE([Diagnosis], [DX] + " ", "")
```

4 STEP: Tableau Prep

###Edit the file first. Change CPF to string and change the State
<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="Captura de Tela 2025-02-26 às 18.36.25.png" width="500" alt="Tableau's Dashboard"/><br>
      </a>
    </td>
  </tr>
</table>

<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="Captura de Tela 2025-02-26 às 19.07.06.png" width="500" alt="Tableau's Dashboard"/><br>
      </a>
    </td>
  </tr>
</table>


###Create a new condition like M-> Masculine

<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="Captura de Tela 2025-02-26 às 19.23.06.png" width="500" alt="Tableau's Dashboard"/><br>
      </a>
    </td>
  </tr>
</table>

```
  CASE [CIDADE]
  WHEN 'rio' THEN 'Rio de Janeiro'
  WHEN 'rio de Janeiro' THEN 'Rio de Janeiro'
  WHEN 'R. de Janeiro' THEN 'Rio de Janeiro'
  ELSE 'Rio de Janeiro'
  END
```

### Aggregate information 

<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="Captura de Tela 2025-02-26 às 19.40.21.png" width="500" alt="Tableau's Dashboard"/><br>
      </a>
    </td>
  </tr>
</table>

### Adjustments and improvements.

The project is still under development, and the upcoming updates will focus on the following tasks:

- [x] Advanced courses about Tableau

The following tools were used in the construction of the project:

- [Tableau Public ](<https://public.tableau.com/app/discover/>)



## 🤝 Creator

<table>
  <tr>
    <td align="center">
      <a href="#" title="Thales Farias">
        <img src="grecia.jpg" width="100" alt="Foto do Thales Farias no GitHub"/><br>
        <sub>
          <b><a href="https://www.linkedin.com/in/thalesfreirefarias/" target="_blank">Thales Farias</b>
        </sub>
      </a>
    </td>
  </tr>
</table>


