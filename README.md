<!DOCTYPE html>
   <title>Jackenaktion ET</title>
   <script
    src="https://code.jquery.com/jquery-3.6.3.js"
    integrity="sha256-nQLuAZGRRcILA+6dMBOvcRh5Pe310sBpanc6+QBmyVM="
    crossorigin="anonymous">
   </script>
   <script>
      function SubForm (){
         $.ajax({
             url:'https://api.apispreadsheets.com/data/faxlPLB09wddvLPd/',
             type: 'post',
             data:$("#myForm").serializeArray(),
             success: function(){
                alert("Form Data Submitted :)")
             },
             error: function(){
                alert("There was an error: (")
             }
          });
       }
   </script>
   <style>
     body {
      font-family: Calibri, calibri light; 
      color: white;
      background-color: #214761;
      text-align: center;
      .right-upper-corner {
      position: absolute;
      top: 0;
      right: 0;
      }
         }
   </style>
   </head>
   <body>
     <img src="./Jackenaktion_web_files/logo2.jpg" width="100" height="100 text-align: right">
     <br>
     <br>
     <br>
     <h1> <font color="#9dbcd4">Softshelljackenaktion der Energietechniker</font></h1>
     <br>
     Liebe Energietechniker und Energietechnikerinnen!
     <br>
     Bei Interesse an einer Softshelljacke bitten wir euch, 
     <br>
     eure E-Mail-Adresse anzugeben sowie eure gewünschte Größe auszuwählen.
     <br>
     <h3>Glück Auf!</h3>
     <br>
     <br>
     <form id="myForm">
        <input placeholder="E-Mail" type="email" name="E-Mail">
        <br>
        <label for="size">Größe/ Size</label>
          <select name="size" id="size">
            <option value="XS">XS</option>
            <option value="S">S</option>
            <option value="M">M</option>
            <option value="L">L</option>+
            <option value="XL">XL</option>
            <option value="2XL">2XL</option>
            <option value="3XL">3XL</option>
            <option value="4XL">4XL</option>
            <option value="5XL">5XL</option>
            <option value="6XL">6XL</option>
          </select>
     </form>
     <br>
     <br>
     <input type="submit" name="submit" onclick="SubForm(); return false;" >
    <br>
    <br>
    <br>
    <br>
    <img src="ET/softshelljacke2.png" width="200" height="200">
    <img src="ET/softshelljacke3.png" width="200" height="200">
    <img src="ET/softshelljacke.png" width="200" height="200">
    <br>
    <br>
    <br>
    <br>
    <br>
<footer>
<p> Studienvertretung Energietechnik/ Student Representatives Industrial Energy Technology </p>
<p>E-Mail: stv-ie@oeh.unileoben.ac.at</p>
</footer>
</body>
</html>
