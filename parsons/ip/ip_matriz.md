---
layout: default
title: Matrizes - Estruturas compostas homogêneas unidimensionais
---
# Práticas de manipulação de matrizes em Python

## Problema 1: Inicializando uma Matriz identidade 2x2
Organize os blocos de código abaixo para criar uma matriz quadrada identidade de tamanho 2x2 (com 1s na diagonal principal e 0s no restante) e imprimi-la.

<div id="01-sortableTrash" class="sortable-code"></div> 
<div id="01-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="01-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="01-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "matriz = [[1, 0], [0, 1]]\n" +
    "for linha in matriz:\n" +
    "    print(linha)\n" +
    "matriz = [[1, 0] [0, 1]]#distractor\n" +
    "matriz = [1, 0, 0, 1]#distractor\n" +
    "for linha in linha:#distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "01-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true,
    "trashId": "01-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#01-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#01-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Problema 2: Somando todos os elementos de uma Matriz 2x2
Ordene o algoritmo para calcular e exibir a soma total de todos os números presentes em uma matriz 2x2.

<div id="02-sortableTrash" class="sortable-code"></div> 
<div id="02-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="02-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="02-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "matriz = [[5, 10], [15, 20]]\n" +
    "soma = 0\n" +
    "for linha in matriz:\n" +
    "    for elemento in linha:\n" +
    "        soma = soma + elemento\n" +
    "print(soma)\n" +
    "soma = matriz#distractor\n" +
    "soma = soma + linha#distractor\n" +
    "for elemento in matriz:#distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "02-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true,
    "trashId": "02-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#02-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#02-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

### Navegação
[Índice da disciplina](../parsons/ip.html)
[Página inicial](../../index.html)
