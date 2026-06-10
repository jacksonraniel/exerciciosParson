---
layout: default
title: Registros - Implementação com Dicionários
---
# Práticas de manipulação de registros (dicionários) em Python

## Problema 1: Acesso Simples

Construa um registro para um livro de fantasia com título, autor e ano, e depois imprima apenas o título usando a chave correta.

<div id="01-sortableTrash" class="sortable-code"></div> 
<div id="01-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="01-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="01-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "livro = {\n" +
    "    &quot;titulo&quot;: &quot;O Hobbit&quot;,\n" +
    "    &quot;autor&quot;: &quot;Tolkien&quot;,\n" +
    "    &quot;ano&quot;: 1937\n" +
    "}\n" +
    "print(livro[&quot;titulo&quot;])";
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

## Problema 2: Busca em Lista de Registros
Complete a função que recebe uma lista de registros de produtos e retorna o nome do produto mais caro.

<div id="02-sortableTrash" class="sortable-code"></div> 
<div id="02-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="02-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="02-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def mais_caro(produtos):\n" +
    "    maior = produtos[0]\n" +
    "    for p in produtos:\n" +
    "        if p[&quot;preco&quot;] &gt; maior[&quot;preco&quot;]:\n" +
    "            maior = p\n" +
    "    return maior[&quot;nome&quot;]\n" +
    "if p[1] &gt; maior[1]:#distractor\n" +
    "return maior#distractor";
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
