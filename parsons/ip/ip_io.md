---
layout: default
title: Entrada e saída de dados
---
# Práticas de entrada e saída de dados (I/O)

## Problema 1: Gerador de E-mail
Peça o nome e o domínio da empresa para gerar um e-mail como saída.

<div id="01-sortableTrash" class="sortable-code"></div> 
<div id="01-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="01-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="01-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "nome = input(&quot;Digite seu nome: &quot;)\n" +
    "empresa = input(&quot;Digite o domínio da empresa: &quot;)\n" +
    "print(f&quot;Seu e-mail é: {nome}@{empresa}&quot;)";
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

## Problema 2: Crachá de Evento
Monte um crachá que exiba o nome em uma linha e a categoria (VIP/Estudante) na outra.

<div id="02-sortableTrash" class="sortable-code"></div> 
<div id="02-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="02-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="02-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "nome = input(&quot;Nome: &quot;)\n" +
    "tipo = input(&quot;Categoria: &quot;)\n" +
    "print(&quot;--- CRACHÁ ---&quot;)\n" +
    "print(f&quot;NOME: {nome}\nSTATUS: {tipo}&quot;)\n" +
    "input(&quot;Nome: &quot;) = nome#distractor\n" +
    "print(&quot;STATUS: {tipo}&quot;)#distractor";
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
[Página inicial](./index.html)
