<style>
    .btn-outline {
        margin-left: auto;
        display: inline-flex;
    }

    .box-1 {
        display: flex;
        justify-content: flex-end;
        flex-direction: column;
    }
</style>
<script>
    import ProjectItem from "./ProjectItem.svelte";

    export let projectsToShow, showMore;
</script>
<div class="box-1">
    <h1>Project</h1>
    {#each projectsToShow as project}
        <ProjectItem {...project}/>
    {/each}

    {#if showMore}
        <a href={showMore} class="btn-outline">see more</a>
    {/if}

</div>
