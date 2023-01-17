
<template>
<nav class="img-navbar d-lg-none d-xl-none d-xxl-none ">
    <div class="container">
        <ul class="d-flex justify-content-between align-content-center list-unstyled">
            <li >
                <a href="#"><img src="src/assets/images/phone.svg" alt="phone"></a>
            </li>
            <li >
                <a href="#"><img src="src/assets/images/tag.svg" alt="tag"></a>
            </li>
            <li >
                <a href="#"><img src="src/assets/images/home.svg" alt="home"></a>
            </li>
            <li >
                <a href="#"><img src="src/assets/images/store.svg" alt="store"></a>
            </li>
            <li >
                
                <span>{{ counterStore.count }}</span>
                <img src="src/assets/images/cart1.svg" alt="cart">
            </li>
        </ul>
    </div>
</nav>
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

.img-navbar {
  background: var(--secondary-background-color);
  position: sticky;
  top: 0;
  z-index: 9999;
}
.img-navbar {
  height: 48px;
}
.img-navbar img {
  padding-block: 12px;
}
</style> -->