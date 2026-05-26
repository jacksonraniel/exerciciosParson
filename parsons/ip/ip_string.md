---
layout: default
title: String - fatiamento e manipulação básica
---
# Práticas de manipulação de Strings em Python

## Problema 1: Inverter e Maiúsculas
Construa uma função grito_invertido(texto) que recebe uma string e a retorna toda em maiúsculas e invertida.

<div id="01-sortableTrash" class="sortable-code"></div> 
<div id="01-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="01-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="01-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def grito_invertido(texto):\n" +
    "    texto_maiusculo = texto.upper()\n" +
    "    texto_invertido = texto_maiusculo[::-1]\n" +
    "    return texto_invertido";
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

## Problema 2: Contador de Vogais
Construa uma função conta_vogais(palavra) que conta quantas vogais (a, e, i, o, u) minúsculas existem na palavra fornecida.

<div id="02-sortableTrash" class="sortable-code"></div> 
<div id="02-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="02-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="02-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def conta_vogais(palavra):\n" +
    "    contador = 0\n" +
    "    for letra in palavra:\n" +
    "        if letra in &quot;aeiou&quot;:\n" +
    "            contador += 1\n" +
    "    return contador\n" +
    "contador = &quot;&quot;#distractor\n" +
    "if letra in &quot;bcdfghjklmnpqrstvwxyz&quot;:#distractor";
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
