### The Practice of jQuery

jQuery is a JavaScript library designed to simplify HTML DOM tree traversal and manipulation, as well as event handling, CSS animation, and Ajax. It is free, open-source software using the permissive MIT License. As of May 2019, jQuery is used by 73% of the 10 million most popular websites. Web analysis indicates that it is the most widely deployed JavaScript library by a large margin, having 3 to 4 times more usage than any other JavaScript library.

```markdown
Example1

<script>
  $(document).ready(function() {
    $("#target1").css("color", "red");
    $("#target1").prop("disabled", true);
    $("#target4").remove();
    $("#target2").appendTo("#right-well");
    $("#target5").clone().appendTo("#left-well");
    $("#target1").parent().css("background-color", "red");
    $("#right-well").children().css("color", "orange");
    $("#left-well").children().css("color", "green");
    $(".target:nth-child(2)").addClass("animated bounce");
    $(".target:even").addClass("animated shake");

  });
</script>

<!-- Only change code above this line. -->

<div class="container-fluid">
  <h3 class="text-primary text-center">jQuery Playground</h3>
  <div class="row">
    <div class="col-xs-6">
      <h4>#left-well</h4>
      <div class="well" id="left-well">
        <button class="btn btn-default target" id="target1">#target1</button>
        <button class="btn btn-default target" id="target2">#target2</button>
        <button class="btn btn-default target" id="target3">#target3</button>
      </div>
    </div>
    <div class="col-xs-6">
      <h4>#right-well</h4>
      <div class="well" id="right-well">
        <button class="btn btn-default target" id="target4">#target4</button>
        <button class="btn btn-default target" id="target5">#target5</button>
        <button class="btn btn-default target" id="target6">#target6</button>
      </div>
    </div>
  </div>
</div>

```

<html>
  <script type="text/javascript">
  $(document).ready(function(){
    $("button").addClass("animated bounce");
    $("button").click(function(){
      var color = this.value;
        $("body").css("background-color", color);
    });
  });
  </script>
  <div class="container-fluid">
    <h3 class="text-primary text-center"></h3>
    <div class="row">
      <div class="col-xs-6">
        <div class="well" id="left-well">
        </div>
      </div>
      <div class="col-xs-6">
        <h4>Change the color of background</h4>
        <div class="well" id="right-well">
        <button style="background-color:black" value="black" id="t1">recover</button>
        <button style="background-color:white" value="white" id="t2">change</button>
      </div>
    </div>
  </div>
  <script>
    $(document).ready(function() {
      $("#target1").css("color", "red");
      $("#target1").prop("disabled", true);
      $("#target4").remove();
      $("#target2").appendTo("#right-well");
      $("#target5").clone().appendTo("#left-well");
      $("#target1").parent().css("background-color", "red");
      $("#right-well").children().css("color", "orange");
      $("#left-well").children().css("color", "green");
      $(".target:nth-child(2)").addClass("animated bounce");
      $(".target:even").addClass("animated shake");
    });
  </script>

  <!-- Only change code above this line. -->

  <div class="container-fluid">
    <h3 class="text-primary text-center">jQuery Playground</h3>
    <div class="row">
      <div class="col-xs-6">
        <h4>#left-well</h4>
        <div class="well" id="left-well">
          <button class="btn btn-default target" id="target1">#target1</button>
          <button class="btn btn-default target" id="target2">#target2</button>
          <button class="btn btn-default target" id="target3">#target3</button>
        </div>
      </div>
      <div class="col-xs-6">
        <h4>#right-well</h4>
        <div class="well" id="right-well">
          <button class="btn btn-default target" id="target4">#target4</button>
          <button class="btn btn-default target" id="target5">#target5</button>
          <button class="btn btn-default target" id="target6">#target6</button>
        </div>
      </div>
    </div>
  </div>
</html>
