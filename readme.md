
Une base de timeline avec utilisation de l'attribut data en HTML5 (HTML5 Custom Data Attributes (data-*)).



Chaque événement comporte un attribut data-date que l'on peut récupérer ou modifier par JavaScript. Un exemple ici tiré de l'excellent article http://html5doctor.com/html5-custom-data-attributes/ montre l'usage de la propriété dataset (qui est préférable même si getAttribute et setAttribute peuvent également être utilisés) :
<pre>
<div id='sunflower' data-leaves='47' data-plant-height='2.4m'></div>

<script>
// 'Getting' data-attributes using dataset
var plant = document.getElementById('sunflower');
var leaves = plant.dataset.leaves; // leaves = 47;

// 'Setting' data-attributes using dataset
var tallness = plant.dataset.plantHeight; // 'plant-height' -> 'plantHeight'
plant.dataset.plantHeight = '3.6m';  // Cracking fertiliser
</script>
</pre>
