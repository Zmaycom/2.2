<html>
    <head>
        <script src="jquery-3.5.1.js"></script>
        <script>
         $(document).ready(function(){

             $("#btn1").click(function(){
                $("#txt").animate({width: '400px',});
                $("#b1").prop( "disabled", true );
                $("#b2").prop( "disabled", false );
            
             });
             $("#btn2").click(function(){
                $("#txt").animate({width: '50px'});
                $("#b2").prop( "disabled", true );
                $("#b1").prop( "disabled", false );
             });
            
             $("#btn3").click(function(){
                $("#txt").animate({height: '400px'});
                $("#b3").prop( "disabled", true );
                $("#b4").prop( "disabled", false );
             });
             
             $("#btn4").click(function(){
                $("#txt").animate({height: '50px'});
                $("#b4").prop( "disabled", true );
                $("#b3").prop( "disabled", false );
             });
         });
        </script>
    </head> 
    <body>
        <input type="button" id="btn1" value="Широкий"/><br>
        <input type="button" id="btn2" value="Узкий" disabled/><br>
        <input type="button" id="btn3" value="Высокий"/><br>
        <input type="button" id="btn4" value="Низкий" disabled/><br>
        <div id="txt" style="background: green;height: 50px;width: 50px;"></div>
    </body>
</html> 
