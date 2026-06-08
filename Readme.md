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
- VS Code
- Extensão Jupyter do VS Code
- QGIS instalado, se for executar as células que chamam `gdalinfo.exe`, `gdalwarp.exe`, `ogrinfo.exe` ou `qgis_process-qgis-ltr.bat`

CRIAR O AMBIENTE:

```powershell
python -m venv .venv
.\.venv\Scripts\Activate.ps1 
python -m pip install --upgrade pip
python -m pip install -r requirements.txt
```

SELECIONAR O KERNEL NO VS CODE:

- `Select Kernel` > `Jupyter Kernel...` > `.venv\Scripts\python.exe`

<!--
git add * ; git commit -m "aula update"; git push cdg main
jupyter nbconvert --to slides Prospecção.ipynb --TagRemovePreprocessor.remove_input_tags="hide_input" --SlidesExporter.reveal_scroll=True --post serve

reset
git init
git remote add cdg https://github.com/HumbertoDiego/cdg-ime
git add * ; git commit -m "aula update"; git push cdg main --force
-->
