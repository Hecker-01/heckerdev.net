<script>
  let currentYear = new Date().getFullYear();

  let socials = [
    {
      icon: "fab fa-discord",
      href: "https://discord.heckerdev.net/",
    },
    {
      icon: "fab fa-github",
      href: "https://github.com/hecker-01",
    },
    {
      icon: "fas fa-envelope",
      href: "mailto://info@heckerdev.net",
    },
  ];
</script>

<footer
  class=" bg-black border-t border-solid border-violet-950 flex flex-col justify-center items-center w-full pb-[40]"
>
  <div class="flex justify-between items-center max-w-4xl w-[80%] py-5">
    <div class="text-[15px] w-[205] text-left">
      <h1 class=" text-xl"><strong>This Website</strong></h1>
      <p>
        Was made by <br />
        <a
          href="https://github.com/hecker-01"
          target="_blank"
          class="underline"
          style="text-decoration-color: #A855F7; text-decoration-thickness: 2px;"
          >@Hecker-01</a
        >.
      </p>
    </div>
    <div class="text-right">
      <h1 class="text-xl"><strong>Socials:</strong></h1>
      <div class="flex flex-row gap-2 mx-auto">
        {#each socials as social, index}
          <div
            class="w-[30px] h-[30px] bg-white rounded-md flex justify-center items-center"
          >
            <a href={social.href} target="_blank">
              <i
                class="pt-1 pl-[1px] {social.icon}"
                style="color: black; font-size: 20px;"
              ></i>
            </a>
          </div>
        {/each}
      </div>
    </div>
  </div>
  <div
    class="bg-gradient-to-r from-purple-950 to-purple-900 flex flex-col justify-center items-center max-w-5xl w-[80%] rounded-t-xl h-[40px]"
  >
    <p>© HeckerDev.net | 2020 — {currentYear}</p>
  </div>
</footer>
