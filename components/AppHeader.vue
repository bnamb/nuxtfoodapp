<template>
  <section class="masthead" role="img" aria-label="Image Description">
      <h1>
        Brenda's Restaurant Guide
      </h1>
        <nuxt-link to="/restaurants">
      <button>
          See Restaurants >
      </button>
        </nuxt-link>
  </section>
</template>

<script>
  export default {

  }
</script>

<style lang="scss" scoped>
  .masthead {
    margin: auto;
    width: 100%;
    padding: 40px;
    height: 90vh; /* if you don't want it to take up the full screen, reduce this number */
    overflow: hidden;
    background-size: cover !important;
    background: radial-gradient(ellipse at center, rgba(0,0,0,0) 0%, rgba(0,0,0,0) 80%, rgba(0,0,0,0.65) 100%), url(~assets/headerimg.jpg) no-repeat center center scroll;
    display: flex;
    align-items: center;
    flex-direction: column;
    justify-content: center;
  }

  h1 {
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
    font-style:normal;
    font-weight: bold;
    color: #eee;
    font-size: 10vmin;
    letter-spacing: 0.03em;
    line-height: 1;
    text-shadow: 1px 2px 4px rgba(0, 0, 0, 0.8);
    margin-bottom: 25px;
  }

</style>


