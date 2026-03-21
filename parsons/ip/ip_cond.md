---
layout: default
title: Estruturas de controle condicional
---
# Práticas de estruturas de controle condicional

## Problema 1: Par ou Ímpar
Ordene os blocos de código para criar um programa que verifica se um número "n" é par ou ímpar.

<div id="001-sortableTrash" class="sortable-code"></div> 
<div id="001-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="001-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="001-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "if n % 2 == 0:
\n" +
    "    print(&quot;Par&quot;)
\n" +
    "else:
\n" +
    "    print(&quot;Ímpar&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "001-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#001-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#001-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Problema 2: Maioridade Penal
Monte a estrutura correta para verificar se a pessoa é maior de idade, menor de idade ou bebê (menor do que 2 anos).
<div id="002-sortableTrash" class="sortable-code"></div> 
<div id="002-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="002-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="002-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "if idade &lt; 2:
\n" +
    "    print(&quot;Bebê&quot;)
\n" +
    "elif idade &lt; 18:
\n" +
    "    print(&quot;Menor&quot;)
\n" +
    "else:
\n" +
    "    print(&quot;Maior&quot;)
\n" +
    "elif idade &gt;= 18:
\n" +
    "#distractor
\n" +
    "match:
\n" +
    "#distractor
\n" +
    "else idade &gt;= 18:#distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "002-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true,
    "trashId": "002-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#002-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#002-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

### Navegação
[Índice da disciplina](../parsons/ip.html)

[Página inicial](../../index.html)
