<script>
    const cal_id = '42ae9bf55268920cdca87878eabe21fbf12e32cc19f32ffae05fc38233a5f558@group.calendar.google.com'
    const api_key = 'AIzaSyC_DNLR-eCZTfCCROJPlFHu-VRZAtbk0Uc'

    let CalendarData = []
    fetch(`https://www.googleapis.com/calendar/v3/calendars/${cal_id}/events?key=${api_key}`)
        .then(response => response.json())
        .then(data => {
            console.log(data);
            CalendarData = data.items
        })
        .catch(error => {
            console.error('Error:', error);
    });

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
    <div class="flex justify-center">
        <h1 class="text-green-700 text-6xl">{title}</h1>
    </div>
    
    <div class="flex flex-wrap justify-around">
        {#each events as event}
            <div class="w-1/3 px-5 flex">
                <div class="bg-red-500 text-white grow shadow-lg rounded-2xl px-4 py-4 flex flex-wrap">
                    <div class="capitalize md:uppercase decoration-solid w-full rounded-full bg-yellow-500 p-4">{event.title}</div>
                    <div class="italic">{event.content}</div>
                    <div class="flex items-end">{event.date}</div>
                </div>
            </div>         
        {/each}
    </div>
    <div>
        
    </div>
</div>

<style>


</style>
