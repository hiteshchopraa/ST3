# ST3
<!DOCTYPE html>
<html>
<head>
	<title>Table</title>
	<link rel="stylesheet" href="style.css">
    <style>
    table{
	margin-top: 100px;
	text-align: center;
	color: #fff;
    width:50%;
    	padding: 16px;

}

#show th, #show td{
	padding: 16px;
}

#btna td input{
	width: 100%;

}
#pp
{
    background-color:#ff944d;
    width:150px;

}
#p
{
text-align:center;
}
#body
{
background-color:#b3b3ff;
}
    </style>
</head>
<body id="body">
<div id="p"> Detail Form<div>
<hr>

	<center>
		<table >
			<thead>
				<tr>
					<th> Name</th>
					<td><input type="text" name="fname" id="fname"></td>
				</tr>
			</thead>
			<tbody>
				<tr>
					<th>Mob No.</th>
					<td><input type="text" name="lname" id="lname"></td>
				</tr>
				<tr>
					<th>Email</th>
					<td><input type="text" name="email" id="email"></td>
				</tr>
                <tr>
                </tr>
					 <tr>
                </tr> <tr>
                </tr> <tr>
                </tr> <tr>
                </tr> <tr>
                </tr> <tr>
                </tr>
				
			</tbody>
		</table>
        
        
        <div id="btna">
					<input id="pp"type="button" name="button" id="btn" value="Submit" onclick="AddRow()">
				</div>
        
        
        <hr>

		<table  id="show">
			<thead>
				<tr>
					<th>First Name</th>
					<th>Mob No.</th>
					<th>Email ID</th>
				</tr>
			</thead>
		</table>
	</center>
	
	<script>
		
		var list1 = [];
		var list2 = [];
		var list3 = [];

		var n = 1;
		var x = 0;

		function AddRow(){

			var AddRown = document.getElementById('show');
			var NewRow = AddRown.insertRow(n);

			list1[x] = document.getElementById("fname").value;
			list2[x] = document.getElementById("lname").value;
			list3[x] = document.getElementById("email").value;

			var cel1 = NewRow.insertCell(0);
			var cel2 = NewRow.insertCell(1);
			var cel3 = NewRow.insertCell(2);

			cel1.innerHTML = list1[x];
			cel2.innerHTML = list2[x];
			cel3.innerHTML = list3[x];
            

			n++;
			x++;
		}

	</script>
</body>
</html>
