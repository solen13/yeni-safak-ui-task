<template>
  <div class="recommeneded-list">
    <div class="recommeneded-list__header">
      <img
        class="recommeneded-list__header--left-image"
        src="../../public/marka.png"
        alt=""
      />
      <img
        class="recommeneded-list__header--right-image"
        src="https://s3-alpha-sig.figma.com/img/59ab/5ccc/be6dd4692f5b834c6726bcebffb83701?Expires=1718582400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=jN7Ph8o0rAVPSCPDOcqJ7QoB6OvX-NgJs6ZpWkTNzKi9S8I6eEPy3Fqp~4axv9pblHCkaZi1o40kkmErBE9wMLLzrXixySA0YSKz23d2kLiZZsOsjx-h9Vod7L3FABwTeGl6PNKb0q6X9VKwW4bw9s-nJGvXli~iemn0-Bu3sVIpITV8AiyNAvSEwTfpYD1YGt1QLzuWFS8h68WGYGJOQDtoq-ZfYg2VcIzKc0eN8311n6zcI3nHsk0MoRjmACSf4bZWQlPbWIZQP-whSCJR3kfr7G5RwiwbGcmG9i3dXszj0khOPXt583L-yUyCq7AJbM-MEfF6c1nzyD2vebRZBA__"
        alt=""
      />
    </div>
    <ul class="recommeneded-list__list">
      <li class="recommeneded-list__list__item" v-for="item in 6">
        <img
          class="recommeneded-list__list__item--image"
          src="https://s3-alpha-sig.figma.com/img/c54c/0259/93b833ec285e44e02de52eae60f4e792?Expires=1718582400&Key-Pair-Id=APKAQ4GOSFWCVNEHN3O4&Signature=WaVsv5Z~HnmwifuhVJfkvRYR71F0QThahwjhRZJ6O1o4BrFElW0LbO7pv~Wtincp5bQwu6AweN2ErVjTPuy84z7J0iCoTRDNJSmIacchdg52Aq85HzHx1c4HhJSPTYD9vb4Kfx94UhHvvoBaLNH4Wes0RZbtSMHYWJ6Sc6r2swX8vsdTk6r4L~BlIT5e4t6~khwL6JwZkR3RbWZLwaY~cBXUPQtWyIK9L6WUZmAxjgwkC1gVrvVDwwnswao8A3V~C73QHnTArED4K69Y1bxTwtyXJWscsU01oewUjY367UelqmSKfsiR0Wi1BpPVP0N5ackWeGnlvFuJlY9nBoa~5A__"
          alt=""
        />
        <h3 class="recommeneded-list__list__item--text">
          Karaköy’de en sevdiklerimizden: Karabatak! 🧡
        </h3>
      </li>
    </ul>
    <div class="recommeneded-list__button">
      <button class="recommeneded-list__button--item">Daha fazla</button>
    </div>
  </div>
</template>
<style lang="scss" src="./recommended-list.scss"></style>
