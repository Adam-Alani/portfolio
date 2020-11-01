<script>
  let y;
  import { fade, fly } from 'svelte/transition';
</script>

<hr align="center" width="82%" color= #CD65FF>
<div class="textarea">

    <h1><span class='color'>&lt;</span>projects<span class='color'>&gt</span></h1>

  <div class="sub">
    <div class="verticalLine">
      {#if y >= 1050}
      <p in:fade out:fly={{x:100}}>Auto_Channel  &#123;</p>
      {/if}
        <div class="verticalLine">
          <p1>A discord bot to organise and create channels, reducing spam and clutter.</p1>
          <br>
          <p2>Programmed with Javascript and NodeJS, Hosted on AWS.</p2>
          <br>
          <a href="https://github.com/Adam-Alani/AutoChannel/" target="_blank">Visit Github</a>
        </div>
      <p> &#125</p>

      {#if y >= 1350}
      <p in:fade out:fly={{x:100}}>Mood_Classification  &#123;</p>
      {/if}
      <div class="verticalLine">
        <p1>Neural network to classify playlists based on their "mood". ( + a spotify scraper )</p1>
        <br>
        <p2>Programmed with Python and Tensorflow, using the Spotify API.</p2>
        <br>
        <a href="https://github.com/Adam-Alani/AutoChannel/" target="_blank">Visit Github</a>
      </div>
    <p> &#125</p>

    {#if y >= 1650}
    <p in:fade out:fly={{x:100}}>Covid_Tracker  &#123;</p>
    {/if}
    <div class="verticalLine">
      <p1>Using datasets online, I built this COVID-19 tracker back in march.</p1>
      <br>
      <p2>Programmed with Python and Pandas, data shown using MatPlotLib.</p2>
      <br>
      <a href="https://github.com/Adam-Alani/AutoChannel/" target="_blank">Visit Github</a>
    </div>
  <p> &#125</p>

  {#if y >= 1950}
  <p in:fade out:fly={{x:100}}>Amazon_Tracker  &#123;</p>
  {/if}
  <div class="verticalLine">
    <p1>A quick build, i wrote this in order to keep track of some products i wanted to buy during the holiday season.</p1>
    <br>
    <p2>Programmed with Python using Pandas and BeautifulSoup.</p2>
    <br>
    <a href="https://github.com/Adam-Alani/AutoChannel/" target="_blank">Visit Github</a>
  </div>
<p> &#125</p>
      
    </div>
  </div>

  <h1><span class='color'>&lt;</span>projects<span class='color'>&gt</span></h1>

</div>

<svelte:window bind:scrollY={y}/>


<style>
	.textarea {
		text-align: left;
		padding: 1em;
    margin-top: 10rem;
    margin-left:10rem
	}

  .sub {
    margin-left: -2rem;
    width: 37rem;
  }

	h1 {

		line-height: 1 ;
		text-align: left;
		color: whitesmoke;
		font-size: em;
    font-weight: 100;
    padding-top: 1.5rem;
    padding-bottom: .5rem;
  }
  
  p {
    font-size: 1.5em;
    color: #FFE374;
    padding-left: 5rem;
    padding-top: 1%;
    padding-bottom: 1%;
  

  }

  p1 {
		line-height: 1 ;
		text-align: left;
		color: whitesmoke;
		font-size: 1.5em;
		font-weight: 100;
    position: relative;
    left: 4.3rem;

  }
  p2 {
		line-height: 1.5 ;
		text-align: left;
		color: rgb(226, 226, 226);
    font-size: 1em;
    font-style: italic;
		font-weight: 100;
    position: relative;
    left: 4.3rem;

  }

  a {
		line-height: 2 ;
		text-align: left;
		color: #a9ff67;
		font-size: 1.25em;
		font-weight: 100;
    max-width: 50px;
    padding-left: 4.3rem;
  }
  .color {
    color: #398FFF;
  }

  hr {
    margin-top:10rem;
  }

    
  .verticalLine {
  border-left: thin solid #949494;
  margin-left: 7.5rem;
}



</style>