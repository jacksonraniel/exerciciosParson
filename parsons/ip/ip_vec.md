---
layout: default
title: Vetores - Estruturas Compostas Homogêneas Unidirecionais
---
# Práticas de vetores com listas em Python

## Problema 1: Imprimir um vetor de trás para frente
Organize os blocos de código para criar um vetor de 4 números predefinidos e imprimir seus valores do último para o primeiro.

<div id="01-sortableTrash" class="sortable-code"></div> 
<div id="01-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="01-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="01-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "vetor = [10, 20, 30, 40]\n" +
    "tamanho = 4\n" +
    "for i in range(tamanho - 1, -1, -1):\n" +
    "    print(vetor[i])";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "01-sortable",
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

## Problema 2: Encontrar o maior valor no vetor
Organize os blocos para criar um algoritmo que encontra e imprime o maior número dentro de um vetor.

<div id="02-sortableTrash" class="sortable-code"></div> 
<div id="02-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="02-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="02-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "vetor = [15, 8, 23, 4, 11]\n" +
    "maior = vetor[0]\n" +
    "for i in range(1, 5):\n" +
    "    if vetor[i] &gt; maior:\n" +
    "        maior = vetor[i]\n" +
    "print(maior)\n" +
    "maior = 0#distractor\n" +
    "if i &gt; maior:#distractor";
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
