<template>
        <footer class="footer">
<div class="logo-block">
    <img :src="logo" alt="" class="logo">
</div>
        <div class="social-block">
            <div class="social-link">

<SvgSprite/>
        <svg v-for="(icon, index) in icons" 
        class="social-link__icon icon" 
        :key="`${icon}_${index}`">
        <use :xlink:href="`${icon}`">{{icon}}</use>
    </svg>
            </div>
        </div>
    </footer>
</template>

<script>
import SvgSprite from './SvgSprite'
export default {
    name: 'Footer',
    components:
    { SvgSprite : SvgSprite},
    data: () => ({
        isActive: false,
        activeIndex: null,
        logo: require('../assets/img/mainlogo.png'),
        show: true,
        icons: ['#linkedin', '#facebook', '#instagram', '#behance', '#telegram'],
    }),
    methods: {
    }
}
</script>

