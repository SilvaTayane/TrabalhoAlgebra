# Análise de Vibração de uma Viga em Python

Este projeto realiza a análise das **frequências naturais** e **modos de vibração** de uma viga engastada utilizando o **método dos elementos finitos (MEF)**. O script é implementado em Python e utiliza bibliotecas como NumPy, SciPy e Matplotlib.

---

## Descrição

- A viga considerada tem as seguintes propriedades:
  - Comprimento: 1 m
  - Módulo de Young: 210 GPa
  - Momento de inércia: 1e-6 m⁴
  - Densidade: 7800 kg/m³
  - Área da seção: 0.01 m²
- O domínio é discretizado em 10 elementos.
- As matrizes de **rigidez** e **massa** são montadas com base em formulações clássicas do MEF.
- O sistema de equações generalizado é resolvido para encontrar os **autovalores** (frequências naturais) e **autovetores** (modos de vibração).
- O sistema é considerado **engastado na extremidade esquerda**.

---

## Tecnologias Utilizadas

- Python 3.x
- [NumPy](https://numpy.org/)
- [SciPy](https://scipy.org/)
- [Matplotlib](https://matplotlib.org/)

---

## Como Executar

1. Clone o repositório:
 ```bash
 git clone https://github.com/seu-usuario/vibracao-viga.git
 cd vibracao-viga
```

2. (Opcional) Crie e ative um ambiente virtual:

```bash
python -m venv venv
venv\Scripts\activate  # no Windows
```

3. Instale as dependências:

```bash
pip install -r requirements.txt
```

4. Execute o script:

```bash
python vibracao_viga.py
```

---

## Resultado

O programa imprime as **5 primeiras frequências naturais** da viga e exibe um gráfico com os **3 primeiros modos de vibração**.

