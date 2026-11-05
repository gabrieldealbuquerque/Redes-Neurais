# Redes Neurais — fundamentos na prática

Notebooks de estudo sobre redes neurais e aprendizado de máquina, desenvolvidos no contexto acadêmico da **UFES**. A coleção percorre o neurônio de McCulloch–Pitts, operações com imagens, otimização por gradiente e redes multicamadas, com implementações em **Python, NumPy e PyTorch**.

> **English summary:** Educational notebooks covering McCulloch–Pitts neurons, image arrays, gradient descent, linear regression, MLP backpropagation in NumPy, and sine regression with PyTorch autograd and analytical gradients.

## Percurso de estudo

Os links abaixo apontam para os notebooks de referência de cada assunto. A ordem segue dos modelos mais simples ao treinamento de redes multicamadas.

| Etapa | Notebook | O que explorar |
| --- | --- | --- |
| 1 | [Neurônio MCP e circuitos lógicos](Exerc%C3%ADcio%201/02-01-MPC-Atividade-especificacao.ipynb) | Pesos, limiar de ativação, tabelas verdade e composição de neurônios. |
| 2 | [MCP como classificador](Exerc%C3%ADcio%201/MCP-classificador-especificacao.ipynb) | Classificação binária, acurácia, fronteiras de decisão e separabilidade linear. |
| 3 | [Arrays e imagens](Exerc%C3%ADcio%202/02_02_arrays_e_imagens-especificacao.ipynb) | Matrizes NumPy, canais de cor, transformações e manipulação de imagens com OpenCV e Pillow. |
| 4 | [Descida do gradiente](Exercicio%20Gradiente/08-01-descida_do_gradiente_intro-especificacao.ipynb) | Gradientes, otimização e visualização da trajetória de atualização dos parâmetros. |
| 5 | [Regressão linear](Regress%C3%A3o%20Linear/08-02-linear-with-gd-especificacao.ipynb) | Função de perda, derivadas e ajuste dos parâmetros por descida do gradiente. |
| 6 | [Regressão de seno](Revis%C3%A3o%20Prova%202/resposta.ipynb) | Ajuste de `sin(x + a) + b` com autograd do PyTorch e com derivadas implementadas manualmente. |
| 7 | [MLP e backpropagation](Revis%C3%A3o%20Prova%202/backprop.ipynb) | Forward, propagação dos gradientes, ativações e implementações de redes multicamadas em NumPy. |

## Como executar

É possível ler os notebooks diretamente no GitHub. Para executar as células localmente, clone o repositório e prepare um ambiente Python:

```bash
git clone https://github.com/gabrieldealbuquerque/Redes-Neurais.git
cd Redes-Neurais
python -m venv .venv
```

Ative o ambiente com `source .venv/bin/activate` no Linux/macOS ou `.venv\Scripts\Activate.ps1` no PowerShell. Em seguida:

```bash
python -m pip install -r requirements.txt
jupyter lab
```

Abra o notebook pela interface do Jupyter e execute as células na ordem. Mantenha o diretório de trabalho na pasta do notebook: as atividades usam caminhos relativos para imagens e arquivos de dados, como `ds_0.txt` e `data-1.txt`.

### Ambiente e dados

- [requirements.txt](requirements.txt) reúne as dependências usadas nos notebooks e o JupyterLab. As versões não estão fixadas; o arquivo facilita a instalação, mas não constitui um ambiente reproduzível com lock de versões.
- Os dados de regressão estão nas próprias pastas das atividades. Algumas células também acessam imagens pela internet ou bases via OpenML, exigindo conexão.
- Há referências a arquivos que não acompanham a coleção, como `chameleon.jpg`. Nessas células, forneça a imagem solicitada ou ajuste o caminho para uma imagem local.
- Inicializações aleatórias e diferenças de versão podem alterar curvas e resultados. As saídas salvas registram execuções anteriores; esta apresentação não atesta a reexecução integral dos notebooks.

## Organização

```text
Exercício 1/          Neurônio MCP, lógica e classificação
Exercício 2/          Arrays, imagens e arquivos de apoio
Exercicio Gradiente/  Introdução à descida do gradiente
Regressão Linear/    Ajuste de modelos e datasets de regressão
Revisao Prova 1/     Materiais de revisão sobre MCP e imagens
Revisão Prova 2/     Regressão de seno e MLP com backpropagation
```

As pastas de revisão e as versões alternativas foram preservadas como registro de estudo. Para começar, use o percurso acima; a coleção contém enunciados, respostas e experimentos em diferentes estágios de desenvolvimento.

## Créditos e licença

**Gabriel de Albuquerque** — resoluções, experimentos e organização deste repositório de estudos.

Os enunciados e materiais didáticos fornecidos na disciplina são atribuídos ao **professor Filipe Mutz**. A coleção reúne material de aula e contribuições de estudo; a disponibilização aqui não implica autoria exclusiva sobre os enunciados, imagens ou materiais de terceiros.

O repositório contém uma [licença MIT](LICENSE). Preserve os créditos e os avisos de autoria aplicáveis aos materiais educacionais e aos recursos externos utilizados.
