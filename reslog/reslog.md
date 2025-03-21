# CSCI 1430 Results Log

## Required homework items

Report your classification performance for the three recognition pipelines:

Accuracy (tiny images + nearest neighbor): 21.867%

Accuracy (bag of words + nearest neighbor): 54.267%

Accuracy (bag of words + one vs. all linear SVM): 56.733%

Full confusion matrix and table of classifier results:

<!DOCTYPE html>
<html>
<head>
<link href=http://fonts.googleapis.com/css?family=Nunito:300|Crimson+Text|Droid+Sans+Mono rel=stylesheet type=text/css>
<style type="text/css">
body {
  margin: 0px;
  width: 100%;
  font-family: Crimson Text, serif;
  background: #fcfcfc;
}
table td {
  text-align: center;
  vertical-align: middle;
}
h1 {
  font-family: Nunito, sans-serif;
  font-weight: normal;
  font-size: 28px;
  margin: 25px 0px 0px 0px;
  text-transform: lowercase;
}
.container {
  margin: 0px auto 0px auto;
  width: 1160px;
}
</style>
</head>
<body>

<div class="container">


<center>
<h1>Scene classification results visualization</h1>
<img src="confusion_matrix.png">

<br>
Accuracy (mean of diagonal of confusion matrix) is 0.567
<p>

