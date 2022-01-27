<template>
  <ol>
    <!-- <li property="itemListElement" typeof="ListItem">
      <NLink property="item" typeof="WebPage" to="/">
        <span property="name">Vonage Learn</span>
      </NLink>
      <meta property="position" content="1" />
    </li> -->
    <li
      v-for="(crumb, index) in crumbs"
      :key="index"
      property="itemListElement"
      typeof="ListItem"
    >
      <NLink property="item" typeof="WebPage" :to="crumb.path">
        <span property="name">{{
        crumb.name
        }}</span>
      </NLink>
      <meta property="position" :content="index + 2" />
    </li>
  </ol>
</template>

<script>
export default {
  name:'Breadcrumbs',
  
computed: {
    crumbs() {
      const fullPath = this.$route.fullPath
      const params = fullPath.substring(1).split('/')
      const crumbs = []

      let path = ''
      console.log('crumbs', crumbs)
      params.forEach((param, index) => {
        path = `${path}/${param}`
        const match = this.$router.match(path)
        console.log('path', path)
        if (match.name !== null) {
          crumbs.push(match)
        }
      })

      return crumbs
    },
  },
}
</script>

<style scoped>
ol {
  list-style: none;
}
li {
  display: inline;
}
li:after {
  content: ' » ';
  display: inline;
  font-size: 0.9em;
  color: #aaa;
  padding: 0 0.0725em 0 0.15em;
}
li:last-child:after {
  content: '';
}
li a {
  color: black;
}
li a.nuxt-link-exact-active.nuxt-link-active {
  color: rgb(255, 166, 1);
}
li a:visited{
  color:orange;
}
</style>