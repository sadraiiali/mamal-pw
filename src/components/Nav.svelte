<script>
    export let segment;
</script>

<style>
    nav {
        border-bottom: var(--nav-border-size) solid var(--color-6);
        font-weight: 300;
        padding: 0;
        margin-bottom: 50px;
    }

    ul {
        margin: 0;
        padding: 17px 0;
        display: flex;
        justify-content: center;
        align-items: center;
    }

    /* clearfix */
    ul::after {
        content: '';
        display: block;
        clear: both;
    }

    li {
        display: block;
        float: left;
        margin-left: 30px;
    }

    [aria-current] {
        position: relative;
        display: inline-block;
        font-weight: bold;
    }


    a {
        text-decoration: none;
        padding: 0;
        display: inline-flex;
        margin: 0 20px;
        font-size: var(--font-size-2);
        font-family: var(--font-2);
    }


    .home {
        margin-right: auto;
        font-family: var(--second-font);
        display: flex;
        justify-content: center;
        align-items: center;
        font-size: var(--font-size-1);
    }

    .home img {
        margin-right: 30px;
    }

    .home span {
        margin-top: calc(var(--font-size-1) / 4);
    }

</style>

<nav>
    <ul>
        <li class="home">
            <img src="icons/home.svg" height="35" alt="Home Icon">
            <span>
                Mohammad Reza Mirzaei
            </span>
        </li>
        <li><a aria-current="{segment === undefined ? 'page' : undefined}" href=".">EXPERINCE</a></li>
        <li><a aria-current="{segment === 'projects' ? 'page' : undefined}" href="projects">Projects</a></li>

        <!-- for the blog link, we're using rel=prefetch so that Sapper prefetches
             the blog data when we hover over the link or tap it on a touchscreen -->
        <li><a rel=prefetch aria-current="{segment === 'blog' ? 'page' : undefined}" href="">CV</a></li>
        <li class="btn-1">
            <a rel=prefetch aria-current="{segment === 'contact' ? 'page' : undefined}" href="contact">contact</a>
        </li>

    </ul>
</nav>
