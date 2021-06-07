<!DOCTYPE html>
<html>

	<head>
		<meta charset="utf-8">
	<title>Connexion</title>
	<head>
	<body>
		<h1>Bases de données MySQL</h1>  
        <?php
            $servername = 'localhost';
            $username = 'root';
            $password = '';
			$dbname = 'vvalucasc';
            
            //On établit la connexion
            $conn = new mysqli($servername, $username, $password,$dbname);
            
            //On vérifie la connexion
            if($conn->connect_error){
                die('Erreur : ' .$conn->connect_error);
            }
            echo 'Connexion réussie';
        ?>
		<?php
		
		$res = mysqli_query($conn, "SELECT NOINSCRIP,USER,NOACT,DATEINSCRIP,DATEANNULE FROM INSCRIPTION") ;
		

			
		?>
		
		<table border="2" style="width:100%" cellspacing='5'>

  <tr>
    <td>NO INSCRIPTION</td>
    <td>UTILISATEUR</td>
	<td>NO ACTIVITE</td>
	<td>DATE INSCRIPTION</td>
	<td>DATE ANNULE</td>
   
	
  </tr>
<?php while ($ligne = mysqli_fetch_array($res)){ ?>

			<tr>
				<td><?php echo $ligne['NOINSCRIP'];?></td>
				<td><?php echo $ligne['USER'];?></td>
				<td><?php echo $ligne['NOACT'];?></td>
				<td><?php echo $ligne['DATEINSCRIP'];?></td>
				<td><?php echo $ligne['DATEANNULE'];?></td>
			</tr>

		
<?php } ?>
				</table>
		
				
   
		</body>
	
</html>
