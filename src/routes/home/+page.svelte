<script>
</script>

<template>
	<div class="container">
		<h1>Svelte</h1>
		<!-- description what is svelte -->
		<p>
			Svelte is a new way to build web applications. It's a compiler that takes your declarative
			components and converts them into efficient JavaScript that surgically updates the DOM.
		</p>
        <div class="container-form">
            <!-- input for send email -->
            <input type="email" placeholder="Enter your email" />
            <!-- button for send email -->
            <button>Subscribe</button>
        </div>
	</div>
</template>

<!-- Language: svelte -->
<style>
    h1{ 
        color: #fff;
        text-align: center;
        font-weight: bold;
        font-size: 8rem;
        z-index: 100;
    }
    p{
        color: #fff;
        text-align: center;
        font-size: 1.2rem;
        z-index: 100;
        width: 50%;
    }
    .container-form{
        display: flex;
        justify-content: center;
        align-items: center;
        margin-top: 2rem;
    }
    input{
        outline: none;
        height: 3rem;
        z-index: 100;
        border: 3px solid transparent;
        border-image: linear-gradient(120deg, #32a8f8 0%, #b932f8 50%, #ff2768 100%) 1;
        border-radius: 5px;
        padding: 0 1rem;
        background-color: transparent;
        color: #fff;
        font-size: 1.2rem;
    }
    button{
        outline: none;
        height: 3rem;
        z-index: 100;
        border: 3px solid transparent;
        border-image: linear-gradient(120deg, #32a8f8 0%, #b932f8 50%, #ff2768 100%) 1;
        border-radius: 5px;
        padding: 0 1rem;
        background-color: transparent;
        color: #fff;
        font-size: 1.2rem;
        margin-left: 1rem;
        cursor: pointer;
    }
    .container{
        width: 100%;
        height: 100vh;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }
    .container::before {
      content: "";
      position: fixed;
      width: 200px;
      height: 200px;
      left: 35%;
      top: 30%;
      filter: blur(90px);
	    background-image: linear-gradient(120deg, #32a8f8 0%, #b932f8 100%);

    }
    .container::after {
      content: "";
      position: fixed;
      width: 200px;
      height: 200px;
      left: 55%;
      top: 30%;
		background-image: linear-gradient(120deg, #b932f8 0%, #ff2768 100%);
      filter: blur(80px);
    }
</style>
