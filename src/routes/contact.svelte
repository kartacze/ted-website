<script>
  import LinkedinIcon from "../../static/svg/linkedin.svg";
  import MailIcon from "../../static/svg/mail.svg";
  import PhoneIcon from "../../static/svg/phone.svg";
  import { fade } from "svelte/transition";
</script>

<style>
  .wrapper {
    height: 100%;
    width: 100%;
  }

  h1 {
    margin-bottom: 25px;
  }
  .Contact-body {
    display: flex;
    flex-direction: column;
    justify-content: space-evenly;
  }

  .Contact-body :global(svg) {
    height: 25px;
    width: 25px;
    fill: var(--second-color);
  }

  .icon {
    height: 25px;
  }

  .text {
    margin-left: 20px;
  }

  ul {
    padding: 0;
    list-style-type: none;
  }

  li {
    display: flex;
    margin-top: 1em;
    align-items: center;
  }
</style>

<svelte:head>
  <title>Contact</title>
</svelte:head>

<div class="wrapper" transition:fade style="position:absolute">
  <h1>Contact info</h1>

  <div class="Contact-body">
    <ul>
      <li>
        <div class="icon">{@html LinkedinIcon}</div>
        <div class="text">
          <a href="https://www.linkedin.com/in/teodor-pytka" target="_blank">
            linkedin.com/in/teodor-pytka
          </a>
        </div>
      </li>
      <li>
        <div class="icon">{@html MailIcon}</div>
        <div class="text">
          <a href="mailto:teodorpytka@gmail.com">teodorpytka@gmail.com</a>
        </div>
      </li>
      <li>
        <div class="icon">{@html PhoneIcon}</div>
        <div class="text">
          <a href="tel:0048533466451">+48 533 466 451</a>
        </div>
      </li>
    </ul>
  </div>
</div>
