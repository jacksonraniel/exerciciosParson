layout: default
title: Entrada e saída de dados
---
# Práticas de entrada e saída de dados (I/O)

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
