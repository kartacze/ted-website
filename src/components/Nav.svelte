<script>
  export let segment;
</script>

<style>
  nav {
    border-bottom: 1px solid var(--second-color);
    font-weight: 300;
    padding: 0 1em;
    background-color: var(--third-color);
  }
  ul {
    margin: 0;
    padding: 0;
  }

  /* clearfix */
  ul::after {
    content: "";
    display: block;
    clear: both;
  }

  li {
    display: block;
    float: left;
  }

  .selected {
    position: relative;
    display: inline-block;
  }

  .selected::after {
    position: absolute;
    content: "";
    width: calc(100% - 1em);
    height: 6px;
    background-color: var(--second-color);
    display: block;
    bottom: -3px;
  }

  a {
    text-decoration: none;
    padding: 1em 0.5em;
    display: block;
    color: var(--first-color);
  }

  div {
    max-width: 58em;
    margin: 0 auto;
  }
</style>

<nav>
  <div>
    <ul>
      <li>
        <a class='{segment === undefined ? "selected" : ""}' href=".">home</a>
      </li>
      <li>
        <a class='{segment === "contact" ? "selected" : ""}' href="contact"
          >contact</a
        >
      </li>
      <li>
        <a class='{segment === "blog" ? "selected" : ""}' href="blog">blog</a>
      </li>
    </ul>
  </div>
</nav>

