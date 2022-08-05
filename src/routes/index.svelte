<svelte:head>
    <meta charset="utf-8">
    <meta name="description" content="Fintech project">
    <meta name="author" content="">
    <link rel="stylesheet" href="https://maxst.icons8.com/vue-static/landings/line-awesome/line-awesome/1.3.0/css/line-awesome.min.css">
</svelte:head>

<script>
    import "../app.css";
    import Nav from '../components/nav.svelte';
    import Main from '../components/main.svelte';
</script>

<style scoped>

</style>

<div class="block md:flex">
    <Nav/>
    <div>
        <Main/>
    </div>
</div>

