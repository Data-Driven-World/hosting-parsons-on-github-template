---
layout: default
title: Week 1 Parsons' Problem
---
# Parsons Practice for Week 1

## Bubble Sort Version 1 Pseudocode

<div id="sortableTrash" class="sortable-code"></div> 
<div id="sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="feedbackLink" value="Get Feedback" type="button" /> 
    <input id="newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "1. n = length of array\n" +
    "2. For outer_index from 1 to n-1, do:\n" +
    "    2.1 For inner_index from 1 to n-1, do:\n" +
    "        2.1.1 first_number = array[inner_index - 1]\n" +
    "        2.1.2 second_number = array[inner_index]\n" +
    "        2.1.3 if first_number &gt; second_number, do:\n" +
    "            2.1.3.1 swap(first_number, second_number)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "sortable",
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
  $("#newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
