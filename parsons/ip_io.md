---
layout: default
title: Entrada e saída de dados
---
# Práticas de entrada e saída de dados (I/O)

## Testando possibilidades

Crie um menu que só para quando o usuário digitar 3. Dentro do loop, apenas mostre o menu e leia a opção.

<div id="11-sortableTrash" class="sortable-code"></div> 
<div id="11-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="11-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="11-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "opcao = 0\n" +
    "while opcao != 3:\n" +
    "    print(&quot;1. Opção A&quot;)\n" +
    "    print(&quot;2. Opção B&quot;)\n" +
    "    print(&quot;3. Sair&quot;)\n" +
    "    opcao = int(input(&quot;Escolha: &quot;))\n" +
    "if opcao == 3:#distractor\n" +
    "print(&quot;Até logo!&quot;)#distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "11-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true,
    "trashId": "11-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#11-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#11-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Problema 1: Gerador de E-mail
Peça o nome e o domínio da empresa para gerar um e-mail como saída.

<div id="parsons-1" class="parsons-problem">
  <script type="text/javascript">
    var initial = "nome = input(\"Digite seu nome: \")\n" +
      "empresa = input(\"Digite o domínio da empresa: \")\n" +
      "print(f\"Seu e-mail é: {nome}@{empresa}\")";
    var p = new ParsonsWidget({
      "sortableId": "parsons-1",
      "grader": ParsonsWidget._graders.LineBasedGrader,
      "lang": "en"
    });
    p.init(initial);
    p.shuffleLines();
  </script>
</div>

## Problema 2: Crachá de Evento
Monte um crachá que exiba o nome em uma linha e a categoria (VIP/Estudante) na outra.

<div id="parsons-2" class="parsons-problem">
  <script type="text/javascript">
    var initial = "nome = input(\"Nome: \")\n" +
      "tipo = input(\"Categoria: \")\n" +
      "print(\"--- CRACHÁ ---\")\n" +
      "print(f\"NOME: {nome}\\nSTATUS: {tipo}\")\n" +
      "input(\"Nome: \") = nome #distractor\n" +
      "print(\"STATUS: {tipo}\") #distractor";
    var p = new ParsonsWidget({
      "sortableId": "parsons-2",
      "max_wrong_lines": 2,
      "grader": ParsonsWidget._graders.LineBasedGrader
    });
    p.init(initial);
    p.shuffleLines();
  </script>
</div>
