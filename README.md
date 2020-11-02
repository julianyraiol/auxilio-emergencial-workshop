# auxilio-emergencial-workshop

Os dados trabalhados nesse workshop foram retirados do [Portal da Transparência da União](http://www.portaltransparencia.gov.br/pagina-interna/603519-download-de-dados-auxilio-emergencial). 

Slides apresentados no workshop do [CODA2020](https://escoladedados.org/coda2020/): [Link](https://docs.google.com/presentation/d/1QoP9EHWsl-OZca-DCQIoXK1B70to55K_CyMAK3QsWcY/edit?usp=sharing)

### Estrutura do projeto

```
|-- notebooks
|   |-- notebooks
|   |-- auxilio-emergencial.ipynb
|   |-- coda-br.ipynb
|
|-- Pipfile
|-- Pipfile.lock
|-- README.md
`-- docker-compose.yml
```

### Setup
Este projeto requer **Python 3.+** e a instalação do [**Pipenv**](https://pipenv-fork.readthedocs.io/en/latest/install.html), arquivo que contém as dependências do projeto. Para instalá-lo, execute: 

```bash
pip install pipenv
```

Caso haja algum problema durante a instação do pacote, veja a documentação da ferramenta.

### Configuração o projeto

Faça o clone deste projeto e execute o arquivo **Pipenv**:

```bash
$ git clone https://github.com/julianyraiol/auxilio-emergencial-workshop.git
$ cd auxilio-emergencial-workshop
$ pipenv install
$ pipenv shell
```

### Para executar os notebooks

No seu terminal, já tendo executado o arquivo de instalação, execute o seguinte comando:

```bash
$ jupyter-lab
```

### Para persistir os dados no elasticsearch

Execute o docker-compose para criar uma instância local do elasticsearch. Ele ficará rodando na endereço: http://localhost:9200/. 
O kibana estará no endereço: http://localhost:5601/

```bash
$ docker-compose up -d
```
