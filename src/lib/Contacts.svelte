
<main>
  <section class="my-20 max-w-4xl mx-auto p-6" id="contact">
    <h2 class="text-4xl font-bold text-center">Contact Us</h2>

    <form action="" class="flex flex-col mt-8 space-y-6">
      <label for="subject" class="text-2xl font-medium">Subject:</label>
      <input type="text" name="subject" id="subject" placeholder="Your Subject"
        class="bg-white rounded-2xl p-4 text-black text-xl font-medium" required
      >

      <label for="message" class="text-2xl font-medium">Message</label>
      <textarea name="message" id="message" required cols="30" rows="15" 
         placeholder="Your Message"
        class="bg-white rounded-2xl p-4 text-black text-xl font-medium"
      ></textarea>

      <button class="self-start bg-teal-600 text-xl p-3 rounded-xl cursor-pointer font-medium">Submit</button>
    </form>
  </section>
</main>