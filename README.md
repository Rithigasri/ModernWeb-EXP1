# EXPERIMENT 01: TO CREATE A WEB PORTFOLIO/CV USING HTML & CSS
## AIM:
To create a web portfolio/cv using html and css.
## ALGORITHM:
1. Create basic html page.
2. Use div components to separate each section of the webpage.
3. Add css styling to the required components.
4. Link the css file inside the head tag of html file.
5. Run the html page and dsiplay the output.
## PROGRAM:
### cv.html
```
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <link rel="stylesheet" href="cv.css"/>
    <script defer src="cv.js"></script>

</head>
<body background="https://i.pinimg.com/236x/ac/dc/1b/acdc1b5563a3d1e172eb7d8b6e90bd58.jpg" style="background-size: cover;">
   
    <div class="container">
        <div class="header" >
            <div class="top" id="up">
                <div><b>ABOUT</b></div>
                <div><b>SKILLS</b></div>
                <div><b>PORTFOLIO</b></div>
                <div><b>EXPERIENCE</b></div>
                <div><b>CONTACT</b></div>
            </div>
            <center>
                
                <img src="photo.jpeg" height="300px" width="250px" style="border-radius: 20px;" id="img">
                <h1 style="color:white;font-family: sans-serif;">Rithiga Sri.B</h1>
                <h2 style="color:white;font-family:monospace">I'm a data scientist, I turn numbers into knowledge</h2>
                
            </center>
        </div>
        <div class="box">
            <div class="info">
                Career Objective
            </div>
            <div class="details">
                <p>My career objective is to become an expert in the field of Artificial Intelligence and 
                    Data Science and leverage my knowledge and skills to solve complex problems in diverse industries.
                     I aspire to work with leading organizations and contribute towards developing innovative solutions that 
                     transform businesses and improve human lives. </p>
            </div>
        </div>
        <div>
            <div class="heading" id="head">
                Basic Info
            </div>
            <!-- <div class="details">
                <p><b>Age:</b>20 yrs<br/><b>Email-Id:</b>rithigasri383@gmail.com<br/>
                <b>Phone Number:</b>7305328312<br/><b>Address:</b>No.18/A,Indira Nagar 5th street,Vinayagapuram,Chennai-99
                <br/><b>Languages Known:</b>Tamil,English</p>

            </div> -->
            <div class="elements">
                <div style="margin-left:200px"></div>
                <div class="b1">Age</div>
                <div class="b2"><p>20 years</p></div>
                <div class="b1">Email-Id</div>
                <div class="b2"><p>rithigasri383@gmail.com</p></div>
                
            </div>
            <div class="elements">
                <div style="margin-left:200px"></div>
                <div class="b1">Phone Number</div>
                <div class="b2"><p>7305328312</p></div>
                <div class="b1">Address</div>
                <div class="b2"><p>Enclave Garden,Chennai</p></div>
                
            </div>
            <div class="elements">
                <div style="margin-left:200px"></div>
                <div class="b1">Languages</div>
                <div class="b2"><p>Tamil,English</p></div>
                <div class="b1">Date Of Birth</div>
                <div class="b2"><p>03.08.2003</p></div>
                
            </div>
        </div>
        <div class="skill">
            <center>Skills Acquired</center><br/>
            
                <li>Machine Learning</li>
                <li >Deep Learning</li>
                <li>Natural Language Processing</li>
                <li >Data Analysis and Visualization</li>
                <li>Programming</li>
                <li>Communication and Collaboration</li>
        </div>
        <div class="box">
            <div class="info">
                Work Experience
            </div>
            <div class="details">
                <p>Monolith Research and Development Center<i>(Jan-Feb 2023)</i>
                    <br/>Teachnook <i>(Feb-Mar 2023)</i></p>
            </div>
        </div>

        <div class="box">
            <div class="info">
                Education
            </div>
            <div class="details">
                
                <p>SSLC - 96.4% Velammal Vidhyshram <i>(2018-2019)</i><br/>
                SSLC - 90.0% Velammal Vidhyshram <i>(2020-2021)</i><br/>
                B.Tech Artificial Intelligence and Data Science <i>(2021-2025)</i></p>
            </div>
        </div>

        <div class="footer">
            <center><p style="font-family: monospace;padding-top: 5px;font-size:20px">Connect Me</p></center>
                <div style="display:flex;justify-content: space-evenly;margin-left:30px;margin-right: 30px;">
                    <div class="button">Github</div>
                    <div class="button">LinkedIn</div>
                    <div class="button">Gmail</div>
                </div>
        </div>
    </div>
 </body>   
</html>
```
### cv.css
```
body
{
    margin-left:15px;
    margin-right: 15px;
    
    
}
/* .container
{
    width: 1080px;
    margin-left: auto;
    margin-right: auto;
    background-image: url("https://i.pinimg.com/236x/ac/dc/1b/acdc1b5563a3d1e172eb7d8b6e90bd58.jpg"); 
    background-size: cover;
    overflow: hidden;  
    box-shadow: 15px 15px 8px gray;
} */
.top
{
    display: flex;
    color: black;
    font-family: monospace;
    justify-content: space-between;
    padding: 15px;
    margin-bottom: 25px;
    background-color: lightgreen;
    
}

.box
{
    height:250px;
    display: flex;
    transition: transform 0.3s ease-in-out;
    
}
.info
{   margin-top:50px;
    margin-left:200px;
    width:300px;
    height:200px;
    background-color: lightgreen;
    overflow: hidden;
    color:Black;
    font-family: monospace;
    font-size: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 10px 0 0 10px;
    
}
.box:hover {
    transform: scale(1.2);

}
.details
{   height:200px;
    width:700px;
    background-color: white;
    margin-top:50px;
    margin-right: 200px;
    color:Black;
    font-family:'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    font-size: 20px;
    padding-left: 10px;
    padding-right: 10px;
    display: flex;
    align-items: center;
    text-align: justify;
    line-height: 35px;
    border-radius: 0 10px 10px 0;
}
.skill
{
    /* border:3px solid greenyellow; */
    /* box-shadow: 0px 5px 10px 0px white; */
    font-family:monospace;
    border-radius: 30px;
    padding: 15px;
    color:white;
    font-size: 20px;
    margin:100px 50px 20px 50px;
    width: 1300px;
    height:200px;
    box-shadow: blue 0px 0px 0px 2px inset,black 10px -10px 0px -3px, green 10px -10px, black 20px -20px 0px -3px, yellow 20px -20px, black 30px -30px 0px -3px, orange 30px -30px,black 40px -40px 0px -3px, red 40px -40px;
    cursor: pointer;
}

.skill:hover
{
    animation: shadow-wave 1s ease infinite;
}

@keyframes shadow-wave {
    0%{
        box-shadow: blue 0px 0px 0px 2px inset,black 10px -10px 0px -3px, green 10px -10px, black 20px -20px 0px -3px, yellow 20px -20px, black 30px -30px 0px -3px, orange 30px -30px,black 40px -40px 0px -3px, red 40px -40px;
    }
    20% {
        
        box-shadow: red 0px 0px 0px 2px inset,black 10px -10px 0px -3px, blue 10px -10px, black 20px -20px 0px -3px, green 20px -20px, black 30px -30px 0px -3px, yellow 30px -30px,black 40px -40px 0px -3px, orange 40px -40px;
 
      }
    40% {
        
        box-shadow: orange 0px 0px 0px 2px inset,black 10px -10px 0px -3px, red 10px -10px, black 20px -20px 0px -3px, blue 20px -20px, black 30px -30px 0px -3px, green 30px -30px,black 40px -40px 0px -3px,yellow 40px -40px;
    }
    60% {
      
        box-shadow: yellow 0px 0px 0px 2px inset,black 10px -10px 0px -3px, orange 10px -10px, black 20px -20px 0px -3px, red 20px -20px, black 30px -30px 0px -3px, blue 30px -30px,black 40px -40px 0px -3px, green 40px -40px;
    }
    80% {

        box-shadow: green 0px 0px 0px 2px inset,black 10px -10px 0px -3px, yellow 10px -10px, black 20px -20px 0px -3px, orange 20px -20px, black 30px -30px 0px -3px, red 30px -30px,black 40px -40px 0px -3px, blue 40px -40px;
    }
    100% {
      
        box-shadow: blue 0px 0px 0px 2px inset,black 10px -10px 0px -3px, green 10px -10px, black 20px -20px 0px -3px, yellow 20px -20px, black 30px -30px 0px -3px, orange 30px -30px,black 40px -40px 0px -3px, red 40px -40px;
    }
}
.footer
{
    background-color:lightgreen;
    height: 100px;
    margin-top:100px;
    
}
.button
{
    background-color:black;
    color:white;
    font-family: monospace;
    padding: 15px;
    border-radius: 20px;
}

.heading
{
    margin-top:50px;
    margin-left:200px;
    width:1000px;
    padding-top: 10px;
    height:50px;
    background-color: lightgreen;
    color:Black;
    font-family: monospace;
    font-size: 30px;
    text-align: center;
    align-items: center;
    justify-content: center;
    border-radius: 10px 10px 10px 10px;
    border: 3px solid black;
    
}

.b1
{
    margin-top:50px;
    width:150px;
    height:50px;
    background-color: lightgreen;
    overflow: hidden;
    color:Black;
    font-family: monospace;
    font-size: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    border-radius: 10px 0 0 10px;
}
.elements
{
    
    display: flex;
    transition: transform 0.3s ease-in-out;
    
}
.b2
{
    height:50px;
    width:250px;
    background-color: white;
    margin-top:50px;
    margin-right: 150px;
    color:Black;
    font-family:'Trebuchet MS', 'Lucida Sans Unicode', 'Lucida Grande', 'Lucida Sans', Arial, sans-serif;
    font-size: 20px;
    padding-left: 10px;
    padding-right: 10px;
    display: flex;
    align-items: center;
    text-align: justify;
    border-radius: 0 10px 10px 0;
}
.elements:hover {
    transform: scale(1.2);

}
```
## OUTPUT:
![image](https://github.com/Rithigasri/ModernWeb-EXP1/assets/93427256/2d4ab8ac-f39c-41a5-bef2-12610041e880)
![image](https://github.com/Rithigasri/ModernWeb-EXP1/assets/93427256/64c1aa55-73ac-4cbd-b758-f7d3c862f13a)
![image](https://github.com/Rithigasri/ModernWeb-EXP1/assets/93427256/816a9794-be74-4ab5-b4fd-9b5e6acbf30f)
![image](https://github.com/Rithigasri/ModernWeb-EXP1/assets/93427256/41fae4ee-0b39-43d7-8da3-a559cbf9bd65)

## RESULY:
Thus,a portfolio is created using html and css.


