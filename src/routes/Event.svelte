<script>
    let title = "Event"
    let content = "The Flushing Tech Meetup is thrilled to host its dynamic Bi-Weekly Hackathon, bringing together tech enthusiasts, developers, and innovators from the Flushing, Queens community and beyond. This recurring event serves as a collaborative platform for individuals with a passion for technology to engage in hands-on coding, problem-solving, and creative thinking."
    let events = [
        {
            title: "Bi-weekly Hackathon",
            content: content,
            date: "Next date: Nov 18 2023"
        },
        {
            title: "After Hours",
            content: "Bar time!!!! Are you 21-years old?",
            date: "Next date: Nov 22 2023"
        }
    ]
</script>


<div> 
    <h1 class="text-green-700 text-6xl grow">{title}</h1>
    {#each events as event}
            <div class="flex flex-wrap">
                <div class="m-1/2 w-1/4">
                    {event.title} - {event.content} - {event.date}
                </div>         
                <div class="m-1/2 w-1/4">
                    {event.title} - {event.content} - {event.date}
                </div>         
                <div class="m-1/2 w-1/4">
                    {event.title} - {event.content} - {event.date}
                </div>         
                <div class="m-1/2 w-1/4">
                    {event.title} - {event.content} - {event.date}
                </div>
            </div>
    {/each}
</div>

<style>


</style>
