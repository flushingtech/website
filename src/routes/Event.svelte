<script>
    let title = "Event"
    let contents = "The Flushing Tech Meetup is thrilled to host its dynamic Bi-Weekly Hackathon, bringing together tech enthusiasts, developers, and innovators from the Flushing, Queens community and beyond. This recurring event serves as a collaborative platform for individuals with a passion for technology to engage in hands-on coding, problem-solving, and creative thinking."
    let events = [
        {
            title: "Bi-weekly Hackathon",
            content: contents,
            date: "Next date: Nov 18 2023"
        },
        {
            title: "After Hours",
            content: "Bar time!!!! Are you 21-years old?",
            date: "Next date: Nov 22 2023"
        },
        {
            title: "Virtual Session",
            content: "Can't attend the meetup in person? Join us on Zoom!",
            date: "Next date: Nov 22 2023"
        },
    ]
</script>


<div> 
    <h1 class="text-green-700 text-6xl grow">{title}</h1>
    <div class="flex flex-wrap ">
        {#each events as event}
            <div class="w-1/3 shadow-lg bg-orange-700 rounded-2xl px-5 mx-3">
                <p class="capitalize md:uppercase underline decoration-solid">{event.title}</p>
                {event.content} - {event.date}
            </div>         
        {/each}
    </div>
</div>

<style>


</style>
