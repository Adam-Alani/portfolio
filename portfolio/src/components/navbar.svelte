<script>
  export let menu = 1;
  import Hover from './hover.svelte'
    
</script>

<style>

  ul {
    list-style-type: none;
    margin: 0;
    padding: 0;
    overflow: hidden;
  }

  li {
    height:70px;
    float:left;
  }
  
  li a {
    margin: 0;
    display: flex;
    height: 45px;
    color:whitesmoke ;
    text-align: center;
    padding: 1rem 3rem;

  }
  
  .active {
    text-underline-position: under;
    text-decoration: underline;
  }
  
</style>


<Hover let:hover={active}>
  <div class:active>
<ul id="menu">
	<li><a href="/" on:click|preventDefault={() => (menu = 1)}>&lt;home&gt;</a></li>
  <li><a href="/" on:click|preventDefault={() => (menu = 2)}>&lt;about-me&gt;</a></li>
  <li><a href="/" on:click|preventDefault={() => (menu = 1)}>&lt;projects&gt;</a></li>
  <li><a href="/" on:click|preventDefault={() => (menu = 2)}>&lt;art&gt;</a></li>
  <li><a href="/" on:click|preventDefault={() => (menu = 2)}>&lt;contact-me&gt;</a></li>
</ul>
</div>
</Hover>
