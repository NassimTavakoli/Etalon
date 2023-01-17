<template>
    <section class="new-collection">
            <div class="container">
                <h3 class="text-capitalize">new collection</h3>
                <ul class="row list-unstyled g-4 mb-5">
                    <li class="col-12 col-l-5 ">
                        <div class="d-flex flex-column">
                            <div class="jacket-collection position-relative m-1">
                                <p class="text-capitalize">Men’s Jacket Collection</p>
                                <picture>
                                    <source srcset="src/assets/images/men-jeans-coat.png"  media="(min-width:770px">
                                    <source srcset="src/assets/images/men-jeans-coat-sm.png" >
                                    <img src="src/assets/images/men-jeans-coat-sm.png" alt="men-with-helmet">
                                </picture>
                                <a class="btn btn-black" href="#" title="discover">Discover Now</a>
                            </div>
                        </div>
                    </li>
                    <li class="col-12 col-l-7 ">
                        <div class="sunglasses-collection d-flex position-relative">
                            <picture class="col-6 col-md-7 col-l-7 col-xl-7 col-xxl-7">
                                <source srcset="src/assets/images/men-tshirt.png"  media="(min-width:770px">
                                <source srcset="src/assets/images/men-tshirt-sm.png" >
                                <img src="src/assets/images/men-tshirt-sm.png" alt="men-with-helmet">
                            </picture>
                            <div class="col-6 col-md-5  col-l-5 col-xl-5 col-xxl-5">
                                <p class="body-p text-capitalize">Men’s Sunglasses Collection</p>
                                <span class="text-uppercase offer">40% off</span>
                                <a class="btn btn-black" href="#" title="discover">Discover Now</a>
                            </div>
                        </div>
                    </li>
                </ul>
            </div>
        </section>
</template>
<!-- <style scoped>
.new-collection{
    background-color:var(--white-background-color);
}
.jacket-collection,
.sunglasses-collection {
  border-radius: 24px;
 
}
.jacket-collection {
  background-color: var(--primary-dark-background-color);
}
.sunglasses-collection {
  background-color: var(--secondary-background-color);
}
.jacket-collection picture {
  object-fit: cover;
  object-position: center;
  margin-left: 110.67px;
  max-height: 478.88px;
  max-width: 278.66px;
}
.btn-black {
  position: absolute;
  bottom: 24px;
  right: 24px;
  z-index: 1;
}
.sunglasses-collection picture {
  margin-top: 30.64px;
  object-fit: cover;
  object-position: center;
  max-height: 520.12px;
  max-width: 455.14px;
}
.jacket-collection p,
.sunglasses-collection p {
  font-size: var(--fs-body);
  font-weight: 700;
  line-height: 40px;
}
.jacket-collection p {
  margin: 24px 0 5px 24px;
}
.sunglasses-collection p {
  margin-top: 71.87px;
  margin-inline: auto;
  max-width: 200px;
  text-align: center;
}
.offer {
  display: block;
  font-family: var(--secondary-font-family);
  font-size: var(--fs-h3);
  font-weight: 700;
  line-height: 56px;
  margin-top: 95.51px;
  text-align: center;
} 

</style> -->