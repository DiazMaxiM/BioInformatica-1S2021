# Trabajo Practico 2
##### DIAZ, MAXIMILIANO MARTIN
### Reto I:

| **PROCARIOTAS** | **EUCARIOTAS**|
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| ADN localizado en una región: _Nucleoide_, no rodeada por una membrana.                                                                                                                                                      | Núcleo rodeado por una membrana. Material genético fragmentado en cromosomas formados por ADN y proteínas.                                                                                                   |
| Células pequeñas 1-10 µm                                                                                                                                                                                                     | Por lo general células grandes, (10-100 µm), Algunos son microbios, la mayoría son organismos grandes.                                                                                                       |
| División celular directa, principalmente por fisión binaria. No hay centríolos, huso mitótico ni microtúbulos.
Sistemas sexuales escasos, si existe intercambio sexual se da por transferencia de un donador a un receptor. | División celular por mitosis, presenta huso mitótico, o alguna forma de ordenación de microtúbulos.
Sistemas sexuales frecuentes. Alternancia de fases haploides y diploides mediante Meiosis y Fecundación |
| Escasas formas multicelulares<br>Ausencia de desarrollo de tejidos                                                                                                                                                           | Los organismos multicelulares muestran desarrollo de tejidos                                                                                                                                                 |
| Formas anaerobias estrictas, facultativas, microarerofílicas y aerobias                                                                                                                                                      | Casi exclusivamente aerobias                                                                                                                                                                                 |
| Ausencia de mitocondrias: las enzimas para la oxidación de moléculas orgánicas están ligadas a las membranas                                                                                                                 | Las enzimas están en las mitocondrias                                                                                                                                                                        |
| Flagelos simples formados por la proteína flagelina                                                                                                                                                                          | Flagelos compuestos,  (9+2) formados por tubulina y otras proteínas                                                                                                                                          |
| En especies fotosintéticas, las enzimas necesarias están ligadas a las membranas. Exitencia de fotosíntesis aerobia y anaerobia, con productos finales como azufre, sulfato y Oxígeno                                        | Las enzimas para la fotosíntesis se empaquetan en los cloroplastos.                                                                                                                                          |
| ![](http://www.biologia.edu.ar/bacterias/figbac/coli.jpg)                                                                                                                                                                    | ![](http://www.biologia.edu.ar/images/celulas.gif)                                                                                                                                                           |
| _Escherichia coli_ división por fisión binaria. Copyright Dennis Kunkel (MET 92.750x [http://www.pbrc.hawaii.edu/~kunkel/gallery](http://www.pbrc.hawaii.edu/~kunkel/gallery/fungi-sm1/92386a.html), usada con permiso.      | Célula Eucariota                                                                                                                                                                                             |
### Reto II:
```php
$input = readline('Ingrese la cadena de aminoacidos : ');
  
$data = array();
$data['F']=['UUU','UUC'];
$data['L']=['UUA','UUG','CUU','CUC','CUA','CUG'];
$data['C']=['UGU','UGC'];
$data['W']=['UGG'];
$data['P']=['CCU','CCC','CCA','CCG'];
$data['H']=['CAU','CAC'];
$data['Q']=['CAA','CAG'];
$data['R']=['CGU','CGC','CGA','CGG','AGA','AGG'];
$data['I']=['AUU','AUC','AUA'];
$data['T']=['ACU','ACC','ACA','ACG'];
$data['Inicio']=['AUG'];
$data['Stop']=['UAA','UAG','UGA'];
$data['N']=['AAU','AAC'];
$data['K']=['AAA','AAG'];
$data['S']=['AGU','AGC'];
$data['V']=['GUU','GUC','GUA','GUG'];
$data['A']=['GCU','GCC','GCA','GCG'];
$data['G']=['GGU','GGC','GGA','GGG'];
$data['E']=['GAA','GAG'];
$data['D']=['GAU','GAC'];
$data['Y']=['UAU','UAC'];
$output = $data['Inicio'][array_rand($data['Inicio'])];	
$chars = str_split($input);
foreach($chars as $char){
    $output .= $data[$char][array_rand($data[$char])];
}
$output .=$data['Stop'][array_rand($data['Stop'])];	;

echo $output;
```

### Reto III:
```html
<html>
<body>
    <textarea id="texto">
    </textarea>
    <button onclick="resaltar();">Resaltar</button>
    <div id="text">
        <script>
            function resaltar() {
                const csLewisRepeat = document.getElementById("texto").value;
                const repeatRegex = /TATA/g;

                document.getElementById("text").innerHTML = csLewisRepeat.replace(new RegExp(repeatRegex, "gi"), (match) => `</mark>${match}<mark>`);
            }
        </script>

</body>

</html>
```

### Reto IV:
Aprendiendo sobre proteinas [Jugar](https://app.pilas-engine.com.ar/#/proyecto/cfcf18b0-4a9a-43bc-a01d-ffa3ed8abab2?sin_cabecera=true).


