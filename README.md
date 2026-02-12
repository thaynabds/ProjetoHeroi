# ProjetoHeroi
# ⚔️ Projeto Herói - Classes e Objetos em Python

Este projeto faz parte de um desafio da DIO e tem como objetivo praticar os conceitos de **Programação Orientada a Objetos (POO)** em Python, criando uma classe genérica que representa um herói de aventura.

## 🧠 Objetivo

Criar uma classe que modele um herói com **nome**, **idade** e **tipo** (guerreiro, mago, monge ou ninja), além de um método `atacar()` que exibe uma mensagem personalizada com base no tipo do herói.

---

## 📦 Estrutura do Projeto

```
projeto-heroi/
│
├── heroi.py          # Código principal com a classe e exemplo de uso
└── README.md         # Documentação do projeto
```

---

## 🧱 Classe: `Heroi`

**Atributos:**
- `nome`: nome do herói
- `idade`: idade do herói
- `tipo`: tipo do herói (guerreiro, mago, monge ou ninja)

**Métodos:**
- `atacar()`: exibe a mensagem de ataque conforme o tipo

---

## ⚔️ Tabela de Ataques

| Tipo        | Ataque            |
|-------------|-------------------|
| mago        | usou magia        |
| guerreiro   | usou espada       |
| monge       | usou artes marciais |
| ninja       | usou shuriken     |

---

## 💻 Código

```python
class Heroi:
    def __init__(self, nome, idade, tipo):
        self.nome = nome
        self.idade = idade
        self.tipo = tipo
    
    def atacar(self):
        ataques = {
            "mago": "magia",
            "guerreiro": "espada",
            "monge": "artes marciais",
            "ninja": "shuriken"
        }
        
        ataque = ataques.get(self.tipo, "ataque desconhecido")
        print(f"o {self.tipo} atacou usando {ataque}")

# Entrada do usuário
nome = input("Digite o nome do herói: ")
idade = input("Digite a idade do herói: ")
tipo = input("Digite o tipo do herói (guerreiro, mago, monge, ninja): ")

# Criação do objeto e ataque
heroi = Heroi(nome, idade, tipo)
heroi.atacar()
```

---

## ▶️ Exemplo de Execução

```
Digite o nome do herói: Aric
Digite a idade do herói: 28
Digite o tipo do herói (guerreiro, mago, monge, ninja): mago
o mago atacou usando magia
```

```
Digite o nome do herói: Takashi
Digite a idade do herói: 22
Digite o tipo do herói (guerreiro, mago, monge, ninja): ninja
o ninja atacou usando shuriken
```

---

## 🛠️ Conceitos Aplicados

- ✅ Variáveis  
- ✅ Operadores  
- ✅ Estruturas de decisão  
- ✅ Funções  
- ✅ Classes e Objetos  
- ✅ Dicionários  
- ✅ Entrada e saída de dados  

---

## 📌 Como executar

1. Tenha o Python 3 instalado.
2. Salve o código em um arquivo `heroi.py`.
3. No terminal, execute:
   ```
   python heroi.py
   ```

---

## 📄 Licença

Este projeto é de uso livre para fins educacionais.

---

Desenvolvido como parte do desafio da **[Digital Innovation One](https://www.dio.me)** 🚀
