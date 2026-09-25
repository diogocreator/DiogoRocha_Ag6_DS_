# DiogoRocha_Ag5_DS_I
Agenda 05_Desenvolvimento de Sistemas I_ Apresentação_Introdução ao Fichário_Atividade de Recuperação_


![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)

## 📌 Sobre o Projeto
A **Calculadora de Consumo Elétrico** é uma aplicação em Python criada para ajudar usuários a estimar o consumo mensal de energia elétrica de seus eletrodomésticos e a apresentar uma estimativa de custo mensal com base em uma tarifa média.

## 🧮 Fórmula Utilizada
O consumo mensal em quilowatts-hora (kWh) é determinado através da seguinte equação:

$$consumoMensal = \frac{potencia \times horasDia \times 30}{1000}$$

---

## 🚀 Como Executar o Projeto

### Pré-requisitos
* Ter o **Python** instalado na máquina.

### Passo a passo
1. Clone este repositório ou baixe os arquivos.
2. Abra o terminal na pasta do projeto.
3. Execute o comando:

```bash
python app.py
def calcular_consumo():
    print("=" * 40)
    print("⚡ CALCULADORA DE CONSUMO ELÉTRICO ⚡")
    print("=" * 40)

    # Entradas de dados
    aparelho = input("Nome do aparelho eletrodoméstico:").strip()
    potencia = float(input("Potência do aparelho (em Watts):"))
    horas_dia = float(input("Tempo médio de uso diário (em horas):"))

    # Cálculo do consumo mensal em kWh
    consumo_mensal = (potencia * horas_dia * 30) / 1000

    # Cálculo do custo estimado (R$ 0,75 por kWh)
    tarifa_kwh = 0.75
    custo_estimado = consumo_mensal * tarifa_kwh

    # Exibição dos resultados
    print("\n" + "-" * 40)
    print(f"Aparelho: {aparelho}")
    print(f"Consumo estimado: {consumo_mensal:.2f} kWh/mês")
    print(f"Custo estimado: R$ {custo_estimado:.2f}/mês (Tarifa ref.: R$ 0,75/kWh)")
    print("-" * 40)

if __name__ == "__main__":
    calcular_consumo()
