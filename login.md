<style>
  body {
  font-family: Arial, sans-serif;
  background-color: #f0f0f0;
  display: flex;
  flex-direction: column;
  align-items: center;
  height: 100vh;
  margin: 0;
  padding: 0;
}

header {
  background-color: #333;
  color: #fff;
  padding: 20px;
  width: 100%;
}

header h1 {
  margin: 0;
}

main {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
  padding: 50px;
}

form {
  background-color: #fff;
  border: 1px solid #333;
  padding: 40px;
  width: 500px;
  display: flex;
  flex-direction: column;
  align-items: center;
}

form h2 {
  margin: 0;
  margin-bottom: 20px;
}

input[type="text"],
input[type="password"] {
  width: 100%;
  padding: 10px;
  margin-bottom: 20px;
  font-size: 16px;
  border: 1px solid #333;
}

button[type="submit"] {
  background-color: #333;
  color: #fff;
  padding: 10px 20px;
  border: none;
  cursor: pointer;
  font-size: 16px;
}

button[type="submit"]:hover {
  background-color: #fff;
  color: #333;
}

</style>
<head>
    <meta charset="UTF-8">
    <title>Login/Sign Up</title>
  </head>
  <body>
    <main>
      <form id="form">
        <h2>Login/Sign Up</h2>
        <input type="text" placeholder="Username" id="username">
        <input type="password" placeholder="Password" id="password">
        <button type="submit">Submit</button>
      </form>
    </main>
</body>

<script>
  const form = document.querySelector('#form');
  const username = document.querySelector('#username');
  const password = document.querySelector('#password');

  form.addEventListener('submit', e => {
    e.preventDefault();

    const data = {
      username: username.value,
      password: password.value
    };

    console.log(data);

    // Add your own code here to submit the data to a server, for example using fetch or XMLHttp

</script>
