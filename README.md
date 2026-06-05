<?php

$servidor = "localhost";
$usuario = "root";
$contrasena = "";
$basedatos = "tienda";

// Crear conexión
$conexion = mysqli_connect($servidor, $usuario, $contrasena, $basedatos);

// Verificar conexión
if (!$conexion) {
    die("Error de conexión: " . mysqli_connect_error());
}

echo "<h2>Conexión exitosa a la base de datos 'tienda'</h2>";

mysqli_close($conexion);

?>
