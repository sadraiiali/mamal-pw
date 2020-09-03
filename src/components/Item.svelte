<style>
    .container {
        display: flex;
        justify-content: flex-start;
        align-items: center;
        width: 100%;
        flex-direction: row;
        flex-wrap: wrap;
    }

    .item-box {
        width: 50%;
    }

    .item {
        padding: 25px 25px 25px 0;
        display: flex;
        flex-direction: row;
    }

    .item:hover .vl {
        background-color: var(--color-5);
    }

    .vl {
        background-color: var(--color-6);
        width: 3px;
        border-radius: 4px;
        margin-right: 27px;
        transition: 200ms background-color ease;
    }

    .col {
        display: flex;
        flex-direction: column;
    }

    h3 {
        font-weight: bold;
    }
</style>

<script>
    export let itemToShow = [];
    export let title;
</script>


<div class="box-1">
    <h1>{title}</h1>

    <div class="container">
        {#each itemToShow as ex}
            <div class="item-box">
                <div class="item">
                    <div class="vl"></div>
                    <div class="col">
                        <h3>{ex.title}</h3>
                        <h4>{ex.description}</h4>
                        <span>{ex.time}. {ex.location}</span>
                    </div>
                </div>
            </div>
        {/each}
    </div>
</div>
