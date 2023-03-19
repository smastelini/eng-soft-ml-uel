# Tutorial de instalação

Utilizaremos o jupyter notebook para criar arquivos interativos que podem combinar código e texto. Esses arquivos serão compartilhados (em geral) no começo das aulas, para que possam acompanhar a execução dos códigos e melhor entender o conteúdo apresentado.

Passos (ler observação no final):

1. Instalar o miniconda: [website](https://docs.conda.io/en/latest/miniconda.html)
2. Criar uma pasta para as aulas da disciplina
3. Salvar o conteúdo a seguir como um arquivo chamado `environment.yml`, dentro da pasta criada
  - Atenção na extensão do arquivo

```yml

name: uel
channels:
  - defaults
dependencies:
  - ca-certificates=2023.01.10=haa95532_0
  - certifi=2022.12.7=py39haa95532_0
  - openssl=1.1.1t=h2bbff1b_0
  - pip=22.3.1=py39haa95532_0
  - python=3.9.16=h6244533_0
  - setuptools=65.6.3=py39haa95532_0
  - sqlite=3.40.1=h2bbff1b_0
  - vc=14.2=h21ff451_1
  - vs2015_runtime=14.27.29016=h5e58377_2
  - wheel=0.38.4=py39haa95532_0
  - wincertstore=0.2=py39haa95532_2
  - pip:
      - altair==4.2.2
      - anyio==3.6.2
      - argon2-cffi==21.3.0
      - argon2-cffi-bindings==21.2.0
      - arrow==1.2.3
      - asttokens==2.2.1
      - attrs==22.2.0
      - backcall==0.2.0
      - beautifulsoup4==4.11.2
      - bleach==6.0.0
      - blinker==1.5
      - cachetools==5.3.0
      - cffi==1.15.1
      - charset-normalizer==3.0.1
      - click==8.1.3
      - colorama==0.4.6
      - comm==0.1.2
      - contourpy==1.0.7
      - cycler==0.11.0
      - debugpy==1.6.6
      - decorator==5.1.1
      - defusedxml==0.7.1
      - entrypoints==0.4
      - executing==1.2.0
      - fastjsonschema==2.16.3
      - fonttools==4.38.0
      - fqdn==1.5.1
      - gitdb==4.0.10
      - gitpython==3.1.31
      - idna==3.4
      - importlib-metadata==6.0.0
      - importlib-resources==5.12.0
      - ipykernel==6.21.2
      - ipython==8.10.0
      - ipython-genutils==0.2.0
      - ipywidgets==8.0.4
      - isoduration==20.11.0
      - jedi==0.18.2
      - jinja2==3.1.2
      - joblib==1.2.0
      - jsonpointer==2.3
      - jsonschema==4.17.3
      - jupyter==1.0.0
      - jupyter-client==8.0.3
      - jupyter-console==6.6.1
      - jupyter-core==5.2.0
      - jupyter-events==0.6.3
      - jupyter-server==2.3.0
      - jupyter-server-terminals==0.4.4
      - jupyterlab-pygments==0.2.2
      - jupyterlab-widgets==3.0.5
      - kiwisolver==1.4.4
      - lightgbm==3.3.5
      - markdown-it-py==2.2.0
      - markupsafe==2.1.2
      - matplotlib==3.7.0
      - matplotlib-inline==0.1.6
      - mdurl==0.1.2
      - mistune==2.0.5
      - nbclassic==0.5.2
      - nbclient==0.7.2
      - nbconvert==7.2.9
      - nbformat==5.7.3
      - nest-asyncio==1.5.6
      - notebook==6.5.2
      - notebook-shim==0.2.2
      - numpy==1.24.2
      - packaging==23.0
      - pandas==1.5.3
      - pandocfilters==1.5.0
      - parso==0.8.3
      - pickleshare==0.7.5
      - pillow==9.4.0
      - platformdirs==3.0.0
      - plotly==5.13.1
      - prometheus-client==0.16.0
      - prompt-toolkit==3.0.37
      - protobuf==3.20.3
      - psutil==5.9.4
      - pure-eval==0.2.2
      - pyarrow==11.0.0
      - pycparser==2.21
      - pydeck==0.8.0
      - pygments==2.14.0
      - pympler==1.0.1
      - pyparsing==3.0.9
      - pyrsistent==0.19.3
      - python-dateutil==2.8.2
      - python-json-logger==2.0.7
      - pytz==2022.7.1
      - pytz-deprecation-shim==0.1.0.post0
      - pywin32==305
      - pywinpty==2.0.10
      - pyyaml==6.0
      - pyzmq==25.0.0
      - qtconsole==5.4.0
      - qtpy==2.3.0
      - requests==2.28.2
      - rfc3339-validator==0.1.4
      - rfc3986-validator==0.1.1
      - rich==13.3.1
      - scikit-learn==1.2.1
      - scipy==1.10.1
      - seaborn==0.12.2
      - semver==2.13.0
      - send2trash==1.8.0
      - six==1.16.0
      - smmap==5.0.0
      - sniffio==1.3.0
      - soupsieve==2.4
      - stack-data==0.6.2
      - streamlit==1.19.0
      - tenacity==8.2.1
      - terminado==0.17.1
      - threadpoolctl==3.1.0
      - tinycss2==1.2.1
      - toml==0.10.2
      - toolz==0.12.0
      - tornado==6.2
      - traitlets==5.9.0
      - typing-extensions==4.5.0
      - tzdata==2022.7
      - tzlocal==4.2
      - uri-template==1.2.0
      - urllib3==1.26.14
      - validators==0.20.0
      - watchdog==2.3.0
      - wcwidth==0.2.6
      - webcolors==1.12
      - webencodings==0.5.1
      - websocket-client==1.5.1
      - widgetsnbextension==4.0.5
      - zipp==3.15.0

```

4. Abrir um terminal adequado para manipular o anaconda/miniconda:
  - No Windows: anaconda powershell
  - No Linux e Mac: o terminal padrão do sistema
5. Navegar no terminal até a pasta criada (alternativamente, o terminal pode ser aberto diretamente na pasta)
6. Executar o seguinte comando: `conda env create -f environment.yml`

A partir daqui, os passos serão utilizados toda vez que formos utilizar os notebooks jupyter:

7. Com o terminal aberto na pasta das aulas, rodar o seguinte comando para ativar o ambiente de programação criado: `conda activate uel`
8. Abrir o ambiente do jupyter notebook, rodando o seguinte comando: `jupyter notebook`

> **Obs:** pode ser que seja necessário fechar e reabrir o terminal após a execução do passo 1, para que os passos posteriores funcionem corretamente

Vamos iniciar a parte prática de hoje.