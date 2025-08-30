<script lang="ts">
    let websites: { title: string; description: string; image: string; alt: string; link: string; }[] = [
        {
            title: 'Real Estate',
            description: 'Showcase website of a real estate project.',
            image: 'client1.png',
            alt: 'Screenshot of a website I built for Growbyte company',
            link: 'https://modricka.realyx.cz/'
        },
        {
            title: 'Finance Company',
            description: 'Portfolio website of a finance company specializing in receivables.',
            image: 'client2.png',
            alt: 'Screenshot of a website I built for Luma production agency',
            link: 'https://expohledavky.cz/'
        },
        {
            title: 'Sales Funnel',
            description: 'Sales funnel for a personal growth course.',
            image: 'client3.png',
            alt: 'Screenshot of a website I built for SX Media',
            link: 'https://konzultace.martinkrejcir.cz/'
        }
    ]
    // let tools: { name: string; image: string; }[] = [
    //     {
    //         name: 'My Brain',
    //         image: 'brain.png'
    //     },
    //     {
    //         name: 'Next.js',
    //         image: 'nextjs.svg'
    //     },
    //     {
    //         name: 'Svelte',
    //         image: 'svelte.svg'
    //     },
    //     {
    //         name: 'TypeScript',
    //         image: 'typescript.svg'
    //     },
    //     {
    //         name: 'Tailwind',
    //         image: 'tailwind.svg'
    //     },
    //     {
    //         name: 'Supabase',
    //         image: 'supabase.svg'
    //     },
    //     {
    //         name: 'PostgreSQL',
    //         image: 'postgres.svg'
    //     },
    //     {
    //         name: 'Python',
    //         image: 'python.svg'
    //     },
    //     {
    //         name: 'GitHub',
    //         image: 'github.svg'
    //     },
    //     {
    //         name: 'Cursor',
    //         image: 'cursor.webp'
    //     },
    //     {
    //         name: 'Claude Code',
    //         image: 'claude.svg'
    //     }
    // ]
</script>


<svelte:head>
    <title>Oliver Cingl | GrowByte</title>
</svelte:head>

<a href="/" class="text-white text-sm text-opacity-50 underline pt-16 block">{'<'}&nbsp; Back to main page</a>
<h1 class="text-3xl font-bold pb-8 pt-2">GrowByte</h1>
<h3 class="text-white text-opacity-80 text-lg font-light">We make all kinds of websites and web apps, whether it's a simple one-page portfolio or a complex custom CRM.<br><br>We also MVPs and custom AI solutions to automate your business processes.<br><br>For most of our clients, we made a system for automatic email cold outreach. It automatically generates leads and sends them a personalized emails with followups.<br><br>Below are some examples of websites we built, to see more, including AI automations, contact me using the links on the bottom of the page.</h3>
<h2 class="text-xl font-semibold pt-20 pb-6 text-white text-opacity-90">Websites we built:</h2>
<section class="w-full flex flex-col justify-center gap-20">
    {#each websites as website}
        <div class="flex flex-col gap-2">
            <img src="/images/growbyte/{website.image}" alt={website.alt} class="w-full rounded-xl">
            <h2 class="font-bold text-lg mt-2">{website.title}</h2>
            <p class="text-white text-opacity-75 pb-1">{website.description}</p>
            <a href={website.link} target="_blank"><button class="font-semibold bg-white text-[#181818] rounded-lg px-4 py-1.5">See website</button></a>
        </div>
    {/each}
</section>
<a href="https://growbyte.co/" target="_blank" class="text-xl font-semibold text-white text-opacity-90 block underline-offset-4 pt-20 pb-20"><span class="inline-flex gap-3 items-center border-b w-auto">More info on the website <img src="/icons/link.svg" alt="Link to my media production agency website" class="w-5 h-5"></span></a>
<!-- <h2 class="text-2xl font-semibold pt-20 pb-6 text-white text-opacity-90">Tools I use:</h2>
{#each tools as tool}
    <div class="flex gap-1 items-center">
        <img src="/icons/growbyte/{tool.image}" alt="{tool.name} icon" class="w-12 h-12 p-2">
        <p>{tool.name}</p>
    </div>
{/each} -->
