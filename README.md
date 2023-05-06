## hi, I am PedroZiTan

I'am years 17 old

 <div>
   <a href="https://github.com/PedroZiTan">
<img height="180em" src="https://github-readme-stats.vercel.app/api?username=PedroZiTan&show_icons=true&theme=cobalt&include_all_commits=true&count_private=true"/>
   <img height="180em" src="https://github-readme-stats.vercel.app/api/top-langs/?username=PedroZiTan&layout=compact&langs_count=6&theme=tokyonight"/>

</div>
<div style="display: inline_block"><br>
  <img align="center" alt="Js" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-plain.svg">
  <img align="center" alt="HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
</div>
 
 <br>
 
  ### PedroZiTan
 
<div> 
  <a href="https://www.youtube.com/@PedroZiTan" target="_blank"><img src="https://img.shields.io/badge/YouTube-FF0000?style=for-the-badge&logo=youtube&logoColor=white" target="_blank"></a>
  <a href="https://www.instagram.com/pedrozitan/" target="_blank"><img src="https://img.shields.io/badge/-Instagram-%23E4405F?style=for-the-badge&logo=instagram&logoColor=white" target="_blank"></a>
  <a href="https://www.linkedin.com/in/pedro-zi-kang-tan-621110269/" target="_blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a> 
 </div>
  
 <div style="position: fixed; z-index: -1; top: 0; left: 0; width: 100%; height: 100%;">
  <canvas id="canvas"></canvas>
</div>

<div style="position: absolute; top: 50%; left: 50%; transform: translate(-50%, -50%);">
  <h1 style="font-size: 5rem; color: white; text-shadow: 0 0 10px black;">Seu Nome GitHub</h1>
</div>

<style>
  body {
    margin: 0;
    padding: 0;
  }
</style>

<script>
  const canvas = document.getElementById('canvas');
  const ctx = canvas.getContext('2d');

  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;

  const colors = [
    'rgb(255, 0, 0)',
    'rgb(0, 255, 0)',
    'rgb(0, 0, 255)',
    'rgb(255, 255, 0)',
    'rgb(0, 255, 255)',
    'rgb(255, 0, 255)'
  ];

  let colorIndex = 0;
  let colorDirection = 1;

  function animate() {
    ctx.fillStyle = colors[colorIndex];
    ctx.fillRect(0, 0, canvas.width, canvas.height);

    if (colorIndex === colors.length - 1 || colorIndex === 0) {
      colorDirection *= -1;
    }

    colorIndex += colorDirection;

    requestAnimationFrame(animate);
  }

  animate();
</script>

