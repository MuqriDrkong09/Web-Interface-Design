<template>
  <form>
    <div>
      <h2>Search Invoice</h2><br>

      <input type="radio" required>
      <label>General Equality</label><br>

      <input type="radio" required>
      <label>Exact Match</label><br><br>

      <div class="form-row">
        <div class="form-group">
          <label for="first-name">Invoice Number</label>
          <input id="first-name" type="text">
        </div>
        <div class="form-group">
          <label for="last-name">Invoice Date</label>
          <input id="last-name" type="date">
        </div>
        <div class="form-group">
          <label for="first-name">Invoice Type</label>
          <input id="first-name" type="text">
        </div>
        <div class="form-group">
          <label for="last-name">Bank Reference Number</label>
          <input id="last-name" type="text">
        </div>
      </div>
      <div class="form-row">
        <div class="form-group">
          <label for="location">Invoice Amount</label>
          <input id="location" type="text">
        </div>
        <div class="form-group">
          <label for="some-input">Invoice Recorded Date</label>
          <input id="some-input" type="date">
        </div>
        <div class="form-group">
          <label for="some-input">BRN</label>
          <input id="some-input" type="text">
        </div><br>
      </div>
      <div class="button">
        <button class="submit" type="submit">Reset</button>
        <button class="reset" type="reset">Search</button>
      </div>
    </div>
  </form>
</template>

<script>
export default {
  data() {
    return {

    }
  }
}
</script>

<style scoped>
form {
  max-width: 100%;
  /*margin: 30px auto;*/
  background: #fff;
  text-align: left;
  padding: 20px;
  border-radius: 10px;
}

label {
  color: black;
  display: inline-block;
  margin-bottom: 5px;
}

.form-row {
  display: flex;
}

.form-group {
  padding: 5px;
  width: 50%;
  margin: 8px;
}

.form-group input {
  width: 100%;
}

button {
  background: blue;
  border: 0;
  padding: 10px 20px;
  color: white;
  border-radius: 8px;
  margin: 8px;
  width: 150px;
}

.submit {
  text-align: center;
}

.error {
  color: #ff0000;
  margin-top: 10px;
  font-size: 0.8em;
  font-weight: bold;
}

</style>