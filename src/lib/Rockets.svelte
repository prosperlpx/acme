<script>
  import Card from "../components/Card.svelte";
  import rocketman from '../assets/img/rocketman.png';
  import rocketlaunch from '../assets/img/rocketlaunch.png';
  import rocketride from '../assets/img/rocketride.png';

</script>

<main>
  <section class="my-20 max-w-4xl mx-auto p-6 scroll-mt-20 sm:scroll-mt-0" id="rockets">
    <h1 class="text-4xl font-bold text-center">Our Rockets</h1>
    <Card>
      <li class="bg-black border border-solid border-white p-8 rounded-2xl">
        <img src={rocketman} alt="rocketman">
      </li>

      <li class="bg-black border border-solid border-white p-8 rounded-2xl">
        <img src={rocketlaunch} alt="rocketman">
      </li>

      <li class="bg-black border border-solid border-white p-8 rounded-2xl">
        <img src={rocketride} alt="rocketman">
      </li>
    </Card>   
  </section>
  

  <hr class="w-1/2 mx-auto">
</main>