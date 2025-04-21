---
layout: default
title: Week 2 Parsons' Problem
---
# Parsons Practice for Week 2

## <a name="maxchild"></a> Max Child for Binary Heap

<div id="max-child-sortableTrash" class="sortable-code"></div> 
<div id="max-child-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="max-child-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="max-child-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def max_child(array: list[int|float], index: int, heap_size: int) -&gt; int:\n" +
    "    if right_of(index) &gt;= heap_size:\n" +
    "        return left_of(index)\n" +
    "    else:\n" +
    "        if array[left_of(index)] &gt; array[right_of(index)]:\n" +
    "            return left_of(index)\n" +
    "        else:\n" +
    "            return right_of(index)";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "max-child-sortable",
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
  $("#max-child-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#max-child-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>

## <a name="minheapify"></a> Min Heapify

<div id="min-heapify-sortableTrash" class="sortable-code"></div> 
<div id="min-heapify-sortable" class="sortable-code"></div> 
<div style="clear:both;"></div> 
<p> 
    <input id="min-heapify-feedbackLink" value="Get Feedback" type="button" /> 
    <input id="min-heapify-newInstanceLink" value="Reset Problem" type="button" /> 
</p> 
<script type="text/javascript"> 
(function(){
  var initial = "def min_heapify(array: list[int|float], index: int, size: int) -&gt; None:\n" +
    "    cur_idx: int = index\n" +
    "    while cur_idx &lt; size:\n" +
    "        min_child_idx: int = min_child(array, cur_idx, size) \n" +
    "        if min_child_idx &lt; size and array[min_child_idx] &lt; array[cur_idx]:\n" +
    "            array[min_child_idx], array[cur_idx] = array[cur_idx], array[min_child_idx]\n" +
    "        cur_idx = min_child_idx";
  var parsonsPuzzle = new ParsonsWidget({
    "sortableId": "min-heapify-sortable",
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
  $("#min-heapify-newInstanceLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.shuffleLines(); 
  }); 
  $("#min-heapify-feedbackLink").click(function(event){ 
      event.preventDefault(); 
      parsonsPuzzle.getFeedback(); 
  }); 
})(); 
</script>
