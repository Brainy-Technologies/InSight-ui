<script>
	import '../sass/app.scss';
    import '../sass/font.scss';
    import { Header, Footer } from '$lib'
</script>

<div>
    <Header/>
    <div class="pt-20">
        <slot />
    </div>
    <Footer/>
</div>
