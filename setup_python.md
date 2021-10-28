Para isolar as dependencias dos projetos é criando ambientes (env) para estes projetos.

Estes ambientes precisam ser criados e apontados para as IDEs de codificação, por exemplo PyCharm, ou VScode.

Neste scenaio criamo o ambiente utilizando o ANACONDA(miniconda) e VENS.

### Anaconda

1. Instalado PyCharm, VS Code e anaconda.
2. Configurado o ambiente do projeto "aula" no anaconda:
````
conda create -n aula python=3.7
conda activate aula
conda list

conda install -c anaconda numpy
````

3. Configurado settings.json do meu ambiente:
````
{
    "python.pythonPath": "C:\\Users\\glaub\\.conda\\envs\\aula\\python.exe",
    "python.terminal.activateEnvironment": true,
    "terminal.external.windowsExec": "C:\\WINDOWS\\System32\\cmd.exe \"/K\" C:\\Users\\glaub\\.conda\\envs\\aula\\Scripts\\activate.bat C:\\Users\\glaub\\.conda"
}
````

Pode ser necessario alterar o interpretador padrão (acionado pelo comano f1, para o CMD)
[image](https://user-images.githubusercontent.com/22028539/131329823-5458e0c1-f4b2-4548-b715-3ff1fa1acbcc.png)


4. Por meio da interface grafica é possivel configurar utilizando o caminho: File>Settings> Project> Python interpreter > Add exixtent env

### VENVs

````
python3 -m venv /path/to/new/virtual/environment
python -m venv c:\path\to\myenv
````
