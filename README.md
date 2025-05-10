<!-- index.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Accessible Website</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <a href="#main" class="skip-link">Skip to main content</a>
  <header>
    <nav>
      <ul class="nav">
        <li><a href="index.html">Home</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>
  <main id="main">
    <h1>Welcome</h1>
    <p>This is the homepage of an accessible site.</p>
    <img src="img1.jpg" alt="Image one">
  </main>
</body>
</html>

<!-- gallery.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Gallery</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <a href="#main" class="skip-link">Skip to main content</a>
  <header>
    <nav>
      <ul class="nav">
        <li><a href="index.html">Home</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>
  <main id="main" class="gallery">
    <h1>Image Gallery</h1>
    <div class="grid">
      <img src="img1.jpg" alt="Image 1">
      <img src="img2.jpg" alt="Image 2">
      <img src="img3.jpg" alt="Image 3">
      <img src="img4.jpg" alt="Image 4">
      <img src="img5.jpg" alt="Image 5">
    </div>
  </main>
</body>
</html>

<!-- contact.html -->
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>Contact</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <a href="#main" class="skip-link">Skip to main content</a>
  <header>
    <nav>
      <ul class="nav">
        <li><a href="index.html">Home</a></li>
        <li><a href="gallery.html">Gallery</a></li>
        <li><a href="contact.html">Contact</a></li>
      </ul>
    </nav>
  </header>
  <main id="main">
    <h1>Contact Us</h1>
    <p>Email: contact@example.com</p>
  </main>
</body>
</html>

/* style.css */
.skip-link {
  position: absolute;
  top: -40px;
  left: 0;
  background: #000;
  color: #fff;
  padding: 8px;
  z-index: 100;
}
.skip-link:focus {
  top: 0;
}

.nav {
  display: flex;
  gap: 20px;
  list-style: none;
  background-color: #eee;
  padding: 10px;
}

.nav a {
  text-decoration: none;
  color: #333;
}

.nav a:hover {
  color: #007BFF;
  text-decoration: underline;
}

img {
  border: 2px solid #ccc;
  padding: 10px;
  border-radius: 8px;
  margin: 10px;
}

.grid {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  gap: 20px;
  padding: 20px;
}

.grid img:nth-child(odd) {
  border-radius: 20px;
}
