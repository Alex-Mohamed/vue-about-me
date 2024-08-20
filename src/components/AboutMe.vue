<template>
    <ul id='list'>
        <li>Became interested in software development during my sophmore year of high school</li>
        <li>Acquired a microbiology internship at UMB during my senior year</li>
        <li>Joined the quantum and cybersecurity clubs in the past semester</li>
        <li>Learned C++, JavaScript, HTML, and CSS this summer</li>
        <li>Planning to take AWS certification exams soon</li>
    </ul>

    <div>
        <p>&emsp;</p>
        <button class="button" onclick="document.getElementById('demo').innerHTML = 'Genetic Engineering --> https://amohamedgeneticengineering.weebly.com/  <br> Computer Science --> https://amohamedcomputerscience.weebly.com/'" >Press for link to research websites!</button>
        <p>&emsp;</p>
        <p id="demo"></p>
        <p>&emsp;</p>
        <!-- This button does not work yet -->
        <button class="button" onclick="randomPic()">Click to generate a new picture!</button>
        <p>&emsp;</p>
    </div>

    <form>
        <fieldset>
            <h2 style="color:aqua">Webpage Improvement Survey</h2>
            <h3>How would you improve this webpage for future visitors?</h3>

            <input class="radio-input" type="radio" id="poll" name="poll" placeholder="Enter answer here" required>
            <label class="radio-label" for="box1"> Make the webpage more mobile-friendly</label><br>

            <input class="radio-input" type="radio" id="poll" name="poll" placeholder="Enter answer here" required>
            <label class="radio-label" for="box2"> Increase the amount of interactive elements</label><br>

            <input class="radio-input" type="radio" id="poll" name="poll" placeholder="Enter answer here" required>
            <label class="radio-label" for="box3"> Investigate causes of slow page load times</label><br>

            <input type="submit" value="Submit">
        </fieldset>
    </form>
</template>

<script>
    function randomPic() {
        if(Math.floor(Math.random() * 2) + 1 == 1) {
            document.getElementById('pic').src = "./assets/about_me.jpeg";
        } else {
            document.getElementById('pic').src = "./assets/linked_in.jpeg";
        }
    }
</script>

<style>
 ul {
    line-height: 2.5;
    font-size:large;
    color:royalblue;
 }

 #demo {
    font-size: medium;
    text-align: center;
 }

 .button {
    font-size: large;
    margin: auto;
    display: grid;
 }

 h2, h3 {
    text-align: center;
    color: aqua;
 }

 form {
    text-align: center;
    color: dodgerblue;
 }
</style>