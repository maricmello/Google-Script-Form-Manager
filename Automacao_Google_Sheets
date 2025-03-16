function cadastrarDados() {
  var planilhaFormulario = SpreadsheetApp.getActiveSpreadsheet().getSheetByName('Formulario');
  var dados = planilhaFormulario.getRange('D5:D34').getValues();

  // Verificar se há dados faltando
  for (let i = 0; i < dados.length; i++) {
    if (!dados[i][0]) {
      SpreadsheetApp.getUi().alert('Preencha todos os campos obrigatórios.');
      return;
    }
  }

  var planilhaBanco = SpreadsheetApp.getActiveSpreadsheet().getSheetByName('BancoDeDados');
  var ultimaLinha = planilhaBanco.getLastRow();
  var linhaAlvo = ultimaLinha + 1;

  // Inserir dados no banco de dados
  planilhaBanco.getRange(linhaAlvo, 1, 1, dados.length).setValues([dados]);
}

function limparFormulario() {
  var planilhaFormulario = SpreadsheetApp.getActiveSpreadsheet().getSheetByName('Formulario');
  planilhaFormulario.getRange('D5:D34').clearContent();
}

function abrirDashboard() {
  var url = "https://seu-link-aqui.com"; // Substitua pelo link desejado
  var htmlOutput = HtmlService.createHtmlOutput('<html><script>window.open("' + url + '");google.script.host.close();</script></html>');
  SpreadsheetApp.getUi().showModalDialog(htmlOutput, 'Abrindo Dashboard');
}
