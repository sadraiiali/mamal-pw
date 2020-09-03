<style>
    h1 {
        font-family: var(--second-font);
    }

    .box-1 {
        padding: 50px;
        margin: 25px;
    }

    .box {
        display: flex;
        flex-direction: row;
    }

    .pic {
        margin-right: 3%;
    }

    .pic img {
        border-radius: 100%;
    }

    .about {
        font-weight: bold;
    }

    h3 {
        font-weight: bold;
        margin: 0;
    }

    ul {
        list-style: none;
        padding: 0;
        margin: 0;
    }

    li {
        font-weight: normal;
    }

    .row {
        display: flex;
        justify-content: center;
        align-items: flex-start;
        flex-direction: row;
    }

    .intrest {
        width: 30%;
    }

    .education {
        width: 70%;
    }

    .education span {
        font-weight: var(--font-light);
    }
</style>

<script>

    const intrests = [
        "Robotics",
        "Mechatronics",
        "Motion Planning",
        "Control",
        "Applied Design",
    ];

    const education = [
        {
            degree: 'BSc',
            field: "Mechanical Engineering",
            time: "2015-2020",
            university: "K.N. Toosi University of Technology"
        }
    ];
</script>
<div class="box-1">
    <div class="head">
        <h1>About Me</h1>
    </div>
    <div class="box">
        <div class="pic">
            <img src="me.jpg" alt="Mohamad Reza Mirzaei's pic">
        </div>
        <div class="body">
            <div class="about">
                <p>
                    Hi. My name is MohammadReza Mirzaei. Recently, I graduted from K.N.Toosi University and I’m looking
                    to
                    continue my studies in the areas that I am intrested in.
                    Previously, I was a mechanical engineering student at K.N. Toosi University of Technology in Iran.
                    During my time in KNTU, I was privilaged to work in 3 research groups, under supervision of Prof.
                    Hamid
                    D. Taghirad, Dr. Ravandi, and Dr. Najafi.
                </p>
                <div class="row">
                    <div class="intrest">
                        <h3>Intrests:</h3>
                        <ul>
                            {#each intrests as intrest}
                                <li>{intrest}</li>
                            {/each}
                        </ul>
                    </div>

                    <div class="education">
                        <h3>Educations:</h3>
                        {#each education as ed }
                            <div>
                                {ed.degree} in {ed.field}, {ed.time}
                                <br>
                                <span>{ed.university}</span>
                            </div>
                        {/each}
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
