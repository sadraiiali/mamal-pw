<style>
    .item-box {
        width: 100%;
    }

    .item {
        padding: 25px 25px 25px 0;
        display: flex;
        flex-direction: row;
        align-items: center;
    }

    .item:hover .vl {
        background-color: var(--color-5);
    }

    .item:hover img {
        border-color: var(--color-5);
    }

    .vl {
        background-color: var(--color-6);
        width: 3px;
        border-radius: 4px;
        margin-right: 27px;
        transition: 200ms background-color ease;
        height: 150px;
    }

    .col {
        display: flex;
        flex-direction: column;
    }

    h3 {
        font-weight: bold;
    }

    img {
        margin-left: auto;
        border-radius: 100%;
        border: 2px solid transparent;
        transition: 200ms border-color ease-in-out;
    }

    .row {
        display: flex;
        flex-direction: row;
        align-items: center;
    }
</style>

<script>
    export let title, description, time, img;
</script>

<div class="item-box">
    <div class="item">
        <div class="row">
            <div class="vl"></div>
            <div class="col">
                <h3>{title}</h3>
                <h4>{description}</h4>
                <span>{time}</span>
            </div>
        </div>
        <img src={img} alt="{title}'s Project Img">
    </div>
</div>
