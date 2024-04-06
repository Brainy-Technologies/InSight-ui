<script>
	import '../sass/app.scss';
    import '../sass/font.scss';
    import { Header, Footer } from '$lib'
</script>

<div>
    <Header/>
    <slot />
    <Footer/>
</div>
