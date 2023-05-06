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

