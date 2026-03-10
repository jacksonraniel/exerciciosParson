---
layout: default
title: Entrada e saída de dados
---
# Práticas de entrada e saída de dados (I/O)

## Problema 1: Gerador de E-mail
Peça o nome e o domínio da empresa para gerar um e-mail como saída.

<div id="io1-sortableTrash" class="sortable-code"></div> 
<div id="io1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="io1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="io1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "nome = input(&quot;Digite seu nome: &quot;)
\n" +
    "empresa = input(&quot;Digite o domínio da empresa: &quot;)
\n" +
    "print(f&quot;Seu e-mail é: {nome}@{empresa}&quot;)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "io1-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true,
    "trashId": "io1-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#io1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#io1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## Problema 2: Crachá de Evento
Monte um crachá que exiba o nome em uma linha e a categoria (VIP/Estudante) na outra.

<div id="io2-sortableTrash" class="sortable-code"></div> 
<div id="io2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="io2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="io2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "nome = input(&quot;Nome: &quot;)
\n" +
    "tipo = input(&quot;Categoria: &quot;)
\n" +
    "print(&quot;--- CRACHÁ ---&quot;)
\n" +
    "print(f&quot;NOME: {nome}\nSTATUS: {tipo}&quot;)
\n" +
    "input(&quot;Nome: &quot;) = nome
\n" +
    "#distractor
\n" +
    "print(&quot;STATUS: {tipo}&quot;#distractor";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "io2-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true,
    "python3": true,
    "trashId": "io2-sortableTrash"
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#io2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#io2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

### Navegação
[Índice da disciplina](../parsons/ip.html)
[Página inicial](./index.html)
