<script>
    import Nav from '../components/Nav.svelte';
    import Contacts from "../components/Contacts.svelte";

    export let segment;
</script>

<style>
    main {
        position: relative;
        padding: 2em;
        margin: 0 auto;
        box-sizing: border-box;
    }

    .main-box {
        max-width: var(--max-body-wigt);
        width: 100%;
    }

    .container {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        width: 100%;
    }
</style>

<div class="container">
    <div class="main-box">
        <Nav {segment}/>

        <main>
            <slot></slot>
            <Contacts/>
        </main>

    </div>
</div>
