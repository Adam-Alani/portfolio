<script>
	let showLeft = true
	let showYellow = true
</script>

<hr align="center" width="82%" color= #CD65FF>
<div class="textarea">

  <h1> <span class='color'>&lt;</span>skills<span class='color'>&gt</span></h1>
  <p>Here's what i know what to do</p>


  <ul class="cards">
    <li class="cards__item">
      <div class="card">
        <div class="card__image card__image--fence"></div>
        <div class="card__content">
          <div class="card__title">Programming</div>
          <p class="card__text">This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. Default is 0 1 auto. </p>
        </div>
      </div>
    </li>
    <li class="cards__item">
      <div class="card">
        <div class="card__image card__image--fence"></div>
        <div class="card__content">
          <div class="card__title">Design</div>
          <p class="card__text">This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. Default is 0 1 auto. </p>
        </div>
      </div>
    </li>
    <li class="cards__item">
      <div class="card">
        <div class="card__image card__image--fence"></div>
        <div class="card__content">
          <div class="card__title">Communication</div>
          <p class="card__text">This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. Default is 0 1 auto. </p>
        </div>
      </div>
    </li>
    <li class="cards__item">
      <div class="card">
        <div class="card__image card__image--fence"></div>
        <div class="card__content">
          <div class="card__title">Other</div>
          <p class="card__text">This is the shorthand for flex-grow, flex-shrink and flex-basis combined. The second and third parameters (flex-shrink and flex-basis) are optional. Default is 0 1 auto. </p>
        </div>
      </div>
    </li>



  </ul>






 <h1> <span class='color'>&lt;/</span>skills<span class='color'>&gt</span></h1>

</div>



<style>
  
  .card__title {
    color: #FFE374;
  font-size: 1.25rem;
  font-weight: 100;
  margin-left: 10rem;
  letter-spacing: 2px;
  text-transform: uppercase;
}
  .cards {
  display: flex;
  list-style: none;
  margin: 0;
  padding: 0;
}

  .card__content {
  display: flex;
  flex: 1 1 auto;
  flex-direction: column;
  padding: 1rem;
}
  .card__text {
    color: whitesmoke;
  flex: 1 1 auto;
  font-size: 0.875rem;
  line-height: 1.5;
  margin-bottom: 1.25rem;
}

  .cards {
   display: flex;
   justify-content: space-between;
   flex-basis:0rem;
}


	.textarea {
		text-align: left;
		padding: em;
    margin-top: 20rem;
    margin-left:10rem;
    margin-right:10rem;
	}

  .sub {
    margin-bottom: 5rem;
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
    padding-left: 10rem;
    padding-top: 1%;
    padding-bottom: 1%;

  }



  .color {
    color: #398FFF;
  }

  hr {
    margin-top:15rem;
  }
  

</style>