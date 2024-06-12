HTML FILE
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" />
    <title>Four box</title>
    <!-- icon link tag -->
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.5.2/css/all.min.css" integrity="sha512-SnH5WK+bZxgPHs44uWIX+LLJAJ9/2PkPKZ5QiAj6Ta86w+fsb2TkcmfRyVX3pBnMFcV7oQPJkl9QevSCWr3W6A==" crossorigin="anonymous" referrerpolicy="no-referrer" />
    <link rel="stylesheet" href="four-box.css" />
    <link rel="stylesheet" href="four-box.css" media="screen and (min-width:480px)">
  </head>
  <body>
    <section class="entire-body">
      <section class="box-container1">
      <div class="div1">
        <p class="first-para head">Reliable, efficient delivery</p>
        <h1 class="second-para head">Powered by Technology</h1>
        <p class="third-para head">
          Our Artificial intelligence powered tools use millions of project
          datapoints to ensure that your project is successful
        </p>
      </div>
      <div class="div2">
        <div class="box-1">
          <h4>Team Builder</h4>
          <p>
            scans our talent network to create the optimal team for your project
          </p>
          <i class="fa-solid fa-house-chimney"></i>
        </div> 
        <div class="box-3">
          <h4>Karma</h4>
          <p>
            Regularly evaluates our talent to ensure quality
          </p>
          <i class="fa-solid fa-lightbulb"></i>
        </div>
        <div class="box-2">
         <h4>Calculator</h4>
          <p>
            
            Monitor activity to identify projects roadblocks
          </p>
          <i class="fa-solid fa-tv"></i>  
        </div>
        <div class="box-4">
          <h4>Supervisor</h4>
          <p>
            Uses data from past projects to provide better delivery estimates
          </p>
          <i class="fa-solid fa-magnifying-glass"></i>
        </div>
      </div>
       </section>
      </section>
  </body>
</html>



CSS FILE

*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}
body{
    height: 100vh;
}
.div1{
    display: flex;
    justify-content: center; 
    align-items: center;  
    flex-direction: column; 
}

.div2{
    display: grid;
    grid-template-areas:
    'box-1'
    'box-2 box-3'
    'box-4'
    ;
    /* justify-content: center; */
    /* align-items: center;  */
    /* flex-direction: column; */
}
.first-para{
    font-size: 30px;
    margin-top: 40px;
}
.second-para{
    font-weight: bold;
    font-size: 40px;
    margin: 5px;
}
.third-para{
    font-size: 20px;
    margin: 5px;
}
.box-container1{
margin: auto;
height: 600px;
width: 80%;
position: relative;
}
.box-1{
    margin-top: 70px; 
    position: absolute;
    left: 36%; 
    width: 300px;
    height: 200px;
    grid-area: box-1;
    border-top: solid rgba(243, 11, 11, 0.822);
    border-radius: 5px;
    box-shadow: 5px 5px 10px rgba(0,0,0,0.15);
}
.box-4{
    position: absolute;  
    bottom: 0; 
    margin-left: 130px; 
    width: 300px;
    height: 200px; 
    grid-area: box-2 ;
    border-top: solid rgb(3, 206, 206) ;
    border-radius: 5px;
    box-shadow: 5px 5px 10px rgba(0,0,0,0.15);
}
.box-2{
    position: absolute;
    right: 0;
    bottom: 0;
    margin-right: 190px; 
    grid-area: box-3;
    width: 300px;
    height: 200px;
    border-top: solid rgb(59, 59, 216);
    border-radius: 5px;
    box-shadow: 5px 5px 10px rgba(0,0,0,0.15);
}
.box-3{
    position: absolute;
    right: 0;
    left: 36%;
    bottom: -100px; 
    grid-area: box-4;
    width: 300px;
    height: 200px;
    border-top: solid rgba(221, 221, 4, 0.877);
    border-radius: 5px;
    box-shadow: 5px 5px 10px rgba(0,0,0,0.15);
}
.fa-solid{
 font-size: 30px;
 position: absolute;
 right: 0;
 bottom: 0;
 padding: 20px;
 
}
.fa-house-chimney{
    color: rgba(243, 11, 11, 0.822) ;
}
.fa-lightbulb{
    color: yellow ;
}
.fa-tv{
    color: rgb(59, 59, 216) ;
}
.fa-magnifying-glass{
    color: rgb(3, 206, 206) ;
}
