<script lang="ts">
    let skills: { title: string; description: string; image: string; alt: string; link: string; }[] = [
        {
            title: 'Build a website',
            description: 'From building fun websites for myself to creating complex systems for companies, I have the skills to create pretty much any site you could imagine.',
            image: 'growbyte-website-screenshot.png',
            alt: 'Screenshot of a website I built for GrowByte company',
            link: 'web-development',
        },
        {
            title: 'Film & produce any video',
            description: 'My hobby of filming cars grew into a whole production company making marketing videos, music clips, car edits, or other videos & photos of any kind.',
            image: 'music-video-screenshot.png',
            alt: 'Screenshot of a music video I produced for Mark Steiner',
            link: 'media-production',
        },
        {
            title: 'Educate in IT',
            description: 'Since IT education in traditional schools is usually very poor, I decided to make fun workshops for children in elementary schools. I also teach teachers or whole companies.',
            image: 'it-education-workshop.png',
            alt: 'Picture from my IT education workshop',
            link: 'it-education',
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
    <title>Oliver Cingl</title>
</svelte:head>

<div class="flex w-full justify-center items-center pt-24 pb-6">
    <img src="/images/oliver-cingl-profile-picture.jpg" alt={"Oliver Cingl profile picture, a passionate cybersecurity student from Prague"} class="w-48 rounded-full">
</div>
<h1 class="text-4xl font-bold text-center pb-4">Hi, I'm Oliver</h1>
<h3 class="text-center text-white text-opacity-80 text-lg font-light">Currently helping businesses at <a target="_blank" class="text-blue-500 font-semibold underline" href="https://growbyte.co/">GrowByte</a></h3>
<h2 class="text-3xl font-semibold text-center pt-24 pb-12">What can I do?</h2>
<section class="w-full flex flex-col justify-center gap-20">
    {#each skills as skill}
        <div class="flex flex-col gap-2">
            <img src="/images/{skill.image}" alt={skill.alt} class="w-full">
            <h3 class="font-bold text-lg mt-2">{skill.title}</h3>
            <p class="text-white text-opacity-75 pb-1">{skill.description}</p>
            <a href={skill.link}><button class="font-semibold bg-white text-[#181818] rounded-lg px-4 py-1.5">Find out more</button></a>
        </div>
    {/each}
</section>
<h2 class="text-3xl font-semibold text-center pt-24 pb-12">My projects</h2>
<section class="w-full flex flex-col justify-center gap-20">
    {#each projects as project}
        <div class="flex flex-col gap-2">
            <img src="/images/{project.image}" alt={project.alt} class="w-full">
            <h3 class="font-bold text-lg mt-2">{project.title}</h3>
            <a href={project.link} target="_blank"><button class="font-semibold bg-white text-[#181818] rounded-lg px-4 py-1.5">See website</button></a>
        </div>
    {/each}
</section>