<script>
    import AboutMe from "../components/AboutMe.svelte";
    import Item from "../components/Item.svelte";
    import ProjectView from "../components/ProjectView.svelte";

    const experience = [
        {
            title: 'Reseach Assistant',
            description: 'Dr. Najafi’s Reserch Group',
            time: 'Sep 2019 - Present ',
            location: 'K. N. Toosi University of Technology'
        },
        {
            title: 'Teaching Assistant',
            description: 'Technical Drawing II',
            time: 'Sep 2019 - Present ',
            location: 'K. N. Toosi University of Technology'
        },
        {
            title: 'Reseach Assistant',
            description: 'Dr. Najafi’s Reserch Group',
            time: 'Sep 2019 - Present ',
            location: 'K. N. Toosi University of Technology'
        },
        {
            title: 'Teaching Assistant',
            description: 'Technical Drawing II',
            time: 'Sep 2019 - Present ',
            location: 'K. N. Toosi University of Technology'
        }, {
            title: 'Reseach Assistant',
            description: 'Dr. Najafi’s Reserch Group',
            time: 'Sep 2019 - Present ',
            location: 'K. N. Toosi University of Technology'
        },
        {
            title: 'Teaching Assistant',
            description: 'Technical Drawing II',
            time: 'Sep 2019 - Present ',
            location: 'K. N. Toosi University of Technology'
        },
    ];

    const honors = [
        {
            title: '3rd Place, RoboCup Asia Pacific',
            description: 'Real Rescue Robots League',
            time: '2018',
            location: 'Iran'
        },
        {
            title: '3rd Place, RoboCup Asia Pacific',
            description: 'Real Rescue Robots League',
            time: '2018',
            location: 'Iran'
        },
        {
            title: '3rd Place, RoboCup Asia Pacific',
            description: 'Real Rescue Robots League',
            time: '2018',
            location: 'Iran'
        },
        {
            title: '3rd Place, RoboCup Asia Pacific',
            description: 'Real Rescue Robots League',
            time: '2018',
            location: 'Iran'
        },
        {
            title: '3rd Place, RoboCup Asia Pacific',
            description: 'Real Rescue Robots League',
            time: '2018',
            location: 'Iran'
        },
    ];


    const projects = [
        {
            title: 'Camera Dolly',
            description: 'Designing a camera dolly with a hydraulic manipulator',
            time: '2020',
            img: './projectImg/example-project.jpg'
        },
        {
            title: 'Camera Dolly',
            description: 'Designing a camera dolly with a hydraulic manipulator',
            time: '2020',
            img: './projectImg/example-project.jpg'
        }
    ];
</script>

<style>
</style>

<svelte:head>
    <title>Sapper project template</title>
</svelte:head>

<AboutMe/>

<Item itemToShow={experience} title="EXPERIENCE"/>

<ProjectView projectsToShow={projects} showMore='/projects'/>

<Item itemToShow={honors} title="HONORS"/>


