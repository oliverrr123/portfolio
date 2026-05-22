<script lang="ts">
    let skills: { title: string; description: string; image: string; alt: string; link: string; }[] = [
        {
            title: 'GrowByte',
            description: 'This is my agency for custom website & AI solutions which I use to fund my other projects. ',
            image: 'growbyte-logo-with-motto.jpg',
            alt: 'GrowByte logo with motto',
            link: 'growbyte',
        },
        {
            title: 'MyFriend',
            description: '28% of elderly in the US live alone. That\'s why I created MyFriend, a cute AI companion robot.',
            image: 'myfriend-banner.jpg',
            alt: 'MyFriend banner',
            link: 'myfriend',
        },
        {
            title: 'Ambitious Shit',
            description: 'I feel like what I\'m currently building isn\'t at all the best I can do. That\'s why I\'m currently searching for something insane that I will build in the next 5-10 years.',
            image: 'san-francisco-skyline-at-night.jpg',
            alt: 'San Francisco skyline at night shot from Twin Peaks',
            link: 'ambitious-shit',
        }
    ]
    let projects: { title: string; image: string; alt: string; link: string; }[] = [
        {
            title: 'Luma production agency',
            image: 'luma-production-website-screenshot.png',
            alt: 'Screenshot of a website I built for Luma production agency',
            link: 'https://luma-production.com/'
        },
        {
            title: 'SX Media - car photos & videos',
            image: 'sx-media-website-screenshot.png',
            alt: 'Screenshot of a website I built for SX Media',
            link: 'https://sx-media.vercel.app/'
        },
        {
            title: 'GrowByte website',
            image: 'growbyte-website-screenshot.png',
            alt: 'Screenshot of a website I built for Growbyte company',
            link: 'https://growbyte.co/'
        }
    ]
</script>

<svelte:head>
    <title>Oliver Cingl | Founder and CEO of GrowByte</title>
</svelte:head>

<div class="flex w-full justify-center items-center pt-24 pb-6">
    <img src="/images/oliver-cingl-profile-picture.jpg" alt={"Oliver Cingl profile picture, a passionate cybersecurity student from Prague"} class="w-48 rounded-full">
</div>
<h1 class="text-4xl font-bold text-center pb-4">Hi, I'm Oliver</h1>
<h3 class="text-center text-white text-opacity-80 text-lg font-light">Currently builing <a target="_blank" class="text-blue-500 font-semibold underline" href="https://growbyte.co/myfriend">MyFriend</a></h3>
<h2 class="text-3xl font-semibold text-center pt-24 pb-12">My Projects</h2>
<section class="w-full flex flex-col justify-center gap-20">
    {#each skills as skill}
        <div class="flex flex-col gap-2">
            <img src="/images/{skill.image}" alt={skill.alt} class="w-full rounded-xl">
            <h3 class="font-bold text-lg mt-2">{skill.title}</h3>
            <p class="text-white text-opacity-75 pb-1">{skill.description}</p>
            <a href={skill.link}><button class="font-semibold bg-white text-[#181818] px-4 py-1.5 rounded-lg">Find out more</button></a>
        </div>
    {/each}
</section>
<!-- <h2 class="text-3xl font-semibold text-center pt-24 pb-12">My projects</h2>
<section class="w-full flex flex-col justify-center gap-20">
    {#each projects as project}
        <div class="flex flex-col gap-2">
            <img src="/images/{project.image}" alt={project.alt} class="w-full">
            <h3 class="font-bold text-lg mt-2">{project.title}</h3>
            <a href={project.link} target="_blank"><button class="font-semibold bg-white text-[#181818] rounded-lg px-4 py-1.5">See website</button></a>
        </div>
    {/each}
</section> -->