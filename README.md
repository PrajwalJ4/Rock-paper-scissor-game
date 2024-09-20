# Rock-paper-scissor-game
first game created
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="style.css" >
</head>
<body>
    <h1>Rock, Paper and Scissor</h1>
    
 <div>
<button id="rock" class="btn"><img class="image" src="https://wrpsa.com/wp-content/uploads/2021/08/rock.png" ></button>
<button id="paper" class="btn"><img class="image" src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRLaIPiR6QMLkwylcUJoHbLM9iYcyT50-hp6w&s"></button>
<button id="scissor" class="btn"><img class="image" src="https://wrpsa.com/wp-content/uploads/2021/08/scissors.png"></button>
</div>   


 <script src="script.js"  ></script> 
</body>
</html>

div{
    display: flex;
    height: 200px;
    width: 400px;
    justify-content: space-evenly;
    align-items: center;
}
.image{
    height: 100px;
    width: 100px;
    border-radius: 50%;
}
button{
    border: none;
}
body{
    
    justify-content: center;
    align-items: center;
}
let Cc= "";


let result="";
   let btn1=document.querySelector("#rock") ;
   btn1.addEventListener("click",function(){
    Cc=Math.random();
    if (Cc>=0 && Cc<1/3)
        Cc="rock";
    else if (Cc>=1/3 && Cc<2/3)
        Cc="paper";
    
     else
        Cc="scissor";
                                    if(Cc==="rock")
                                        alert(`you have chosed rock,computers choice is rock,Match tied`);
                                    
                                    else if(Cc==="paper")
                                        alert(`you have chosed rock,computers choice is paper,you lose`);
                                    else
                                         alert(`you have chosed rock,computers choice is scissor,you win`);

                                     
   });
   let btn2=document.querySelector("#paper") ;
   btn2.addEventListener("click",function(){
    Cc=Math.random();
    if (Cc>=0 && Cc<1/3)
        Cc="rock";
    else if (Cc>=1/3 && Cc<2/3)
        Cc="paper";
    
     else 
        Cc="scissor";
                                    if(Cc==="rock")
                                        alert(`you have chosed paper,computers choice is rock,you win`);
                                    
                                    else if(Cc==="paper")
                                        alert(`you have chosed paper,computers choice is paper,Match tied`);
                                    else
                                         alert(`you have chosed paper,computers choice is scissor,you lose`);

                                     
   });
   let btn3=document.querySelector("#scissor") ;
   btn3.addEventListener("click",function(){
    Cc=Math.random();
    if (Cc>=0 && Cc<1/3)
        Cc="rock";
    else if (Cc>=1/3 && Cc<2/3)
        Cc="paper";
    
     else
        Cc="scissor";
                                    if(Cc==="rock")
                                        alert(`you have chosed scissor,computers choice is rock,you lose`);
                                    
                                    else if(Cc==="paper")
                                        alert(`you have chosed scissor,computers choice is paper,you win`);
                                    else 
                                         alert(`you have chosed scissor,computers choice is scissor,Match tied`);

                                     
   });
