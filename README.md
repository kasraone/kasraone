### Hi there 👋

<!--
**kasraone/kasraone** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->



<p align="center"> 
  Visitor count<br>
  <img src="https://profile-counter.glitch.me/kasraone/count.svg" />
</p>


<div align="center">
    <a href="https://github.com/kawarimidoll/typograssy">
        <img alt="typograssy" src="https://typograssy.deno.dev/api?text=KASRAONE&l0=none&l1=82d9d0&l2=027353&l3=038c4c&l4=01402e&bg=none&frame=none&speed=100&comment=">
    </a>
</div>


<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Puzzle Animation</title>
<style>
    .puzzle {
        display: inline-block;
        width: 100px;
        height: 100px;
        background-image: url('https://via.placeholder.com/100');
        background-size: 300px 300px;
        transition: all 1s ease-in-out;
    }

    .puzzle:hover {
        transform: translate(100px, 100px);
    }
</style>
</head>
<body>
<div class="puzzle"></div>
<script>
    function splitAndMerge() {
        const puzzle = document.querySelector('.puzzle');
        const size = 100;
        let isSeparated = false;

        function animate() {
            if (isSeparated) {
                puzzle.style.backgroundSize = '300px 300px';
                puzzle.style.transitionDuration = '1s';
                puzzle.style.transform = 'translate(100px, 100px)';
            } else {
                puzzle.style.backgroundSize = '100px 100px';
                puzzle.style.transitionDuration = '1s';
                puzzle.style.transform = 'translate(0, 0)';
            }

            isSeparated = !isSeparated;
        }

        setInterval(animate, 20000); // 20 seconds
    }

    window.onload = function () {
        splitAndMerge();
    };
</script>
</body>
</html>
