---
layout: default
title: Week 1 Parsons' Problem
---
# Parsons Practice for Week 1

## <a name="bubblev1"></a> Bubble Sort Version 1 Pseudocode

<div id="bubblev1-sortableTrash" class="sortable-code"></div> 
<div id="bubblev1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="bubblev1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="bubblev1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "n = length of array\n" +
    "For outer_index from 1 to n-1, do:\n" +
    "    For inner_index from 1 to n-1, do:\n" +
    "        first_number = array[inner_index - 1]\n" +
    "        second_number = array[inner_index]\n" +
    "        if first_number &gt; second_number, do:\n" +
    "            swap(first_number, second_number)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "bubblev1-sortable",
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
  $("#bubblev1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#bubblev1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## <a name="insertionv1"></a> Insertion Sort

<div id="insertionv1-sortableTrash" class="sortable-code"></div> 
<div id="insertionv1-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="insertionv1-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="insertionv1-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "n = length of array\n" +
    "For outer_index in Range(from 1 to n-1), do:\n" +
    "   inner_index = outer_index # start with the i-th element\n" +
    "   As long as (inner_index &gt; 0) AND (array[inner_index] &lt; array[inner_index - 1]), do:\n" +
    "       swap(array[inner_index - 1], array[inner_index])\n" +
    "       inner_index = inner_index - 1 ";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "insertionv1-sortable",
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
  $("#insertionv1-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#insertionv1-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## <a name="palindrome"></a> Palindrome Problem

<div id="palindrome-sortableTrash" class="sortable-code"></div> 
<div id="palindrome-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="palindrome-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="palindrome-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def palindrome(s: str) -&gt; bool:\n" +
    "    for idx in range(len(s)//2):\n" +
    "        if s[idx] != s[len(s)-idx-1]:\n" +
    "            return False\n" +
    "    return True";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "palindrome-sortable",
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
  $("#palindrome-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#palindrome-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## <a name="bubblev2"></a> Bubble Sort V2

<div id="bubblev2-sortableTrash" class="sortable-code"></div> 
<div id="bubblev2-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="bubblev2-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="bubblev2-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "n = length of array\n" +
    "swapped = True\n" +
    "As long as swapped is True, do:\n" +
    "  swapped = False\n" +
    "  For inner_index from 1 to n-1, do:\n" +
    "      first_number = array[inner_index - 1]\n" +
    "      second_number = array[inner_index]\n" +
    "      if first_number &gt; second_number, do:\n" +
    "          swap(first_number, second_number)\n" +
    "          swapped = True";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "bubblev2-sortable",
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
  $("#bubblev2-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#bubblev2-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
