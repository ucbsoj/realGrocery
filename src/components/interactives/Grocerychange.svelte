
<script>
  // Array of images
  let images = [
    '$assets/images/meat1.png?text=Image+1',
    '$assets/images/meat1.png?text=Image+2',
    '$assets/images/meat1.png?text=Image+3',
    '$assets/images/meat1.png?text=Image+4'
  ];

  let currentImageIndex = 0;

  // Function to change image when the button is clicked
  function changeImage() {
    currentImageIndex = (currentImageIndex + 1) % images.length;
  }
</script>

<style>
  .container {
    text-align: center;
    margin-top: 50px;
  }

  img {
    width: 300px;
    height: auto;
  }

  button {
    margin-top: 20px;
  }
</style>

<div class="container">
  <!-- Display the current image -->
  <div>
    <img src={images[currentImageIndex]} alt="Image" />
  </div>

  <!-- Button to change the image -->
  <button on:click={changeImage}>Change Image</button>
</div>