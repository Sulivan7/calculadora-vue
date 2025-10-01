# 🧮 Calculadora Vue

Uma calculadora simples e elegante construída com Vue.js 3 e Bootstrap, oferecendo operações matemáticas básicas com uma interface intuitiva e responsiva.

## ✨ Funcionalidades

- ➕ **Adição** - Soma de dois números
- ➖ **Subtração** - Diferença entre dois números
- ✖️ **Multiplicação** - Produto de dois números
- ➗ **Divisão** - Divisão com validação para evitar divisão por zero
- 🎨 **Interface Responsiva** - Design adaptável para diferentes dispositivos
- ⚡ **Resultados em Tempo Real** - Cálculos instantâneos conforme você digita

## 🛠️ Tecnologias Utilizadas

- **Vue.js**
- **Vite**
- **Bootstrap 5**
- **JavaScript ES6+**

## 📁 Estrutura do Projeto

```
calculadora-vue/
├── public/
│   └── favicon.ico
├── src/
│   ├── components/
│   │   ├── Cabecalho.vue
│   │   └── Formulario.vue
│   ├── App.vue
│   └── main.js
├── index.html
├── package.json
├── vite.config.js
└── README.md
```

## 🚀 Como Executar o Projeto

### Pré-requisitos

- Node.js (versão 16 ou superior)
- npm ou yarn

### Instalação

1. **Clone o repositório**

```bash
git clone https://github.com/Sulivan7/calculadora-vue.git
cd calculadora-vue
```

2. **Instale as dependências**

```bash
npm install
```

3. **Execute o projeto em modo de desenvolvimento**

```bash
npm run dev
```

4. **Acesse a aplicação**
   - Abra seu navegador e vá para `http://localhost:5173`

### Build para Produção

```bash
npm run build
```

### Preview da Build de Produção

```bash
npm run preview
```

## 🎯 Como Usar

1. **Digite dois números** nos campos de entrada
2. **Selecione a operação** desejada no menu dropdown:
   - Adição (+)
   - Subtração (-)
   - Multiplicação (\*)
   - Divisão (/)
3. **Veja o resultado** calculado automaticamente abaixo do formulário

### Tratamento de Erros

- A aplicação previne divisão por zero, exibindo uma mensagem de erro apropriada
- Apenas números são aceitos nos campos de entrada
