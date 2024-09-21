<script lang="ts">
</script>

<div class="container">
  <div class="form-container">
    <form method="post">
      <label>
        Email
        <input type="email" name="email" />
      </label>
      <label>
        Password
        <input type="password" name="password" />
      </label>
    </form>
  </div>

  <p>Login With Google</p>
  <br />
  <br />
  <br />
  <p>Login With Github</p>
</div>

<style>
.container {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}

form {
  padding: 50px;
}

input::active {
  border: none;
  outline: none;
}
</style>
