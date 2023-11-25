<html lang="en">
<head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <title>Todo app</title>
     <link rel="stylesheet" href="cssfile.css">
     <style>
          *{
     margin: 0;
     padding: 0;
     box-sizing: border-box;
     font-family: 'poppins',sans-serif;
}
.container{
   width: 100%;
   min-height: 100vh;
   /* background: linear-gradient(135deg, #153677, #4e085f); */
   /* background-color: #555;
   background-color: aliceblue; */
   padding: 10px;
}
.todo-app{
     width: 100%;
     max-width: 540px;
     background: #fff;
     margin: 100px auto 20px;
     padding: 40px 30px 70px;
     border-radius: 10px;
}
.row{
     display: flex;
     align-items: center;
     justify-content: space-between;
     background: #edeef0;
     border-radius: 30px;
     padding-left: 20px;
     margin-bottom: 25px;
}
input{
   flex: 1;
   border: none;
   outline: none;
   background: transparent;
   padding: 10px;
   font-weight: 14px;
}
button{
     border: none;
     outline: none;
     padding: 16px 50px;
     background: #ff5945;
     color: #fff;
     font-size: 16px;
     cursor: pointer;
     border-radius: 40px;
}
ul li{
     list-style: none;
     font-size: 17px;
     padding: 12px 8px 12px 50px;
     user-select: none;
     cursor: pointer;
     position: relative;
}
ul li::before{
     content: '';
     position: absolute;
     height: 28px;
     width: 28px;
     border-radius: 50%;
     background-image: url(Downloads/radio_button.jpg);
     background-size: cover;
     background-position: center;
     top: 12px;
     left: 0px;

}
ul li span{
     position: absolute;
     right: 0;
     top: 5px;
     width: 40px;
     height: 40px;
     font-size: 22px;
     color: #555;
     line-height: 40px;
     text-align: center;
     border-radius: 50%;
}
ul li span:hover{
     background: #edeef0;
}
     </style>

</head>
<body>   
  <div class="container">
      <div class="todo-app">
           <h1 style="margin-left: 140px;">Todo-App</h1>
           <div class="row">
               <input type="text" id="input-box" placeholder="Enter your text .......">
               <button onclick="AddTask()">Add</button>
           </div>
           <ul id="list-container">
               
           </ul>
      </div>
  </div>
  <script src="jsfile.js"></script>
  <script>
     const inputBox = document.getElementById("input-box");
const listContainer = document.getElementById("list-container");
function AddTask(){
     if(inputBox.value == ''){
          alert("you write must something!");
     }
     else{
          let li = document.createElement("li");
          li.innerHTML = inputBox.value;
          listContainer.appendChild(li);
          let span = document.createElement("span");
          span.innerHTML = "\u00d7";
          li.appendChild(span);
     }
     inputBox.value = "";
}

listContainer.addEventListener("click",function(e){
     if(e.target.tagName == "LI"){
          e.target.classList.toggle("checked");
     }
     else if(e.target.tagName == "SPAN"){
          e.target.parentElement.remove();
     }
},false
);
  </script>
</body>
</html>
