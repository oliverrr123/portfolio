<script lang="ts">
    let websites: { title: string; description: string; image: string; link: string; }[] = [
        {
            title: 'Lettersmith construction company',
            description: 'A portfolio site for a London construction company - Comas Lettersmith Ltd including a couple images and an e-mail contact form.',
            image: 'lettersmith.png',
            link: 'https://comaslettersmith.co.uk/'
        },
        {
            title: 'Luma production',
            description: 'Another portfolio website, this time for my media production company - Luma production. It’s a simple one-pager including all the necessary info.',
            image: 'luma.png',
            link: 'https://luma-production.com/'
        },
        {
            title: 'SX Media',
            description: 'A showcase site of my work in documenting cars. Including a gallery with my best pics.',
            image: 'sxmedia.png',
            link: 'https://sx-media.vercel.app/'
        }
    ]
    let tools: { name: string; image: string; }[] = [
        {
            name: 'Adobe Premiere Pro',
            image: 'PremierePro.svg'
        },
        {
            name: 'Adobe After Effects',
            image: 'AfterEffects.svg'
        },
        {
            name: 'DaVinci Resolve',
            image: 'DaVinciResolve.svg'
        },
        {
            name: 'Adobe Photoshop',
            image: 'Photoshop.svg'
        },
        {
            name: 'Adobe Lightroom',
            image: 'Lightroom.svg'
        },
        // {
        //     name: 'Sony A6500 camera body',
        //     image: 'camera2.svg'
        // },
        // {
        //     name: 'DJI RS3 Mini gimbal',
        //     image: 'shake.svg'
        // }
    ]
</script>

<a href="/" class="text-white text-sm text-opacity-50 underline pt-16 block">{'<'}&nbsp; Back to main page</a>
<h1 class="text-3xl font-bold pb-8 pt-2">Media production</h1>
<h3 class="text-white text-opacity-80 text-lg font-light">One day I went to a drifting event with my friend. He borrowed me his camera and I took a couple of pictures. That’s when I got into it all. Since then, I’ve worked with multiple clients on creating marketing videos, car edits & photoshoots, music videos, and more...</h3>
<a href="https://luma-production.com/" target="_blank" class="text-xl font-semibold text-white text-opacity-90 block underline-offset-4 pt-20 pb-6"><span class="inline-flex gap-3 items-center border-b w-auto">More info on my media production website <img src="/icons/link.svg" alt="link" class="w-5 h-5"></span></a>
<h2 class="text-2xl font-semibold pt-20 pb-6 text-white text-opacity-90">Tools I use:</h2>
{#each tools as tool}
    <div class="flex gap-1 items-center">
        <img src="/icons/media-production/{tool.image}" alt="{tool.name}" class="w-12 h-12 p-2">
        <p>{tool.name}</p>
    </div>
{/each}
