  <style>
    body {
  font-family: Arial, sans-serif;
  margin: 0;
  padding: 0;
}

header {
  background-color: lightgray;
  display: flex;
  justify-content: space-between;
  align-items: center;
  padding: 20px;
}

header h1 {
  margin: 0;
}

nav ul {
  list-style: none;
  display: flex;
  margin: 0;
  padding: 0;
}

nav a {
  text-decoration: none;
  margin: 0 10px;
  color: black;
}

main {
  padding: 20px;
}

section {
  margin-bottom: 20px;
}

footer {
  background-color: lightgray;
  text-align: center;
  padding: 10px;
}

    </style>
  <head>
    <meta charset="UTF-8">
    <title>Welcome to My Website</title>
    <link rel="stylesheet" type="text/css" href="style.css">
  </head>
  <body>
    <header>
      <h1>Welcome to My Website</h1>
      <nav>
        <ul>
          <li><a href="#about">About</a></li>
          <li><a href="#services">Services</a></li>
          <li><a href="#contact">Contact</a></li>
        </ul>
      </nav>
    </header>
    <main>
      <section id="about">
        <h2>About Us</h2>
        <p>We are a team of professionals dedicated to providing top-notch services to our clients. Our goal is to help businesses succeed in the online world by offering a range of web development and digital marketing solutions. Contact us to learn more about how we can help you!</p>
      </section>
      <section id="services">
        <h2>Our Services</h2>
        <ul>
          <li>Web Development</li>
          <li>Digital Marketing</li>
          <li>SEO Optimization</li>
        </ul>
      </section>
      <section id="contact">
        <h2>Contact Us</h2>
        <form>
          <label for="name">Name:</label>
          <input type="text" id="name" name="name"><br><br>
          <label for="email">Email:</label>
          <input type="email" id="email" name="email"><br><br>
          <label for="message">Message:</label>
          <textarea id="message" name="message"></textarea><br><br>
          <button type="submit">Submit</button>
        </form>
      </section>
    </main>
    <footer>
      <p>Copyright © 2023 My Website</p>
    </footer>
  </body>