<table border=0 cellpadding=4 cellspacing=1>
<tr>
<th>Category name</th>
<th>Accuracy</th>
<th colspan=2>Sample training images</th>
<th colspan=2>Sample true positives</th>
<th colspan=2>False positives with true label</th>
<th colspan=2>False negatives with wrong predicted label</th>
</tr>
<tr>
<td>Kitchen</td>
<td>0.590</td>
<td bgcolor=LightBlue><img src="thumbnails/Kitchen_image_0079.jpg" width=75 height=56></td>
<td bgcolor=LightBlue><img src="thumbnails/Kitchen_image_0066.jpg" width=75 height=53></td>
<td bgcolor=LightGreen><img src="thumbnails/Kitchen_image_0194.jpg" width=75 height=56></td>
<td bgcolor=LightGreen><img src="thumbnails/Kitchen_image_0070.jpg" width=75 height=50></td>
<td bgcolor=LightCoral><img src="thumbnails/Kitchen_image_0133.jpg" width=75 height=75><br><small>InsideCity</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Kitchen_image_0056.jpg" width=75 height=50><br><small>Bedroom</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Kitchen_image_0021.jpg" width=75 height=56><br><small>Office</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Kitchen_image_0207.jpg" width=75 height=56><br><small>TallBuilding</small></td>
</tr>
<tr>
<td>Store</td>
<td>0.470</td>
<td bgcolor=LightBlue><img src="thumbnails/Store_image_0298.jpg" width=75 height=56></td>
<td bgcolor=LightBlue><img src="thumbnails/Store_image_0282.jpg" width=75 height=85></td>
<td bgcolor=LightGreen><img src="thumbnails/Store_image_0033.jpg" width=75 height=59></td>
<td bgcolor=LightGreen><img src="thumbnails/Store_image_0124.jpg" width=75 height=50></td>
<td bgcolor=LightCoral><img src="thumbnails/Store_image_0221.jpg" width=75 height=55><br><small>Industrial</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Store_image_0052.jpg" width=75 height=75><br><small>Street</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Store_image_0043.jpg" width=75 height=56><br><small>InsideCity</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Store_image_0196.jpg" width=75 height=56><br><small>Mountain</small></td>
</tr>
<tr>
<td>Bedroom</td>
<td>0.140</td>
<td bgcolor=LightBlue><img src="thumbnails/Bedroom_image_0213.jpg" width=75 height=50></td>
<td bgcolor=LightBlue><img src="thumbnails/Bedroom_image_0179.jpg" width=75 height=60></td>
<td bgcolor=LightGreen><img src="thumbnails/Bedroom_image_0122.jpg" width=75 height=56></td>
<td bgcolor=LightGreen><img src="thumbnails/Bedroom_image_0047.jpg" width=75 height=56></td>
<td bgcolor=LightCoral><img src="thumbnails/Bedroom_image_0146.jpg" width=75 height=75><br><small>TallBuilding</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Bedroom_image_0118.jpg" width=75 height=100><br><small>Kitchen</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Bedroom_image_0064.jpg" width=75 height=55><br><small>Kitchen</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Bedroom_image_0170.jpg" width=75 height=61><br><small>LivingRoom</small></td>
</tr>
<tr>
<td>LivingRoom</td>
<td>0.080</td>
<td bgcolor=LightBlue><img src="thumbnails/LivingRoom_image_0255.jpg" width=75 height=57></td>
<td bgcolor=LightBlue><img src="thumbnails/LivingRoom_image_0211.jpg" width=75 height=81></td>
<td bgcolor=LightGreen><img src="thumbnails/LivingRoom_image_0183.jpg" width=75 height=47></td>
<td bgcolor=LightGreen><img src="thumbnails/LivingRoom_image_0042.jpg" width=75 height=54></td>
<td bgcolor=LightCoral><img src="thumbnails/LivingRoom_image_0068.jpg" width=75 height=76><br><small>Bedroom</small></td>
<td bgcolor=LightCoral><img src="thumbnails/LivingRoom_image_0142.jpg" width=75 height=60><br><small>Bedroom</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/LivingRoom_image_0126.jpg" width=75 height=100><br><small>Office</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/LivingRoom_image_0046.jpg" width=75 height=56><br><small>Street</small></td>
</tr>
<tr>
<td>Office</td>
<td>0.940</td>
<td bgcolor=LightBlue><img src="thumbnails/Office_image_0156.jpg" width=75 height=53></td>
<td bgcolor=LightBlue><img src="thumbnails/Office_image_0211.jpg" width=75 height=54></td>
<td bgcolor=LightGreen><img src="thumbnails/Office_image_0024.jpg" width=75 height=51></td>
<td bgcolor=LightGreen><img src="thumbnails/Office_image_0117.jpg" width=75 height=58></td>
<td bgcolor=LightCoral><img src="thumbnails/Office_image_0191.jpg" width=75 height=56><br><small>LivingRoom</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Office_image_0009.jpg" width=75 height=56><br><small>Kitchen</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Office_image_0108.jpg" width=75 height=42><br><small>Kitchen</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Office_image_0012.jpg" width=75 height=65><br><small>Kitchen</small></td>
</tr>
<tr>
<td>Industrial</td>
<td>0.440</td>
<td bgcolor=LightBlue><img src="thumbnails/Industrial_image_0036.jpg" width=75 height=50></td>
<td bgcolor=LightBlue><img src="thumbnails/Industrial_image_0253.jpg" width=75 height=56></td>
<td bgcolor=LightGreen><img src="thumbnails/Industrial_image_0247.jpg" width=75 height=100></td>
<td bgcolor=LightGreen><img src="thumbnails/Industrial_image_0222.jpg" width=75 height=100></td>
<td bgcolor=LightCoral><img src="thumbnails/Industrial_image_0118.jpg" width=75 height=74><br><small>Store</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Industrial_image_0135.jpg" width=75 height=50><br><small>Bedroom</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Industrial_image_0254.jpg" width=75 height=56><br><small>InsideCity</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Industrial_image_0221.jpg" width=75 height=55><br><small>Store</small></td>
</tr>
<tr>
<td>Suburb</td>
<td>0.620</td>
<td bgcolor=LightBlue><img src="thumbnails/Suburb_image_0208.jpg" width=75 height=50></td>
<td bgcolor=LightBlue><img src="thumbnails/Suburb_image_0097.jpg" width=75 height=50></td>
<td bgcolor=LightGreen><img src="thumbnails/Suburb_image_0137.jpg" width=75 height=50></td>
<td bgcolor=LightGreen><img src="thumbnails/Suburb_image_0236.jpg" width=75 height=50></td>
<td bgcolor=LightCoral><img src="thumbnails/Suburb_image_0153.jpg" width=75 height=75><br><small>OpenCountry</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Suburb_image_0396.jpg" width=75 height=75><br><small>OpenCountry</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Suburb_image_0223.jpg" width=75 height=50><br><small>Forest</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Suburb_image_0075.jpg" width=75 height=50><br><small>Coast</small></td>
</tr>
<tr>
<td>InsideCity</td>
<td>0.460</td>
<td bgcolor=LightBlue><img src="thumbnails/InsideCity_image_0102.jpg" width=75 height=75></td>
<td bgcolor=LightBlue><img src="thumbnails/InsideCity_image_0155.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/InsideCity_image_0231.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/InsideCity_image_0237.jpg" width=75 height=75></td>
<td bgcolor=LightCoral><img src="thumbnails/InsideCity_image_0087.jpg" width=75 height=51><br><small>Industrial</small></td>
<td bgcolor=LightCoral><img src="thumbnails/InsideCity_image_0035.jpg" width=75 height=75><br><small>Highway</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/InsideCity_image_0145.jpg" width=75 height=75><br><small>Kitchen</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/InsideCity_image_0095.jpg" width=75 height=75><br><small>Office</small></td>
</tr>
<tr>
<td>TallBuilding</td>
<td>0.610</td>
<td bgcolor=LightBlue><img src="thumbnails/TallBuilding_image_0184.jpg" width=75 height=75></td>
<td bgcolor=LightBlue><img src="thumbnails/TallBuilding_image_0130.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/TallBuilding_image_0209.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/TallBuilding_image_0126.jpg" width=75 height=75></td>
<td bgcolor=LightCoral><img src="thumbnails/TallBuilding_image_0020.jpg" width=75 height=75><br><small>Street</small></td>
<td bgcolor=LightCoral><img src="thumbnails/TallBuilding_image_0227.jpg" width=75 height=51><br><small>LivingRoom</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/TallBuilding_image_0146.jpg" width=75 height=75><br><small>Bedroom</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/TallBuilding_image_0084.jpg" width=75 height=75><br><small>Coast</small></td>
</tr>
<tr>
<td>Street</td>
<td>0.650</td>
<td bgcolor=LightBlue><img src="thumbnails/Street_image_0033.jpg" width=75 height=75></td>
<td bgcolor=LightBlue><img src="thumbnails/Street_image_0092.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Street_image_0179.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Street_image_0143.jpg" width=75 height=75></td>
<td bgcolor=LightCoral><img src="thumbnails/Street_image_0225.jpg" width=75 height=75><br><small>InsideCity</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Street_image_0179.jpg" width=75 height=75><br><small>InsideCity</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Street_image_0021.jpg" width=75 height=75><br><small>Highway</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Street_image_0024.jpg" width=75 height=75><br><small>Highway</small></td>
</tr>
<tr>
<td>Highway</td>
<td>0.640</td>
<td bgcolor=LightBlue><img src="thumbnails/Highway_image_0111.jpg" width=75 height=75></td>
<td bgcolor=LightBlue><img src="thumbnails/Highway_image_0097.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Highway_image_0146.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Highway_image_0255.jpg" width=75 height=75></td>
<td bgcolor=LightCoral><img src="thumbnails/Highway_image_0118.jpg" width=75 height=75><br><small>Street</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Highway_image_0024.jpg" width=75 height=75><br><small>Street</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Highway_image_0036.jpg" width=75 height=75><br><small>Coast</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Highway_image_0245.jpg" width=75 height=75><br><small>OpenCountry</small></td>
</tr>
<tr>
<td>OpenCountry</td>
<td>0.270</td>
<td bgcolor=LightBlue><img src="thumbnails/OpenCountry_image_0095.jpg" width=75 height=75></td>
<td bgcolor=LightBlue><img src="thumbnails/OpenCountry_image_0226.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/OpenCountry_image_0022.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/OpenCountry_image_0380.jpg" width=75 height=75></td>
<td bgcolor=LightCoral><img src="thumbnails/OpenCountry_image_0236.jpg" width=75 height=75><br><small>Highway</small></td>
<td bgcolor=LightCoral><img src="thumbnails/OpenCountry_image_0024.jpg" width=75 height=75><br><small>Coast</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/OpenCountry_image_0119.jpg" width=75 height=75><br><small>Coast</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/OpenCountry_image_0347.jpg" width=75 height=75><br><small>Forest</small></td>
</tr>
<tr>
<td>Coast</td>
<td>0.870</td>
<td bgcolor=LightBlue><img src="thumbnails/Coast_image_0132.jpg" width=75 height=75></td>
<td bgcolor=LightBlue><img src="thumbnails/Coast_image_0221.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Coast_image_0179.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Coast_image_0026.jpg" width=75 height=75></td>
<td bgcolor=LightCoral><img src="thumbnails/Coast_image_0384.jpg" width=75 height=75><br><small>OpenCountry</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Coast_image_0079.jpg" width=75 height=50><br><small>Suburb</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Coast_image_0181.jpg" width=75 height=75><br><small>Mountain</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Coast_image_0009.jpg" width=75 height=75><br><small>OpenCountry</small></td>
</tr>
<tr>
<td>Mountain</td>
<td>0.760</td>
<td bgcolor=LightBlue><img src="thumbnails/Mountain_image_0241.jpg" width=75 height=75></td>
<td bgcolor=LightBlue><img src="thumbnails/Mountain_image_0144.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Mountain_image_0194.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Mountain_image_0344.jpg" width=75 height=75></td>
<td bgcolor=LightCoral><img src="thumbnails/Mountain_image_0195.jpg" width=75 height=48><br><small>Store</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Mountain_image_0224.jpg" width=75 height=78><br><small>Industrial</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Mountain_image_0030.jpg" width=75 height=75><br><small>Coast</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Mountain_image_0142.jpg" width=75 height=75><br><small>Forest</small></td>
</tr>
<tr>
<td>Forest</td>
<td>0.970</td>
<td bgcolor=LightBlue><img src="thumbnails/Forest_image_0266.jpg" width=75 height=75></td>
<td bgcolor=LightBlue><img src="thumbnails/Forest_image_0214.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Forest_image_0319.jpg" width=75 height=75></td>
<td bgcolor=LightGreen><img src="thumbnails/Forest_image_0091.jpg" width=75 height=75></td>
<td bgcolor=LightCoral><img src="thumbnails/Forest_image_0230.jpg" width=75 height=75><br><small>Highway</small></td>
<td bgcolor=LightCoral><img src="thumbnails/Forest_image_0347.jpg" width=75 height=75><br><small>OpenCountry</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Forest_image_0179.jpg" width=75 height=75><br><small>Mountain</small></td>
<td bgcolor=#FFBB55><img src="thumbnails/Forest_image_0036.jpg" width=75 height=75><br><small>Suburb</small></td>
</tr>
<tr>
<th>Category name</th>
<th>Accuracy</th>
<th colspan=2>Sample training images</th>
<th colspan=2>Sample true positives</th>
<th colspan=2>False positives with true label</th>
<th colspan=2>False negatives with wrong predicted label</th>
</tr>
</table>
</center>


</div>
</body>
</html>


## Extra credit?
No Extra credit

## Anything else?
Nothing else