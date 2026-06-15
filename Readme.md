# Ciência de Dados Geoespaciais IME

Aulas de Ciência de Dados Geoespaciais ministradas para o 3º ano do Curso de Engenharia Cartográfica do Instituto Militar de Engenharia - Rio de Janeiro/RJ.

VISÃO GERAL DA DISCIPLINA:

<img src="media/imgs/Ciência de dados geoespaciais.png">

SUMÁRIO:

- [Prospecção de dados](https://github.com/HumbertoDiego/cdg-ime/blob/main/Prospec%C3%A7%C3%A3o.ipynb)
- [Pré Processamento](https://github.com/HumbertoDiego/cdg-ime/blob/main/PreProcessamento.ipynb)
- [Mineração](https://github.com/HumbertoDiego/cdg-ime/blob/main/Minera%C3%A7%C3%A3o.ipynb)

REQUISITOS:

- [Python 3.12](https://www.python.org/downloads/)
- [VS Code](https://code.visualstudio.com/)
- [Extensão Jupyter do VS Code](https://marketplace.visualstudio.com/search?term=jupyter&target=VSCode&category=All%20categories&sortBy=Relevance)
- [QGIS](https://qgis.org/) (Para execução de `gdalinfo.exe`, `gdalwarp.exe`, `ogrinfo.exe` ou `qgis_process-qgis-ltr.bat`)

CRIAR O AMBIENTE:

```powershell
> python -m venv .venv
> .\.venv\Scripts\Activate.ps1 
(.venv) > python -m pip install --upgrade pip
(.venv) > python -m pip install -r requirements.txt
```

SELECIONAR O KERNEL NO VS CODE:

- `Select Kernel` > `Python Environments...` > `.venv\Scripts\python.exe`

DICAS PARA GERENCIAR MÚLTIPLAS VERSÕES PYTHON:

- Instale o [Python Install Manager](https://www.python.org/downloads/)
```powershell
> py install 3.9 3.10 3.11 3.12 3.14 # Instala as versões python de 3.9 a 3.14
> python --version # Python 3.14.5
> $Env:PYTHON_MANAGER_DEFAULT = "3.12" # Altera a versão para esta seção de terminal apenas
> python --version # Python 3.12.10 --> Daqui pode-se criar o ambiente
```
- Após criar o ambiente verifique se está usando uma cópia do python3.12 da pasta .venv:
```powershell
> python -c "import sys; print(sys.executable)" # C:\Users\...\Python\pythoncore-3.12-64\python.exe
> python -m venv .venv
> .\.venv\Scripts\Activate.ps1 
(.venv) > python -c "import sys; print(sys.executable)" # ...\cdg-ime\.venv\Scripts\python.exe
```


<!--
git add * ; git commit -m "aula update"; git push cdg main
jupyter nbconvert --to slides Prospecção.ipynb --TagRemovePreprocessor.remove_input_tags="hide_input" --SlidesExporter.reveal_scroll=True --post serve
jupyter nbconvert --to slides PreProcessamento.ipynb --TagRemovePreprocessor.remove_input_tags="hide_input" --SlidesExporter.reveal_scroll=True --post serve
jupyter nbconvert --to slides Mineração.ipynb --TagRemovePreprocessor.remove_input_tags="hide_input" --SlidesExporter.reveal_scroll=True --post serve

reset
git init
git remote add cdg https://github.com/HumbertoDiego/cdg-ime
git add * ; git commit -m "aula update"; git push cdg main --force
-->
