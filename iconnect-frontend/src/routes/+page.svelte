<script>
  import SpinningCard from "../components/SpinningCard.svelte";
  import Wave from "../components/LandingPageAssests/Wave.svelte";
  import BuyLink from "../components/LandingPageAssests/BuyLink.svelte";
  import HeroText from "../components/LandingPageAssests/HeroText.svelte";
  import Spacer from "../components/LandingPageAssests/Spacer.svelte";
  import About from "../components/About.svelte";
  import Info from "../components/Info.svelte";
  import Features from "../components/Features.svelte";
  // import Footer from "../components/Footer.svelte";
</script>

<svelte:head>
  <title>iConnect - Connect Easier with NFC cards</title>
  <meta name="description" content="This is iConnect, a startup that's going to revolutionize the NFC card game. Purchase top of thel line google NFC cards.">
</svelte:head>


<Spacer />
<section class="home">
  <HeroText />
  <BuyLink />
  <SpinningCard />
  <Wave />
</section>
<Features />
<Info />
<About />

<style>
  @import url("https://fonts.googleapis.com/css2?family=Cabin+Condensed&display=swap");

  * {
    font-family: "Cabin Condensed", sans-serif;
  }
  @keyframes bepur {
    0% {
      fill: #6ee2f5;
    }
    100% {
      fill: #8c1cff;
    }
  }

  @keyframes beblue {
    0% {
      fill: #8c1cff;
    }
    100% {
      fill: #6ee2f5;
    }
  }

  @keyframes opac {
    0% {
      fill-opacity: 0%;
    }
    100% {
      fill-opacity: 80%;
    }
  }

  .home {
    position: relative;

    display: grid;
    grid-template-columns: repeat(50, 2vw);
    grid-template-rows: repeat(50, 2vh);
    align-items: center;

    height: 100vh;
    width: 100vw;
  }

  @media (max-width: 425px) {
    .home {
      display: flex;
      flex-direction: column;
      height: auto;
      width: auto;
    }
  }

  /* Landing links */

  /* End of links */
</style>
