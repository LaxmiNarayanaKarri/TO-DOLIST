<!DOCTYPE html>
<html>
<head>
	<title>TODO LIST</title>
	<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.0.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-EVSTQN3/azprG1Anm3QDgpJLIm9Nao0Yz1ztcQTwFspd3yD65VohhpuuCOmLASjC" crossorigin="anonymous">
	
	<style>
	.divi
	{
	    margin-left:30%;
	}
	.list
	{
	   position:relative;
	   top:4px;
	   left:-4px;
	   height:37px;
	   border-radius:5px;
	   font-size:20px;
	}
	#de
	{
	   font-size:40px;
	   color:red;
	   
	   cursor:pointer;
	}
	h1
	{
	   margin-left:8px;
	}
	</style>
	
</head>
<body>
    <h1>TO DO LIST:</h1>
    <div class="divi">
    	<input type="text"  placeholder="ENTER HERE"   class="list" id="list"  required >
	    <input type="button" class="btn btn-primary" id="sub" value="ADD">
	</div>
	<br>
	<br>
	<table class="table" id="table">
	        <thead class="thread">
	            <tr>
	                <th>CHECK</th>
	                <th>LIST NAME</th>
	                <th>DELETE</th>
	            </tr>
	        </thead>
	        <tbody class="tbody" id="tbody">
	            
	        </tbody>
	</table>
<script>
    let i=document.getElementById('sub');
    i.addEventListener('click',()=>
    {
        var val=document.getElementById("list").value;
        val=val.trimStart();
        if(val.length!=0)
        {
            let table=document.querySelector('tbody');
            let templet=`
                        <tr>
                            <td><input type="button" value="CHECK"  onclick="swap(this)" class="btn btn-primary"></td>
                            <td>${val}</td>
                            <td><i class="far fa-times-circle" id="de" aria-hidden="true" onclick="del(this)"></i></td>
                        </tr>
                        `;
            table.innerHTML=table.innerHTML+templet;
            document.getElementById("list").value='';
             document.getElementById("list").focus();
        }
        else
        {
            alert("PLEASE ENTER THE LIST FIELD");
        }
        
    }
    )
    
</script>
<script src="https://kit.fontawesome.com/5283fdf09a.js" crossorigin="anonymous"></script>
<script>
     function swap(bt)
     {
        bt.value='CHECKED';
        bt.style.color="white";
        bt.style.background="green";
        
      }
      function del(th)
      {
          var row=th.parentNode.parentNode;
          row.parentNode.removeChild(row);
      }
    
</script>
</body>
</html> 
