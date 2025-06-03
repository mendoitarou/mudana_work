<template>
    <span>
        <a href="https://twitter.com/share?ref_src=twsrc%5Etfw" class="twitter-share-button" data-size="large" data-text="無駄なwork" data-url="https://mudana.work/" data-show-count="false">Tweet</a>
    </span>
</template>

<script>
export default {
    mounted () {
        const script = document.createElement('script');
        script.src = 'https://platform.twitter.com/widgets.js';
        script.async = true;
        document.body.appendChild(script);
        return () => {
            document.body.removeChild(script);
        }
    }
}
</script>
