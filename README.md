<!DOCTYPE html>
<html>
<head>
	<title>BIODATA</title>
</head>
<style type="text/css">
	body, html{
		margin: 10px;
		background-color: #d3d3d3;
	}
	tr, td{
		padding-right: 5px;
	}
	h1{
		font-weight: bold;
	}
	header{
		text-align: center;
		background-color: red;
		padding: 1px;
		color: white;
		font-family: broadway;
	}
	table{
		padding-top: 10px;
		font-size: 15px;
		color: #000000;
		font-weight: bold;
		padding-left: 200px;
		font-family: corbel;
	}
	.edu-bg{
		font-size: 20px;
		font-family: corbel;
	}

</style>
<body>
	<header><h1><center>STUDENT INFORMATION</center></h1></header>
<form method="post" action="info.php" enctype="multipart/form-data">
	 <table>
		<tr>
			<td>
				<label>Name</label> 
			</td>
			<td>
				:<input type="text" name="name" placeholder="Full name" size="40" required>
			</td>
		</tr>
		<tr>
			<td>
				<label>Address</label>  
			</td>
			<td> 
				:<input type="text" name="address" placeholder="Complete Address" size="40" required>
			</td>
		</tr>

		<tr>
			<td>
				<label>Date of Birth</label>  
			</td>
			<td>
				:<input type="text" name="birth_date" placeholder="mm-day-year" size="20" required>
			</td>
			<td> </td>
			<td>
				<label>Religion</label>
			</td>
			<td>
				:<input type="text" name="religion" required>
			</td>
		</tr>

		<tr>
			<td>
				<label>Civil Status</label>  
			</td>
			<td>
				:<input type="text" name="civil" size="20" required>
			</td>
			<td> </td>
			<td>
				<label>Age</label>
			</td>
			<td>
				:<input type="text" name="age"  required>
			</td>
		</tr>
		<tr>
			<td>
				<label>Citizenship</label>  
			</td>
			<td>
				:<input type="text" name="citizenship" size="20" required>
			</td>
			<td> </td>
			<td>
				<label>Weight</label>
			</td>
			<td>
				:<input type="text" name="weight"  required>
			</td>
		</tr>
		<tr>
			<td>
				<label>Place of Birth</label>  
			</td>
			<td>
				:<input type="text" name="birth_place" size="40" required>
			</td>
			<td> </td>
			<td>
				<label>Height</label>
			</td>
			<td>
				:<input type="text" name="height"  required>
			</td>
		</tr>

		<tr>
			<td>
				<label>Name of Father</label> 
			</td>
			<td> 
				:<input type="text" name="father" size="40" placeholder="Complete Name" required>
			</td>
		</tr>
		<tr>
			<td>
				<label>Name of Mother</label>  
			</td>
			<td> 
				:<input type="text" name="mother" size="40" placeholder="Complete Name" required>
			</td>
		</tr>
		<tr>
			<td>
				<label>Dialects Spoken  </label>
			</td>
			<td> 
				:<input type="text" name="dialect" size="40" required>
			</td>
		</tr>
		<tr>
			<td>
				Person to be notified in Case of Emergency
			</td>
			<td> 
				<label>:</label>
				<input type="text" name="emergency" size="40" required>
			</td>
		</tr>
		<tr>
			<td class="edu-bg">
				<u>EDUCATIONAL BACKGROUND:</u>
			</td>
		</tr>
		<tr>
			<tr>
			<td>
				<label>Elementary</label>  
			</td>
			<td>
				:<input type="text" name="elem" size="40" placeholder="Name of School" required>
			</td>
			<td> </td>
			<td>
				<label>Year Graduated</label>
			</td>
			<td>
				:<input type="text" name="ygelem"  required>
			</td>
		</tr>
		<tr>
			<tr>
			<td>
				<label>High School</label>  
			</td>
			<td>
				:<input type="text" name="HS" size="40" placeholder="Name of School" required>
			</td>
			<td> </td>
			<td>
				<label>Year Graduated</label>
			</td>
			<td>
				:<input type="text" name="yghs"  required>
			</td>
		</tr>
		<tr>
			<tr>
			<td>
				<label>College</label>  
			</td>
			<td>
				:<input type="text" name="college" size="40" placeholder="Name of School" required>
			</td>
			<td> </td>
			<td>
				<label>Year Graduated</label>
			</td>
			<td>
				:<input type="text" name="ygcollege"  required>
			</td>
		</tr>
		<tr>
			<td>
				<label>Course</label> 
			</td>
			<td>
				:<input type="text" name="course" size="40" required>
			</td>
			<tr>
			<td>
				<label>Skills</label>  
			</td>
			<td>
				:<input type="text" name="skill" size="40" required>
			</td>
			<tr>
			</tr>
			<tr>
				<td></td>
				<td>
					<button  value="Save Record" name="btnsave" style="width: 150px; margin-top: 15px; height: 30px;">Save Record</button>
				</td>
			</tr>
	</table>
	
	</form>
