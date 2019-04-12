<template>
    <div class="default-layout">

        <!-- header --> 
        <Header-Front></Header-Front>
        <!-- header end -->

        <!-- View of Home --> 
        <main class="main-content">
            <div class="container">
                <slot class="content"></slot>
            </div>            
        </main>
        <!-- View of Home end -->

        <!-- footer --> 
        <Footer-Front></Footer-Front>
        <!-- footer end -->

    </div>
</template>

<script>
import HeaderFront from '@/partials/HeaderFront'
import FooterFront from '@/partials/FooterFront'
export default {
    name: 'DefaultLayout',
    components: {
        HeaderFront,
        FooterFront
    }
}
</script>