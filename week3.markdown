---
layout: default
title: Week 3 Parsons' Problem
---
# Parsons Practice for Week 3

## <a name="factorial"></a> Factorial

<div id="factorial-recursion-sortableTrash" class="sortable-code"></div> 
<div id="factorial-recursion-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="factorial-recursion-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="factorial-recursion-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def factorial_recursion(n: int) -&gt; int:\n" +
    "    if n == 1 or n == 0:\n" +
    "        return 1\n" +
    "    else:\n" +
    "        return n * factorial_recursion(n - 1)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "factorial-recursion-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#factorial-recursion-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#factorial-recursion-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## <a name="fibonacci-recursive"></a> Fibonacci Recursive

<div id="fibonacci-recursive-sortableTrash" class="sortable-code"></div> 
<div id="fibonacci-recursive-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="fibonacci-recursive-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="fibonacci-recursive-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def fibonacci(index: int) -&gt; int:\n" +
    "    if index == 0:\n" +
    "        return 0\n" +
    "    elif index == 1:\n" +
    "        return 1\n" +
    "    else:\n" +
    "        return fibonacci(index - 1) + fibonacci(index - 2)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "fibonacci-recursive-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#fibonacci-recursive-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#fibonacci-recursive-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## <a name="max-heapify"></a> Max Heapify

<div id="max-heapify-sortableTrash" class="sortable-code"></div> 
<div id="max-heapify-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="max-heapify-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="max-heapify-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def max_heapify(array: list, index: int, heap_size: int) -&gt; None:\n" +
    "    left_idx: int = left_of(index)\n" +
    "    right_idx: int = right_of(index) \n" +
    "    if (left_idx &lt; heap_size) and (array[left_idx] &gt; array[index]):\n" +
    "        largest: int = left_idx\n" +
    "    else:\n" +
    "        largest = index\n" +
    "    if (right_idx &lt; heap_size) and (array[right_idx] &gt; array[largest]):\n" +
    "        largest = right_idx\n" +
    "    if largest != index:\n" +
    "        array[index], array[largest] = array[largest], array[index]\n" +
    "        max_heapify(array, largest, heap_size)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "max-heapify-sortable",
    "max_wrong_lines": 10,
    "grader": ParsonsWidget._graders.LineBasedGrader,
    "exec_limit": 2500,
    "can_indent": true,
    "x_indent": 50,
    "lang": "en",
    "show_feedback": true
  });
  parsonsPuzzle.init(initial);
  parsonsPuzzle.shuffleLines();
  $("#max-heapify-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#max-heapify-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
