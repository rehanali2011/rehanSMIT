<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Periodic Table</title>
  <!-- External CSS File -->
  <link rel="stylesheet" href="style.css" />
</head>
<body>
  <h1>Periodic Table</h1>

  <div class="table">
    <!-- Period 1 -->
    <div class="element nonmetal"><span class="num">1</span><span class="symbol">H</span><span class="name">Hydrogen</span></div>
    <div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div>
    <div class="element noble"><span class="num">2</span><span class="symbol">He</span><span class="name">Helium</span></div>

    <!-- Period 2 -->
    <div class="element alkali"><span class="num">3</span><span class="symbol">Li</span><span class="name">Lithium</span></div>
    <div class="element alkaline"><span class="num">4</span><span class="symbol">Be</span><span class="name">Beryllium</span></div>
    <div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div><div class="empty"></div>
    <div class="element metalloid"><span class="num">5</span><span class="symbol">B</span><span class="name">Boron</span></div>
    <div class="element nonmetal"><span class="num">6</span><span class="symbol">C</span><span class="name">Carbon</span></div>
    <div class="element nonmetal"><span class="num">7</span><span class="symbol">N</span><span class="name">Nitrogen</span></div>
    <div class="element nonmetal"><span class="num">8</span><span class="symbol">O</span><span class="name">Oxygen</span></div>
    <div class="element halogen"><span class="num">9</span><span class="symbol">F</span><span class="name">Fluorine</span></div>
    <div class="element noble"><span class="num">10</span><span class="symbol">Ne</span><span class="name">Neon</span></div>
  </div>
</body>
</html>




CSS
body{
  font-family: Arial, sans-serif;
  background:#f4f6f8;
  padding:20px;
}

h1{
  text-align:center;
  margin-bottom:20px;
}

.table{
  display:grid;
  grid-template-columns: repeat(18, 1fr);
  gap:6px;
  max-width:1200px;
  margin:auto;
}

.element{
  background:#fff;
  border:1px solid #cfd8dc;
  border-radius:6px;
  padding:6px 4px;
  text-align:center;
  min-height:70px;
  font-size:12px;
}

.num{ font-size:10px; color:#555; }
.symbol{ font-size:20px; font-weight:bold; display:block; }
.name{ font-size:10px; }

.empty{ visibility:hidden; }

/* Colors */
.alkali{ background:#ffffff; }
.alkaline{ background:#fff3e0; }
.transition{ background:#e3f2fd; }
.metalloid{ background:#e8f5e9; }
.nonmetal{ background:#f3e5f5; }
.halogen{ background:#e0f7fa; }
.noble{ background:#ede7f6; }
