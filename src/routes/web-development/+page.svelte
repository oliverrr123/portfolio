<script lang="ts">
    let websites: { title: string; description: string; image: string; alt: string; link: string; }[] = [
        {
            title: 'GrowByte company',
            description: 'Site for an IT company I co-founded - GrowByte including a blog CMS and multiple contact forms.',
            image: 'growbyte-website-screenshot.png',
            alt: 'Screenshot of a website I built for Growbyte company',
            link: 'https://growbyte.co/'
        },
        {
            title: 'Luma production',
            description: 'Another portfolio website, this time for my media production company - Luma production. It’s a simple one-pager including all the necessary info.',
            image: 'luma-production-website-screenshot.png',
            alt: 'Screenshot of a website I built for Luma production agency',
            link: 'https://luma-production.com/'
        },
        {
            title: 'SX Media',
            description: 'A showcase site of my work in documenting cars. Including a gallery with my best pics.',
            image: 'sx-media-website-screenshot.png',
            alt: 'Screenshot of a website I built for SX Media',
            link: 'https://sx-media.vercel.app/'
        }
    ]
    let tools: { name: string; image: string; }[] = [
        {
            name: 'Next.js',
            image: 'nextjs.svg'
        },
        {
            name: 'Svelte',
            image: 'svelte.svg'
        },
        {
            name: 'TypeScript',
            image: 'typescript.svg'
        },
        {
            name: 'Tailwind',
            image: 'tailwind.svg'
        },
        {
            name: 'Supabase',
            image: 'supabase.svg'
        },
        {
            name: 'Prisma',
            image: 'prisma.svg'
        },
        {
            name: 'PostgreSQL',
            image: 'postgres.svg'
        },
        {
            name: 'Python',
            image: 'python.svg'
        },
        {
            name: 'GitHub',
            image: 'github.svg'
        },
    ]
</script>


<svelte:head>
    <title>Oliver Cingl | Web Development</title>
</svelte:head>

<a href="/" class="text-white text-sm text-opacity-50 underline pt-16 block">{'<'}&nbsp; Back to main page</a>
<h1 class="text-3xl font-bold pb-8 pt-2">Web development</h1>
<h3 class="text-white text-opacity-80 text-lg font-light">It all begun when I was just a small kid wanting to build a game. After making a couple of web games, I gained experience and built more websites. Now I’m able to create both visually pleasing and functional websites of any kind, for anyone.</h3>
<h2 class="text-xl font-semibold pt-20 pb-6 text-white text-opacity-90">Websites I built:</h2>
<section class="w-full flex flex-col justify-center gap-20">
    {#each websites as website}
        <div class="flex flex-col gap-2">
            <img src="/images/{website.image}" alt={website.alt} class="w-full">
            <h2 class="font-bold text-lg mt-2">{website.title}</h2>
            <p class="text-white text-opacity-75 pb-1">{website.description}</p>
            <a href={website.link}><button class="font-semibold bg-white text-[#181818] rounded-lg px-4 py-1.5">See website</button></a>
        </div>
    {/each}
</section>
<h2 class="text-2xl font-semibold pt-20 pb-6 text-white text-opacity-90">Tools I use:</h2>
{#each tools as tool}
    <div class="flex gap-1 items-center">
        <img src="/icons/web-development/{tool.image}" alt="{tool.name} icon" class="w-12 h-12 p-2">
        <p>{tool.name}</p>
    </div>
{/each}
