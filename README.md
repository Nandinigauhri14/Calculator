<!DOCTYPE html>
<html>
<head lang="en">
	<title>calculator</title>
<meta charset="utf-8">
       <script> 
         function dis(val) 
         { 
             document.getElementById("result").value+=val 
         } 
           
         function solve() 
         { 
             let x = document.getElementById("result").value 
             let y = eval(x) 
             document.getElementById("result").value = y 
         } 
         
         function clr() 
         { 
             document.getElementById("result").value = "" 
         } 
      </script> 
      <style> 
      	body
      	{
      		 background-image: url(https://i.pinimg.com/564x/0b/62/bf/0b62bf5658559ecb44b93c2dec1aadac.jpg);
      		
      	}
         .title{ 
         margin-bottom: 10px; 
         text-align:center; 
         width: 210px; 
         color:black; 
         background-color: lightblue;
         border: solid black 2px; 
         } 
  
         input[type="button"] 
         { 
         background-color:pink; 
         color: black; 
         text-align:center;
         border: solid black 2px; 
         width:100% 

       
         } 
  
         input[type="text"] 
         { 
         background-color:orange; 
         text-align:right;
         border: solid black 2px; 
         width:95% 
      
         
         } 
      </style> 
   </head> 
      <body> 
      <center>
      <div class = title>CALCULATOR <br>by <br>NANDINI GAUHRI</div> 
      <table border="2" > 
         <tr> 
            <td colspan="3"><input type="text" id="result"/></td> 
            
            <td><input type="button" value="c" onclick="clr()"/> </td> 
         </tr> 
         <tr> 
            
            <td><input type="button" value="1" onclick="dis('1')"/> </td> 
            <td><input type="button" value="2" onclick="dis('2')"/> </td> 
            <td><input type="button" value="3" onclick="dis('3')"/> </td> 
            <td><input type="button" value="/" onclick="dis('/')"/> </td> 
         </tr> 
         <tr> 
            <td><input type="button" value="4" onclick="dis('4')"/> </td> 
            <td><input type="button" value="5" onclick="dis('5')"/> </td> 
            <td><input type="button" value="6" onclick="dis('6')"/> </td> 
            <td><input type="button" value="-" onclick="dis('-')"/> </td> 
         </tr> 
         <tr> 
            <td><input type="button" value="7" onclick="dis('7')"/> </td> 
            <td><input type="button" value="8" onclick="dis('8')"/> </td> 
            <td><input type="button" value="9" onclick="dis('9')"/> </td> 
            <td><input type="button" value="+" onclick="dis('+')"/> </td> 
         </tr> 
         <tr> 
            <td><input type="button" value="." onclick="dis('.')"/> </td> 
            <td><input type="button" value="0" onclick="dis('0')"/> </td> 
            <td><input type="button" value="=" onclick="solve()" /> </td> 
            <td><input type="button" value="*" onclick="dis('*')"/> </td> 
         </tr> 
      </table> 
   </center>
   </body> 
</html>    