</body>
</html>


<?php
	

if (isset($_POST['btnsave']))
 {
 
	$name = $_POST['name'];
	$address = $_POST['address'];
	$birthdate = $_POST['birth_date'];
	$civil = $_POST['civil'];
	$citizenship = $_POST['citizenship'];
	$birthplace = $_POST['birth_place'];
	$father = $_POST['father'];
	$mother = $_POST['mother'];
	$dialect = $_POST['dialect'];
	$emergency = $_POST['emergency'];
	$elem = $_POST['elem'];
	$HS = $_POST['HS'];
	$college = $_POST['college'];
	$religion = $_POST['religion'];
	$weight = $_POST['weight'];
	$height = $_POST['height'];
	$age = $_POST['age'];
	$ygelem = $_POST['ygelem'];
	$yghs = $_POST['yghs'];
	$ygcollege = $_POST['ygcollege'];
	$course = $_POST['course'];
	$skill = $_POST['skill'];

	echo "<br>";
	echo "<br>";


	echo "<h1><center>STUDENT INFORMATION</center></h1>";
	echo "<br>";
	echo "<table>";

	echo "<tr>";
	echo "<td>Name</td>";
	echo "<td>:</td>";
	echo "<td>$name</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Address</td>";
	echo "<td>:</td>";
	echo "<td>$address</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Date of Birth</td>";
	echo "<td>:</td>";
	echo "<td>$birthdate</td>";

	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	
	echo "<td>Religion</td>";
	echo "<td>:</td>";
	echo "<td>$religion</td>";
	echo "</tr>";
	

	echo "<tr>";
	echo "<td>Civil Status</td>";
	echo "<td>:</td>";
	echo "<td>$civil</td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td>Age</td>";
	echo "<td>:</td>";
	echo "<td>$age</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Citizenship</td>";
	echo "<td>:</td>";
	echo "<td>$citizenship</td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td>Weight</td>";
	echo "<td>:</td>";
	echo "<td>$weight</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Place of Birth</td>";
	echo "<td>:</td>";
	echo "<td>$birthplace</td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td>Height</td>";
	echo "<td>:</td>";
	echo "<td>$height</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Name of Father</td>";
	echo "<td>:</td>";
	echo "<td>$father</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Name of Mother</td>";
	echo "<td>:</td>";
	echo "<td>$mother</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Dialect Spoken</td>";
	echo "<td>:</td>";
	echo "<td>$dialect</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Person to be notified in Case of Emergency</td>";
	echo "<td>:</td>";
	echo "<td>$emergency</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>";
	echo "<strong><u>EDUCATIONAL BACKGROUND:</u></strong>";
	echo "</td>";
	echo "</tr>";

	echo "<tr>";
	echo "<td>Elementary</td>";
	echo "<td>:</td>";
	echo "<td>$elem</td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td>Year Graduated</td>";
	echo "<td>:</td>";
	echo "<td>$ygelem</td>";
	echo "</tr>";


	echo "<tr>";
	echo "<td>Hish School</td>";
	echo "<td>:</td>";
	echo "<td>$HS</td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td>Year Graduated</td>";
	echo "<td>:</td>";
	echo "<td>$yghs</td>";
	echo "</tr>";


	echo "<tr>";
	echo "<td>College</td>";
	echo "<td>:</td>";
	echo "<td>$college</td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td></td>";
	echo "<td>Year Graduated</td>";
	echo "<td>:</td>";
	echo "<td>$ygcollege</td>";
	echo "</tr>";

	echo "<tr>";
 	echo "<td>Course</td>";
	echo "<td>:</td>";
	echo "<td>$course</td>";
	echo "</tr>";

	echo "<tr>";
 	echo "<td>Skills</td>";
	echo "<td>:</td>";
	echo "<td>$skill</td>";
	echo "</tr>";

	echo "</table>"; 

}

	
	
?>
