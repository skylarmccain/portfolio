<script>
    /** @type {import('./$types').PageData} */
    export let data;
</script>
<div class="flex items-center min-h-screen">
    <div class="container mx-auto">
      <div class="max-w-md mx-auto my-10">
        <div class="text-center">
          <h1
            class="my-3 text-3xl font-semibold"
          >
            Send Me a Message
          </h1>
          
        </div>
        <div class="m-4">
          <form action="https://api.web3forms.com/submit" method="POST" id="form" autocomplete="off">
            <input type="hidden" name="apikey" value="b76e4179-4703-4e15-8b52-b60bacebc08" />
            <div class="mb-6">
                <label
                  for="subject"
                  class="block mb-2 text-sm"
                  >Subject</label
                >
                <input
                  type="text"
                  name="subject"
                  id="subject"
                  required
                  class="input input-bordered w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none  dark:focus:border-gray-500"
                />
              </div>
            <input type="checkbox" name="botcheck" id="" style="display: none;" />
            <div class="mb-6">
              <label
                for="name"
                class="block mb-2 text-sm"
                >Name</label
              >
              <input
                type="text"
                name="name"
                id="name"
                required
                class="input input-bordered w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none  dark:focus:border-gray-500"
              />
            </div>
            <div class="mb-6">
              <label
                for="email"
                class="block mb-2 text-sm"
                >Email Address</label
              >
              <input
                type="email"
                name="email"
                id="email"
                required
                class="input input-bordered w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none  dark:focus:border-gray-500"
              />
            </div>
            
            <div class="mb-6">
              <label
                for="message"
                class="block mb-2 text-sm"
                >Message</label
              >
  
              <textarea
                rows="5"
                name="message"
                id="message"
                class="input input-bordered w-full px-3 py-2 border border-gray-300 rounded-md focus:outline-none  dark:focus:border-gray-500"
                required
              ></textarea>
            </div>
            <div class="mb-6">
              <button
                type="submit"
                class="w-full px-3 py-4 bg-primary rounded-md hover:bg-primary-focus text-base-100"
              >
                Send Message
              </button>
            </div>
            <p class="text-base text-center text-gray-400" id="result"></p>
          </form>
        </div>
      </div>
    </div>
  </div>