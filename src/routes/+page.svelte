<script lang="ts">
    let skills: { title: string; description: string; image: string; link: string; }[] = [
        {
            title: 'Build a website',
            description: 'From building fun websites for myself to creating complex systems for companies, I have the skills to create pretty much any site you could imagine.',
            image: 'lettersmith.png',
            link: 'web-development'
        },
        {
            title: 'Film & produce any video',
            description: 'My hobby of filming cars grew into a whole production company making marketing videos, music clips, car edits, or other videos & photos of any kind.',
            image: 'videoclip.png',
            link: 'media-production'
        },
        {
            title: 'Educate in IT',
            description: 'Since IT education in traditional schools is usually very poor, I decided to make fun workshops for children in elementary schools. I also teach teachers or whole companies.',
            image: 'educate.png',
            link: 'it-education'
        }
    ]
    let projects: { title: string; image: string; link: string; }[] = [
        {
            title: 'Luma production agency',
            image: 'luma.png',
            link: 'https://luma-production.com/'
        },
        {
            title: 'SX Media - car photos & videos',
            image: 'sxmedia.png',
            link: 'https://sx-media.vercel.app/'
        },
        {
            title: 'Lettersmith construction website',
            image: 'lettersmith.png',
            link: 'https://comaslettersmith.co.uk/'
        }
    ]
</script>

<svelte:head>
    <title>Oliver Cingl</title>
</svelte:head>

<div class="flex w-full justify-center items-center pt-24 pb-6">
    <img src="/images/ksicht.png" alt="Avatar" class="w-48">
</div>
<h1 class="text-4xl font-bold text-center pb-4">Hi, I'm Oliver</h1>
<h3 class="text-center text-white text-opacity-80 text-lg font-light">A passionate cybersecurity student from Prague</h3>
<h1 class="text-3xl font-semibold text-center pt-24 pb-12">What can I do?</h1>
<section class="w-full flex flex-col justify-center gap-20">
    {#each skills as skill}
        <div class="flex flex-col gap-2">
            <img src="/images/{skill.image}" alt="Web development" class="w-full">
            <h2 class="font-bold text-lg mt-2">{skill.title}</h2>
            <p class="text-white text-opacity-75 pb-1">{skill.description}</p>
            <a href={skill.link}><button class="font-semibold bg-white text-[#181818] rounded-lg px-4 py-1.5">Find out more</button></a>
        </div>
    {/each}
</section>
<h1 class="text-3xl font-semibold text-center pt-24 pb-12">My projects</h1>
<section class="w-full flex flex-col justify-center gap-20">
    {#each projects as project}
        <div class="flex flex-col gap-2">
            <img src="/images/{project.image}" alt="Web development" class="w-full">
            <h2 class="font-bold text-lg mt-2">{project.title}</h2>
            <a href={project.link} target="_blank"><button class="font-semibold bg-white text-[#181818] rounded-lg px-4 py-1.5">Find out more</button></a>
        </div>
    {/each}
</section>