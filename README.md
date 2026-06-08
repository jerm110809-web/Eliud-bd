<?php
$servidor = "localhost";
$usuario = "root";
$contraseña = "";
$basedatos = "tienda";

$conexion = mysqli_connect($servidor, $usuario, $contraseña, $basedatos);

if (!$conexion) {
    die("Error de conexión: " . mysqli_connect_error());
}

echo "<h2>Conexión exitosa a la base de datos 'tienda'</h2>
