# Google Sheets Automation Script

Este repositório contém um conjunto de scripts em Google Apps Script para automação de tarefas em uma planilha do Google Sheets. O código implementa funcionalidades para cadastro de dados, limpeza de formulários e abertura de um dashboard externo.

## Funcionalidades

### 1. **Cadastrar Dados**
A função `cadastrarDados()` lê os dados de um formulário na aba "Formulario" e os insere na aba "BancoDeDados". Antes de salvar, é realizada uma verificação para garantir que todos os campos obrigatórios (da célula D5 até D34) foram preenchidos. Se algum campo estiver vazio, um alerta será exibido solicitando o preenchimento.

### 2. **Limpar Formulário**
A função `limparFormulario()` apaga o conteúdo das células do formulário (intervalo D5:D34) na aba "Formulario", permitindo que o usuário preencha novos dados de forma fácil.

### 3. **Abrir Dashboard**
A função `abrirDashboard()` abre uma nova janela do navegador com um link especificado (atualmente configurado como um link placeholder, que deve ser substituído pelo URL desejado). O link será aberto em uma nova aba, enquanto o diálogo do Google Sheets será fechado.

## Como Utilizar

1. Implemente o script dentro de um documento do Google Sheets.
2. Para cadastrar dados, preencha os campos na aba "Formulario" e acione a função de cadastro.
3. Para limpar o formulário, use a função `limparFormulario()`, que apagará os dados preenchidos.
4. Para acessar o dashboard, a função `abrirDashboard()` abrirá o link configurado em uma nova janela do navegador.

## Objetivo

O objetivo deste script é facilitar o processo de entrada de dados e navegação para dashboards de relatórios ou visualizações externas, tornando a experiência do usuário mais fluida e eficiente dentro do Google Sheets.

---

**Nota:** Substitua o link placeholder na função `abrirDashboard()` pelo URL do seu dashboard real.
