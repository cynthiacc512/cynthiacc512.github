<template>
    <section class="container" id="contact-me">
      <h1>Contact Me</h1>
      <form method="POST" action="#" id="contact">
        <label class="form-label" for="fname">Firstname</label><br />
        <input type="text" id="fname" name="fname" class="form-control" placeholder="John" /><br />
        <label class="form-label" for="lname">Lastname</label><br />
        <input type="text" id="lname" name="lname" class="form-control" placeholder="Doe" /><br />
        <label class="form-label" for="region">Region</label><br />
        <select class="form-select" name="region" id="region">
          <option value="indonesia">Indonesia</option>
          <option value="australia">Australia</option>
          <option value="singapore">Singapore</option>
          <option value="malaysia">Malaysia</option>
        </select><br />
        <label class="form-label" for="message">Message</label><br />
        <textarea id="message" name="message" rows="4" cols="50" placeholder="Your Message"
          class="form-control"></textarea>
        <br />
        <div class="d-grid gap-2">
          <button class="btn btn-info" type="button" onclick="sendFormData()">Submit</button>
        </div>
      </form>
    </section>
</template>
<script>
export default {
    name: 'ContactMe'
}
</script>