# 💱 Missão 05 - Operação Global Exchange

## 📖 Sobre o Projeto

O **Global Exchange** é um conversor de moedas desenvolvido em C# utilizando .NET Console Application.

O objetivo do projeto é converter valores em Reais (BRL) para Dólares (USD), aplicando conceitos de **Interação Humano-Computador (IHC)** e **Experiência do Usuário (UX)** através das Heurísticas de Nielsen.

Durante a execução, o sistema fornece feedback visual ao usuário, trata erros de entrada e apresenta os resultados de forma organizada e intuitiva.

---

## 🎯 Objetivos

* Desenvolver uma aplicação de console funcional.
* Aplicar conceitos de UX em um sistema baseado em terminal.
* Implementar tratamento de erros utilizando `try-catch`.
* Fornecer feedback visual durante o processamento.
* Exibir resultados de maneira clara e organizada.

---

## 🛠️ Tecnologias Utilizadas

* C#
* .NET SDK
* Visual Studio Code
* Terminal (CMD/PowerShell)
* Git
* GitHub

---

## 📂 Estrutura do Projeto

```text
una-ihcux-lista05/
│
├── ConversorExpert/
│   ├── Program.cs
│   ├── ConversorExpert.csproj
│   └── obj/
│
├── evidencia-final.png
└── README.md
```

---

## 🚀 Funcionalidades

O sistema permite:

* Informar um valor em Reais.
* Informar a cotação atual do Dólar.
* Converter automaticamente o valor para USD.
* Exibir mensagens de carregamento simulando comunicação com um sistema financeiro.
* Mostrar o resultado com duas casas decimais.
* Tratar erros de entrada sem encerrar o programa abruptamente.

---

## 💡 Heurísticas de Nielsen Aplicadas

### 1. Visibilidade do Status do Sistema

O usuário recebe informações constantes sobre o andamento do processo.

Exemplo:

```text
[SISTEMA]: Conectando ao Banco Central...
[SISTEMA]: Calculando taxas...
```

Isso evita que o usuário pense que o programa travou ou deixou de responder.

---

### 5. Prevenção de Erros

O sistema utiliza o bloco `try-catch` para capturar erros de entrada.

Exemplo:

```text
[ERRO CRÍTICO]

Entrada inválida!
Use apenas números e vírgula para decimais.
```

Assim, o programa permanece estável e fornece orientações claras ao usuário.

---

### 8. Estética e Design Minimalista

As informações são exibidas de forma simples, organizada e objetiva.

Exemplo:

```text
-------------------------------------------
VALOR CONVERTIDO: $ 19.23 (Dólares)
-------------------------------------------
```

O uso de cores e separadores melhora a legibilidade sem sobrecarregar a interface.

---

## 🔧 Recursos Utilizados

### Thread.Sleep()

Responsável por simular o tempo de processamento e fornecer feedback visual.

```csharp
Thread.Sleep(1000);
```

### Try-Catch

Utilizado para capturar erros e impedir o encerramento inesperado da aplicação.

```csharp
try
{
    // Código principal
}
catch(Exception)
{
    // Tratamento do erro
}
```

### Formatação de Valores

O resultado da conversão é exibido com duas casas decimais.

```csharp
resultado:F2
```

Exemplo:

```text
$ 19.23
```

---

## ▶️ Como Executar

1. Abra o terminal.
2. Navegue até a pasta do projeto:

```bash
cd ConversorExpert
```

3. Execute a aplicação:

```bash
dotnet run
```

4. Informe:

   * Valor em Reais.
   * Cotação atual do Dólar.

5. Visualize o resultado da conversão.

---

## 📸 Evidência de Execução

Adicionar abaixo a captura de tela mostrando:

* A mensagem "Conectando ao Banco Central..."
* O cálculo das taxas
* O resultado final da conversão

```markdown
![Sistema em execução](./evidencia-final.png)
```

---

## 🧠 Reflexão de Encerramento

### Pergunta

**Após passar por essas 4 missões, como a sua visão sobre "apenas escrever código" mudou ao considerar a experiência de quem vai usar o seu programa?**

### Resposta

Ao longo das atividades, percebi que desenvolver software não significa apenas escrever código que funcione corretamente. Um sistema pode estar tecnicamente perfeito, mas ainda gerar dificuldades para o usuário caso não forneça feedback adequado, não trate erros ou apresente informações de forma confusa.

Aprendi que a experiência do usuário deve ser considerada desde o início do desenvolvimento. Mensagens de status, tratamento amigável de erros e interfaces organizadas tornam o software mais intuitivo, confiável e agradável de utilizar.

Essas missões mostraram que um bom desenvolvedor precisa pensar não apenas na lógica do programa, mas também em como as pessoas irão interagir com ele.

---

## 📚 Aprendizados

Durante esta atividade foi possível aprender:

* Criação de aplicações Console com .NET.
* Utilização do .NET CLI.
* Tratamento de exceções com `try-catch`.
* Uso de `Thread.Sleep()` para feedback visual.
* Aplicação prática das Heurísticas de Nielsen.
* Importância da UX no desenvolvimento de software.

---

## 👩‍💻 Autora

**Ludmilla Santos**

Estudante de Ciência da Computação

Projeto desenvolvido para a disciplina de Interação Humano-Computador (IHC).
