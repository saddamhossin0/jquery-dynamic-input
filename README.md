# jquery-dynamic-input
<html lang="en">  
<head>  
  <title> Example of Add More Field using the Bootstrap and Jquery </title>  
  <script src="http://ajax.googleapis.com/ajax/libs/jquery/1.9.1/jquery.js"></script>  
  <link rel="stylesheet" href="https://maxcdn.bootstrapcdn.com/bootstrap/3.3.6/css/bootstrap.min.css">  
</head>  
<body>  
  
<div class="container" id="container">  
  <div class="panel panel-default">  
    <div class="panel-heading"> Add More Field using the Bootstrap and Jquery </div>  
    <div class="panel-body">  
  
        <form action="action.php" >  
  
        <div class="input-group control-group " id="after-add-more">  
          <input type="text" name="addmore[]" class="form-control" placeholder="Enter Name Here">  
          <div class="input-group-btn">   
            <button class="btn btn-success add-more" id="add" type="button"><i class="glyphicon glyphicon-plus"></i> Add</button>  
          </div>  
        </div>  
  
        </form>  
  
        <!-- Copy Fields -->  
        <div class="copy hide" id="copy">  
          <div class="control-group input-group" style="margin-top:10px" id="control-group">  
            <input type="text" name="addmore[]" class="form-control" placeholder="Enter Name Here">  
            <div class="input-group-btn">   
              <button class="btn btn-danger remove" id="remove" type="button"><i class="glyphicon glyphicon-remove"></i> Remove</button>  
            </div>  
          </div>  
        </div>  
  
    </div>  
  </div>  
</div>  
  
<script type="text/javascript">  
  
    $(document).ready(function() {  
      $("#add").click(function(){   
          var html = $("#copy").html();  
        var after =  $("#after-add-more").after(html);  
      });  

      $("#container").on("click","#remove",function(){   
          $(this).parents("#control-group").remove();  
      });  
  
    });  
  
</script>  
<script>



    function myFunction() {

        const myText = document.getElementById("test1").innerHTML;
          document.getElementById("demo").innerHTML = myText;

        console.log($('#object').css('display'))
        var x = document.getElementById("product_list");
        console.log(x.style.display === "block")
        if (x.style.display === "block") {
            x.style.display = "none";
        } else {
          x.style.display = "block";
        }


      }
      function myFunction2() {

        const myText = document.getElementById("test2").innerHTML;
          document.getElementById("demo").innerHTML = myText;

        console.log($('#object').css('display'))
        var x = document.getElementById("product_list");
        console.log(x.style.display === "block")
        if (x.style.display === "block") {
            x.style.display = "none";
        } else {
          x.style.display = "block";
        }

      }
      function myFunction3() {

        const myText = document.getElementById("test3").innerHTML;
          document.getElementById("demo").innerHTML = myText;

        console.log($('#object').css('display'))
        var x = document.getElementById("product_list");
        console.log(x.style.display === "block")
        if (x.style.display === "block") {
            x.style.display = "none";
        } else {
          x.style.display = "block";
        }

      }


 </script>
  
</body>  
</html>  
