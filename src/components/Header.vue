<template>
<header>
    <div class="navbar navbar-expand-lg navbar-dark d-none d-lg-block d-xl-block d-xxl-block">
        <div class="container">
            <a id="brand" class="navbar-brand" href="#Etalon" title="etalon">Etalon</a>
            <div>
                <ul class="navbar-nav">
                    <li class="nav-item ">
                        <a class="nav-link " href="#home" title="home">Home</a>
                    </li>
                    <li class="nav-item ">
                        <a class="nav-link " href="#store" title="store">store</a>
                    </li>
                    <li class="nav-item ">
                        <a class="nav-link" href="#new" title="new">New</a>
                    </li>
                    <li class="nav-item ">
                        <a class="nav-link " href="#contact" title="contact">Contact</a>
                    </li>
                </ul>
            </div>
            <div class="cart-container position-relative">
                <span class="number-count rounded-pill py-1 px-2">{{ counterStore.count }}</span>
                <img id="cart" src="src/assets/images/cart.svg" width="40px" alt="shopping-card">
            </div>
            
        </div>
    </div>
    <div class="cover">
        <div class="container">
            <div class="row justify-content-center">
                <div class="cover-details col-12 col-l-5 col-xl-5 col-xxl-5">
                    <span>2022</span>
                    <h1>Autumn Jackets</h1>
                    <h4>Autumn Sale/ Up to 50% OFF</h4>
                    <a class="btn btn-yellow text-capitalize">open collection</a>
                </div>
                <div class="col-12 col-md-12 col-l-6 col-xl-6 col-xxl-6 position-relative">
                    <div class="d-xxl-block d-xl-block d-l-block d-md-block d-none">
                        <img class="layer1 position-absolute" src="src/assets/images/circle-layer.svg" alt="circle-layer">
                        <img class=" layer2 position-absolute" src="src/assets/images/circle-layer.svg" alt="circle-layer">
                    </div>
                    <p id="cover-price" class="position-absolute d-none d-lg-block d-xl-block d-xxl-block">$299</p>
                    <div class="d-none d-xl-block d-xxl-block">
                        <span class="flash1 icon-flash-left"></span>
                        <span class="flash2 icon-flash-right"></span>
                    </div>
                    <picture class="cover-img position-relative " >
                        <source srcset="src/assets/images/men-with-helmet.png "  media="(min-width:768px)">
                        <source srcset="src/assets/images/Group 2.svg" >
                        <img src="src/assets/images/Group 2.svg" alt="men-with-helmet">
                    </picture>
                    <img class="off position-absolute d-none d-lg-block d-xl-block d-xxl-block" src="src/assets/images/off.svg" alt="%off">
                </div>
                <div class="circles position-relative col-12 col-l-1 col-xl-1 col-xxl-1 m-auto">
                    <a href="#"><div class="circle1"></div></a>
                    <a href="#"><div class="circle2"></div></a>
                    <a href="#"><div class="circle3"></div></a>
                </div>
            </div>
        </div>
    </div>
</header>
</template>
<script>
    import { useCounterStore } from '../stores/counter';
    import { mapStores } from 'pinia';
    export default{
        computed:{
            ...mapStores(useCounterStore)
        }
    }
</script>
<!-- <style scoped>

/* ---navbar--- */
.navbar {
  font-family: var(--body-font-family);
  margin-inline: 16px;
}
.navbar a:hover {
  color: var(--fc-light);
}

#cart:hover {
  transform-origin: conter;
  transform: scale(1.2);
  cursor: pointer;
}
.cart:hover {
  transform-origin: conter;
  transform: scale(1.1);
  cursor: pointer;
  opacity: 0.9;
}

/* ---cover--- */
.cover-details {
  margin-block: 85.13px;
}
.cover span {
  font-style: italic;
  font-weight: 400;
  font-size: var(--fs-xl);
  line-height: 72px;
  color: rgba(255, 255, 255, 0.3);
}
.cover h1,
.cover h4 {
  margin-top: 24px;
}
.btn-yellow {
  margin-block: 49px;
  padding: 16px 40px;
}
#cover-price {
  color: var(--fc-light);
  font-size: var(--fs-l);
  font-weight: 500;
  line-height: 43px;
  top: 142.63px;
  left: 143px;
}
.cover-img {
  width: 100%;
  z-index: 2;
  top: 63.63px;
  left: 229px;
}
.layer1 {
  left: 158.25px;
  bottom: 77.55px;
}
.layer2 {
  left: 339.15px;
  bottom: 184.33px;
}
.off {
  left: 229.15px;
  bottom: 395.63px;
  z-index: 3;
}
.circle1,
.circle2,
.circle3 {
  transition: all 0.4 ease;
  margin-block: 21px;
  width: 16px;
  height: 16px;
  background: rgba(255, 255, 255, 0.2);
  border-radius: 21px;
  transform: translateX(50px);
}
.circles > * :hover {
  background-color: white;
  transform: scale(1.1);
  transform: translateX(50px);
}
.flash1,
.flash2 {
  display: inline-block;
  position: absolute;
  padding: 12px;
  width: 36px;
  height: 36px;
  background-size: cover;
  bottom: 32px;
}
.flash1 {
  left: 179px;
}
.flash2 {
  left: 227px;
}
.icon-flash-left {
  background-image: url(../images/flash-left.svg);
}
.icon-flash-left:hover,
.icon-flash-left:focus {
  background-image: url(../images/flash-left-hover.svg);
  cursor: pointer;
  transition: all 0.6 ease;
}
.icon-flash-right {
  background-image: url(../images/flash-right.svg);
  transform: rotateX("180deg");
}
.icon-flash-right:hover,
.icon-flash-right:focus {
  background-image: url(../images/flash-right-hover.svg);
  cursor: pointer;
  transition: all 0.6 ease;
}
</style> -->
