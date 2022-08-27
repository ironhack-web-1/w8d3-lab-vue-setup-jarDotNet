<template>
  <div class="page">
    <h1> About me </h1>
    <blockquote>{{ aboutMe }}</blockquote>
  </div>
</template>

<script>
export default {
  data() {
    return {
      aboutMe: `
        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed facilisis
        quam felis, in bibendum ligula vehicula vitae. Vestibulum at dapibus 
        ligula. Nunc viverra sollicitudin est. Class aptent taciti sociosqu ad
        litora torquent per conubia nostra, per inceptos himenaeos. Praesent 
        volutpat, odio sit amet porttitor rhoncus, nibh tellus facilisis odio, 
        a viverra tellus quam et dui. Vivamus vulputate libero sed magna 
        aliquam, vitae rutrum risus maximus. In iaculis ultrices lorem, id 
        dignissim ante malesuada in. Maecenas commodo sed odio non vehicula. In
        mauris libero, bibendum eget bibendum iaculis, scelerisque id felis.
        `,
    };
  },
};
</script>

<style scoped>
@import "@fontsource/medievalsharp";

div {
  font-family: MedievalSharp;
  font-size: 20px;
}

h1 {
  margin-left: 90px;
}

pre {
  font-style: normal;
  font-variant: normal;
  font-weight: 400;
  line-height: 20px;
}

blockquote::before {
  content: open-quote;
}

blockquote::after {
  content: close-quote;
}

blockquote {
  quotes: "“" "”" "‘" "’";
  max-width: 600px;
  margin-left: 90px;
}

.page {
  background-color: #f8f5de;
  background-image: linear-gradient(to right, rgba(255,210,0,0.4), rgba(200, 160, 0, 0.1) 11%, rgba(0,0,0,0) 35%, rgba(200, 160, 0, 0.1) 65%);
  box-shadow: inset 0 0 75px rgba(255,210,0,0.3), inset 0 0 20px rgba(255,210,0,0.4), inset 0 0 30px rgba(220,120,0,0.8);
  color: rgba(0,0,0,0.5);
  letter-spacing: 0.05em;
  padding: 5em 10em 5em 5em;
}
</style>