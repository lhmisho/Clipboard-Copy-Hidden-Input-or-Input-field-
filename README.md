# Clipboard-Copy-Hidden-Input-or-Input-field-
A simple HTML and JS code to copy clipboard value on click ...
please input your latest js cdn

# actual html code for input value 
```html
<input type="text" id="myInput" style="display: none" value="Hello World for my new next">
<button id="myBtn" onclick="myFunction()">Copy text</button>
```

# js code for copy hidden link
in this case i put the input field display none at the begining. becaues i want to copy a hidden link.
```js
<script type="text/javascript">
  function myFunction(){
    $("#myBtn").click(function(){
      var link = $("#myInput").val();
      $("#myInput").css('display',  'block');
      $("#myInput").focus();
      $("#myInput").select();
      document.execCommand('copy');
      $("#myInput").css('display',  'none');
      alert("Copied Link: " + link)
    });
  }
  $(document).ready(function(){
    myFunction();
  })    
</script>
```
# code for copy direct input field
if i want to copy without hidden link than i can skip display hidden
```js
<script type="text/javascript">
  function myFunction(){
    function myFunction(){
      var copyLink = document.getElementById('myInput')
      copyLink.select()
      document.execCommand('copy');
      alert("Copied Link: " + copyLink.value)
    }
</script>
```
