<template>
  <body>
    <Header/>
    <Nav/>
    <main>
        <BrandCooperation/>
        <NewCollection/>
        <BestSeller/>
    </main>
    <Footer/>
  </body>
</template>
<script>
    import Header from './components/Header.vue'
    import Nav from './components/Nav.vue'
    import BrandCooperation from './components/BrandCooperation.vue'
    import NewCollection from './components/NewCollection.vue'
    import BestSeller from  './components/BestSeller.vue'
    import Footer from './components/Footer.vue'

        export default {
          name: "App",
          components:{
          Header,
          Nav,
          BrandCooperation,
          NewCollection,
          BestSeller,
          Footer
          }
        }
</script>


<style scoped>

.btn {
  font-size: var(--fs-btn);
  border-radius: 6px;
}
.btn-yellow {
  background: var(--secondary-background-color);
  color: var(--fc-dark);
}
.btn-yellow:hover {
  background: #ffeb9d;
}
.btn-black,
.btn-black2 {
  background: #181818;
  color: var(--fc-light);
  padding: 16px 40px;
  line-height: 17px;
}
.btn-black:hover {
  background: #1e1e1e;
  color: #ffffff;
}
.btn-black2:hover {
  background: #1e1e1e;
  color: #ffffff;
}
.z-index{
  z-index: 2;
}
</style>
