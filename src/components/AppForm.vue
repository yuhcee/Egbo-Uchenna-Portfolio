<template>
  <div>
    <form
      name="contact"
      method="POST"
      data-netlify="true"
      data-netlify-honeypot="bot-field"
    >
      <h2>ziga ozi</h2>
      <!--add some things here to make it work with Netlify-->
      <p class="visually-hidden">
        <!--add something here to catch the bots!-->
        <input type="hidden" name="form-name" value="contact" />
      </p>
      <p>
        <label>
          Name
          <input type="text" name="name" />
        </label>
      </p>
      <p>
        <label>
          Email
          <input type="email" name="email" />
        </label>
      </p>
      <p>
        <label>
          Message
          <textarea name="message"></textarea>
        </label>
      </p>
      <p>
        <button type="submit">Send</button>
      </p>
    </form>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
h2 {
  text-transform: uppercase;
}

button {
  width: 100%;
}

label,
button {
  margin-top: 20px;
}
</style>
