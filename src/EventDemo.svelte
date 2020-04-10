<script>
  let m = { x: 0, y: 0 };

  function handleMouseEvent(event) {
    m.x = event.clientX;
    m.y = event.clientY;
  }
</script>

<style>
  div {
    height: 200px;
    width: 200px;
    color: purple;
    background-color: coral;
  }
</style>

<div on:mousemove={handleMouseEvent}>
  This is the mounse position x: {m.x} and y: {m.y}
</div>
