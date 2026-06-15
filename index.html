
<?php
error_reporting(E_ALL);
ini_set('display_errors', 1);

$conn = mysqli_connect("localhost", "root", "", "gestion_etudiants");

if(!$conn){
    die("Erreur connexion DB");
}

/* AJOUTER */
if(isset($_POST['ajouter'])){
    $nom = $_POST['nom'];
    $prenom = $_POST['prenom'];
    $classe = $_POST['classe'];

    mysqli_query($conn,
        "INSERT INTO etudiant(nom, prenom, classe)
        VALUES('$nom', '$prenom', '$classe')"
    );
}

/* SUPPRIMER */
if(isset($_GET['delete'])){
    $id = intval($_GET['delete']);

    mysqli_query($conn,
        "DELETE FROM etudiant WHERE id=$id"
    );
}

/* MODIFIER */
if(isset($_POST['update'])){
    $id = $_POST['id'];
    $nom = $_POST['nom'];
    $prenom = $_POST['prenom'];
    $classe = $_POST['classe'];

    mysqli_query($conn,
        "UPDATE etudiant
        SET nom='$nom', prenom='$prenom', classe='$classe'
        WHERE id=$id"
    );

    // 🔥 reset form
    header("Location: index.php");
    exit();
}

/* GET DATA FOR EDIT */
$edit = null;

if(isset($_GET['edit'])){
    $id = intval($_GET['edit']);
    $res = mysqli_query($conn, "SELECT * FROM etudiant WHERE id=$id");
    $edit = mysqli_fetch_assoc($res);
}
?>

<!DOCTYPE html>
<html>
<head>
    <title>Gestion Etudiants</title>
    <link rel="stylesheet" href="styletud.css">
</head>
<body>

<h1>Gestion des Étudiants</h1>

<!-- FORM -->
<form method="post">

    <input type="hidden" name="id" value="<?php echo $edit['id'] ?? ''; ?>">

    Nom :
    <input type="text" name="nom" value="<?php echo $edit['nom'] ?? ''; ?>" required><br><br>

    Prenom :
    <input type="text" name="prenom" value="<?php echo $edit['prenom'] ?? ''; ?>" required><br><br>

    Classe :
    <input type="text" name="classe" value="<?php echo $edit['classe'] ?? ''; ?>" required><br><br>

    <?php if($edit){ ?>
        <button name="update">Modifier</button>
    <?php } else { ?>
        <button name="ajouter">Ajouter</button>
    <?php } ?>

</form>

<hr>

<h2>Liste des étudiants</h2>

<?php
$result = mysqli_query($conn, "SELECT * FROM etudiant") or die(mysqli_error($conn));
while($row = mysqli_fetch_assoc($result)){
?>

<p>
    <?php echo $row['nom']." ".$row['prenom']." ".$row['classe']; ?>

    <a href="?delete=<?php echo $row['id']; ?>">❌ Supprimer</a>

    <a href="?edit=<?php echo $row['id']; ?>">✏️ Modifier</a>
</p>

<?php } ?>

</body>
</html>

